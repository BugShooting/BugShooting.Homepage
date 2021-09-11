---
layout: page
permalink: /free/
---

<div id="requestform">

  <h1>Request Free License</h1>
  The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a <a href="{{ site.baseurl }}/pricing">commercial license</a>.

  <form id="submitform">
    <div class="row mb-3">
      <div class="form-group">
        <label for="activationfile" class="col-sm-2 col-form-label">Email</label>
        <input class="form-control" type="email" placeholder="Email" required name="email" id="email" maxlength="100">
      </div>
    </div>
    <div class="row mb-3">
      <div class="form-group">
        <div class="form-check">
          <input class="form-check-input" type="checkbox" required name="agreement">
          <label class="form-check-label" for="agreement">Accept Bug Shooting <a href="{{ site.baseurl }}/agreement" target="_blank">License Agreement</a></label>
        </div>
      </div>
    </div>
    <div class="row mb-3">
      <div class="form-group">
        <button class="btn btn-lg btn-primary btn-block" type="submit">Request Free License</button>
      </div>
    </div>
  </form>
  
</div>

<div id="resultsuccess" style="display:none">
 <h1>Thank You</h1>
 You will receive your Bug Shooting license by email. Please check your spam folder in case you do not receive the email. 
</div>

<div id="resultfailed" style="display:none">
  <h1>Oops!</h1>
  Something went wrong.
</div>

<script type="text/javascript">

  const form = document.getElementById('submitform');
  
  form.addEventListener('submit', (event) => {

    // disable default action
    event.preventDefault();

    var data = new FormData();
    data.append('email', document.getElementById("email").value);
    data.append('language', 'en-US');

    var request = new XMLHttpRequest();
  
    request.open("POST", "http://localhost:23423/rest/freelicense");
    request.setRequestHeader('Content-type', 'application/x-www-form-urlencoded');
    request.send(data);

    request.onload = (e) => {

      if (request.response === '0') {

        // success
        document.getElementById("requestform").style.display = "none";
        document.getElementById("resultsuccess").style.display = "block";

      } else {

        // failed
        document.getElementById("requestform").style.display = "none";
        document.getElementById("resultfailed").style.display = "block";

      }

    }
    
});
 
</script>
