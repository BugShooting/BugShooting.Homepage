---
layout: page
permalink: /free/
---

# Request Free License

The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a [commercial license]({{ site.baseurl }}/pricing).

<form method="POST" action="https://services.bugshooting.com/rest/freelicense">
  <div class="row mb-3">
    <input class="form-control" type="email" placeholder="E-Mail" required name="email" maxlength="100">
  </div>
  <div class="row mb-3">
    <div class="form-check">
      <input class="form-check-input" type="checkbox" required name="agreement">
      <label class="form-check-label" for="agreement">Accept Bug Shooting <a href="{{ site.baseurl }}/agreement" target="_blank">License Agreement</a></label>
    </div>
  </div>
  <input type="hidden" name="language" value="en-US">
  <input type="hidden" name="successurl" value="{{ site.url }}{{ site.baseurl }}/freesuccess">
  <input type="hidden" name="failurl" value="{{ site.url }}{{ site.baseurl }}/free">
  <button class="btn btn-lg btn-primary btn-block" type="submit">Request Free License</button>
</form>
