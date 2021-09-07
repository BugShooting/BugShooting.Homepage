---
layout: page
permalink: /free/
---

# Request Free License

The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a [commercial license]({{ site.baseurl }}/pricing).

<form method="POST" action="https://services.bugshooting.com/rest/freelicense">
  <div class="row mb-3">
    <label for="email" class="col-sm-2 col-form-label">E-Mail</label>
    <div class="col-sm-4">
      <input class="form-control" type="email" required name="email" maxlength="100">
    </div>
  </div>
  <div class="row mb-3">
    <div class="col-sm-10  offset-sm-2">
      <div class="form-check">
        <input class="form-check-input" type="checkbox" required name="agreement">
        <label class="form-check-label" for="agreement">Accept Bug Shooting <a href="{{ site.baseurl }}/agreement" target="_blank">License Agreement</a></label>
      </div>
    </div>
  </div>
  <input type="hidden" name="language" value="en-US">
  <input type="hidden" name="successurl" value="{{ site.url }}{{ site.baseurl }}/freesuccess">
  <input type="hidden" name="failurl" value="{{ site.url }}{{ site.baseurl }}/free">
  <div class="row mb-3">
    <div class="col-sm-4  offset-sm-2">
       <button class="btn btn-lg btn-primary btn-block" type="submit">Request Free License</button>
    </div>
  </div>
</form>
