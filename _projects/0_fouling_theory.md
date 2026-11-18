---
layout: page
title: Heat Exchangers Fouling Theory
description: A stochastic fouling theory for heat exchangers - why one asymptotic fouling curve can hide different removal mechanisms.
img: assets/img/fouling_theory.png
importance: 0
category: work
related_publications: false
---

[Open the explainer in a full page](/assets/html/fouling_theory.html){:target="_blank" rel="noopener"}

<iframe
  id="fouling-frame"
  src="{{ '/assets/html/fouling_theory.html' | relative_url }}"
  title="One fouling curve, four mechanisms"
  style="width:100%;height:2600px;border:1px solid var(--global-divider-color);border-radius:8px;"
  scrolling="no"
  loading="lazy"></iframe>

<script>
  (function () {
    var f = document.getElementById("fouling-frame");
    function fit() {
      try {
        var d = f.contentWindow.document;
        f.style.height = d.body.offsetHeight + "px";
      } catch (e) {}
    }
    f.addEventListener("load", function () {
      fit();
      try { new ResizeObserver(fit).observe(f.contentWindow.document.body); } catch (e) {}
    });
    window.addEventListener("resize", fit);
  })();
</script>
