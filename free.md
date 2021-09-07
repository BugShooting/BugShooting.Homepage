---
layout: page
permalink: /free/
---

# Request Free License

The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a [commercial license]({{ site.baseurl }}/pricing).

<form method="POST" action="https://services.bugshooting.com/rest/freelicense">
  <div class="form-group row">
    <label for="activationfile" class="col-sm-2 col-form-label">Email</label>
    <input class="form-control" type="email" placeholder="Email" required name="email" maxlength="100">
  </div>
  <div class="form-group row">
    <div class="form-check">
      <input class="form-check-input" type="checkbox" required name="agreement">
      <label class="form-check-label" for="agreement">Accept Bug Shooting <a href="{{ site.baseurl }}/agreement" target="_blank">License Agreement</a></label>
    </div>
  </div>
  <input type="hidden" name="language" value="en-US">
  <input type="hidden" name="successurl" value="{{ site.url }}{{ site.baseurl }}/freesuccess">
  <input type="hidden" name="failurl" value="{{ site.url }}{{ site.baseurl }}/free">
  <div class="form-group row">
    <button class="btn btn-lg btn-primary btn-block" type="submit">Request Free License</button>
  </div>
</form>
