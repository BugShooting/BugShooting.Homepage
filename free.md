---
layout: page
permalink: /free/
---

# Request Free License  
  
The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a <a href="{{ site.baseurl }}/pricing">commercial license</a>.  

<div id="errorMessage" class="alert alert-danger" role="alert" style="display:none"></div>
<div id="successMessage" class="alert alert-success " role="alert">
  You will receive your Bug Shooting license by email. Please check your spam folder in case you do not receive the email.
</div> 
 
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


<div id="resultfailed" style="display:none">
  <h1>Oops!</h1>
  Something went wrong.
</div>

<script type="text/javascript">

  const form = document.getElementById('submitform');
  
  form.addEventListener('submit', (event) => {

    // disable default action
    event.preventDefault();

    var xhr = new XMLHttpRequest();
  
    xhr.onload = function () {
      if (xhr.readyState === xhr.DONE) {
        
        form.reset();
  
        if (xhr.status === 200) {
  
          // show success message
          document.getElementById("successMessage").style.display = "block";
          document.getElementById("errorMessage").style.display = "none";
          form.style.display = "none";
  
        } else {
   
          // show error message
          document.getElementById("successMessage").style.display = "none"; 
          document.getElementById("errorMessage").style.display = "block";
          document.getElementById("errorMessage").innerText = xhr.statusText; 
  
        }
      }
    };
    
    xhr.open("POST", "https://services.bugshooting.com/rest/freelicense", true);
  
    var data = new FormData();
    data.append('email', document.getElementById("email").value);
    data.append('language', 'en-US');
  
    xhr.send(data);
        
  });
 
</script>
