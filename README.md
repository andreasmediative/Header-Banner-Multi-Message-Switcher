# Header Banner Multi-Message Switcher

This switches the header banner based on which creative is clicked. You can add as many sets as you want.

You can view an example [here](https://mediativecreative.github.io/Header-Banner-Multi-Message-Switcher/index.html)

CSS:
```
<style>.media-banner{margin:0;height:0;overflow:hidden}.md_hb_show{margin:auto;height:auto;overflow:auto}</style>
```

JQuery:
```
<script>

jQuery(document).ready(function(e) {
  var mdSet = window.location.href;
  if (mdSet.indexOf("set2") > 0) {
    if (jQuery(window).width() >= 959) {
      jQuery("#md_hb_set1 .desktop-only").addClass("md_hb_show");
    } else if (jQuery(window).width() >= 640) {
      jQuery("#md_hb_set1 .tablet-only").addClass("md_hb_show");
    } else {
      jQuery("#md_hb_set1 .mobile-only").addClass("md_hb_show");
    }
  } else {
    if (jQuery(window).width() >= 959) {
      jQuery("#md_hb_set2 .desktop-only").addClass("md_hb_show");
    } else if (jQuery(window).width() >= 640) {
      jQuery("#md_hb_set2 .tablet-only").addClass("md_hb_show");
    } else {
      jQuery("#md_hb_set2 .mobile-only").addClass("md_hb_show");
    }
  }
});

</script>
```

Sample HTML:
```

<div id="md_hb_set1">
  <div class="media-banner row desktop-only">
    <img src="http://i.walmartimages.ca/img/mediative/Samsung-Q4-2017/14270-Mobile_Holiday/free-3-month-texture-subscription-prom3-with-select-samsung-tablets-e.png" alt="THIS IS THE ALT TEXT" title="THIS IS THE TITLE" />
  </div>

  <div class="media-banner row tablet-only">
    <img src="http://i.walmartimages.ca/img/mediative/Samsung-Q4-2017/14270-Mobile_Holiday/free-3-month-texture-subscription-prom3-with-select-samsung-tablets-tb-e.png" alt="THIS IS THE ALT TEXT" title="THIS IS THE TITLE" />
  </div>

  <div class="media-banner row mobile-only">
    <img src="http://i.walmartimages.ca/img/mediative/Samsung-Q4-2017/14270-Mobile_Holiday/free-3-month-texture-subscription-prom3-with-select-samsung-tablets-mb-e.png" alt="THIS IS THE ALT TEXT" title="THIS IS THE TITLE" />
  </div>
</div>


<div id="md_hb_set2">
  <div class="media-banner row desktop-only">
    <img src="http://i.walmartimages.ca/img/mediative/Samsung-Q4-2017/14308%20-samsung_CE/great-offers-3-from-samsung-tv-e.png" alt="THIS IS THE ALT TEXT" title="THIS IS THE TITLE" />
  </div>

  <div class="media-banner row tablet-only">
    <img src="http://i.walmartimages.ca/img/mediative/Samsung-Q4-2017/14308%20-samsung_CE/great-offers-3-from-samsung-tv-tb-e.png" alt="THIS IS THE ALT TEXT" title="THIS IS THE TITLE" />
  </div>

  <div class="media-banner row mobile-only">
    <img src="http://i.walmartimages.ca/img/mediative/Samsung-Q4-2017/14308%20-samsung_CE/great-offers-3-from-samsung-tv-mb-e.png" alt="THIS IS THE ALT TEXT" title="THIS IS THE TITLE" />
  </div>
</div>
```


