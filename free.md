---
layout: page
permalink: /free/
---

# Request Free License

The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a [commercial license]({{ site.baseurl }}/buy).

<form method="POST" action="https://Services.bugshooting.com/rest/freelicense">
  <div class="mb-3">
    <label for="firstname" class="form-label">First Name</label>
    <input class="form-control" type="text" required name="firstname" >
  </div>
  <div class="mb-3">
    <label for="lastname" class="form-label">Last Name</label>
    <input class="form-control" type="text" required name="lastname">
  </div>
  <div class="mb-3">
    <label for="email" class="form-label">E-Mail</label>
    <input class="form-control" type="email" required name="email">
  </div>
  <div class="mb-3">
    <label for="email2" class="form-label">Retype E-Mail</label>
    <input class="form-control" type="email" required name="email2"
  </div>
  <div class="mb-3">
    <label for="country" class="form-label">Country</label>
    <input class="form-control" type="text" required name="country">
  </div>
  <div class="mb-3">
    <label for="city" class="form-label">City</label>
    <input class="form-control" type="text" required name="city">
  </div>
  <div class="mb-3">
    <label for="zip" class="form-label">ZIP / Postal Code</label>
    <input class="form-control" type="text" required name="zip">
  </div>
  <div class="mb-3">
    <label for="street" class="form-label">Street Address</label>
    <input class="form-control" type="text" required name="street">
  </div>
  <div class="mb-3 form-check">
    <input class="form-check-input" type="checkbox" required name="agreement">
    <label class="form-check-label" for="agreement">Accept Bug Shooting <a href="{{ site.baseurl }}/agreement" target="_blank">License Agreement</a></label>
  </div>
  <button class="btn btn-lg btn-primary btn-block" type="submit">Request Free License</button>
</form>
