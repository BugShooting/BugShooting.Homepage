---
layout: page
permalink: /free/
---

# Request Free License

The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a [commercial license]({{ site.baseurl }}/buy).

<form method="POST" action="https://Services.bugshooting.com/rest/freelicense">
  <div class="mb-3">
    <input class="form-control" type="text" required name="firstname" placeholder="First Name">
  </div>
  <div class="mb-3">
    <input class="form-control" type="text" required name="lastname" placeholder="Last Name">
  </div>
  <div class="mb-3">
    <input class="form-control" type="text" required name="email" placeholder="E-Mail">
  </div>
  <div class="mb-3">
    <input class="form-control" type="text" required name="email2" placeholder="Retype E-Mail">
  </div>
  <div class="mb-3">
    <input class="form-control" type="text" required name="country" placeholder="Country">
  </div>
  <div class="mb-3">
    <input class="form-control" type="text" required name="city" placeholder="City">
  </div>
  <div class="mb-3">
    <input class="form-control" type="text" required name="zip" placeholder="ZIP / Postal Code">
  </div>
  <div class="mb-3">
    <input class="form-control" type="text" required name="street" placeholder="Street Address">
  </div>
  <div class="mb-3 form-check">
    <input class="form-check-input" type="checkbox" id="AgreementCheckbox" required name="agreement">
    <label class="form-check-label" for="AgreementCheckbox">Accept Bug Shooting <a href="{{ site.baseurl }}/agreement" target="_blank">License Agreement</a></label>
  </div>
  <button class="btn btn-lg btn-primary btn-block" type="submit">Request Free License</button>
</form>
