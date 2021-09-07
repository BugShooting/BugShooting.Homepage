---
layout: page
permalink: /pricing/
---

# Buy For Comercial Usage

{% for price in site.data.prices %}

<div class="bs-callout bs-callout-warning">
  <div class="row">
    <div class="col-md-4">
      <p>{{ price.title }}</p>
      <p>{{ price.price_title }} <span class="price_small">{{ price.price }}</span></p>
    </div>
    
    {% if price.price_title == '' %}

      <div class="col-md-6">
        <a class="btn btn-yellow" href="{{ price.purchase_link }}">Purchase</a>
      </div>
    
    {% else %}

      <div class="col-md-3">
        <a class="btn btn-yellow" href="{{ price.purchase_link }}">Purchase</a>
      </div>
      <div class="visible-sm visible-xs">
        <br />
      </div>
      <div class="col-md-5">
        <a class="btn btn-yellow" href="{{ price.purchase_volume_link }}">Purchase volume license</a>
      </div>
    
    {% endif %}

  </div>
</div>

{% endfor %}