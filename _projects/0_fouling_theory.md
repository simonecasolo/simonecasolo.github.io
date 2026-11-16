---
layout: page
title: Heat Exchangers Fouling Theory
description: Stochastic fouling theory for heat exchangers - why one asymptotic fouling curve can hide four different removal mechanisms.
img: assets/img/fouling_theory.png
importance: 0
category: work
related_publications: false
---

An asymptotic fouling curve is usually read as the signature of shear removal, but erosion, detachment, sloughing and surface saturation all produce exactly the same mean curve. This interactive explainer shows how the scatter around the mean tells them apart, and how much measurement noise limits what a thermally reconstructed fouling resistance can reveal about the deposition law.

[Open the explainer in a full page](/assets/html/fouling_theory.html){:target="_blank"}

<iframe
  id="fouling-frame"
  src="{{ '/assets/html/fouling_theory.html' | relative_url }}"
  title="One fouling curve, four mechanisms"
  style="width:100%;height:2600px;border:1px solid var(--global-divider-color);border-radius:8px;"
  loading="lazy"></iframe>

<script>
  (function () {
    var f = document.getElementById("fouling-frame");
    function fit() {
      try {
        var d = f.contentWindow.document;
        f.style.height = d.documentElement.scrollHeight + "px";
      } catch (e) {}
    }
    f.addEventListener("load", function () {
      fit();
      try { new ResizeObserver(fit).observe(f.contentWindow.document.body); } catch (e) {}
    });
    window.addEventListener("resize", fit);
  })();
</script>
