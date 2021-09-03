---
layout: page
permalink: /free/
---

# Request Free License

The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a [commercial license]({{ site.baseurl }}/buy).

<form method="POST" action="https://Services.bugshooting.com/rest/freelicense">
  <input class="form-control" type="text" required name="firstname" placeholder="First Name">
  <input class="form-control" type="text" required name="lastname" placeholder="Last Name">
  <input class="form-control" type="text" required name="email" placeholder="E-Mail">
  <input class="form-control" type="text" required name="email2" placeholder="Retype E-Mail">
  <input class="form-control" type="text" required name="country" placeholder="Country">
  <input class="form-control" type="text" required name="city" placeholder="City">
  <input class="form-control" type="text" required name="zip" placeholder="ZIP / Postal Code">
  <input class="form-control" type="text" required name="street" placeholder="Street Address">
  <input class="form-check-input" type="checkbox" id="AgreementCheckbox" required name="agreement">
  <label class="form-check-label" for="AgreementCheckbox">Accept Bug Shooting <a href="{{ site.baseurl }}/agreement">License Agreement</a></label>
  <button class="btn btn-lg btn-primary btn-block" type="submit">Request Free License</button>
</form>
