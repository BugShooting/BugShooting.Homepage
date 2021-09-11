---
layout: page
permalink: /free/
---

<script type="text/javascript">

  var data = new FormData();
  data.append('email', document.getElementById("email").value);
  data.append('language', 'en-US');
  
  const request = new XMLHttpRequest();
    
  request.open("POST", "https://services.bugshooting.com/rest/freelicense");
  request.send(data);

  request.onload = (e) => {
  
    var requestform = document.getElementById("requestform");
    var result = document.getElementById("result");
  
    requestform.style.display = "none";
  
    if (request.response === 0) {
      // success
      result.style.display = "block";
      
    } else {
      // failed
      result.style.display = "block";
    }
  
     document.getElementById("releasenotes").innerHTML = request.response;
  }
  
</script>

<div id="requestform">

  # Request Free License

  The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a [commercial license]({{ site.baseurl }}/pricing).

  <form>
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
 # Thank You
 You will receive your Bug Shooting license by email. Please check your spam folder in case you do not receive the email. 
</div>
<div id="resultfailed" style="display:none">
  # Oops!
  Something went wrong.
</div>
