---
title: Google CSE
layout: page
permalink: /search/google.html
# optional Google search page, see docs/google.md
# set google-cse-id in _config.yml
---

## Sitio de búsqueda de Google

<div class="alert alert-primary" role="alert">
  Tenga en cuenta: CSE es un servicio gratuito proporcionado por Google. Los resultados dependen de la indexación de terceros y pueden contener anuncios.
</div>

<script>
  (function() {
    var cx = '{{ site.google-cse-id }}';
    var gcse = document.createElement('script');
    gcse.type = 'text/javascript';
    gcse.async = true;
    gcse.src = 'https://cse.google.com/cse.js?cx=' + cx;
    var s = document.getElementsByTagName('script')[0];
    s.parentNode.insertBefore(gcse, s);
  })();
</script>
<gcse:search></gcse:search>
