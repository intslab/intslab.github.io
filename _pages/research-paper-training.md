---
layout: page
title: 科研入门培训
permalink: /research-paper-training/
description: 科研入门培训 PDF 下载
nav: false
pdf_path: /assets/pdf/intslab科研入门培训.pdf
_styles: |
  .training-download-count {
    color: #c00000;
    font-weight: 700;
  }
---

正在打开科研入门培训 PDF。

<p id="busuanzi_container_page_pv" class="training-download-count">
  累计下载 <span id="busuanzi_value_page_pv">...</span> 次
</p>

如果 PDF 没有自动打开，请[点击这里]({{ page.pdf_path | relative_url }})。

<script>
  (function () {
    var pdfUrl = "{{ page.pdf_path | relative_url }}";
    var redirected = false;

    function openPdf() {
      if (redirected) return;
      redirected = true;
      window.location.href = pdfUrl;
    }

    var attempts = 0;
    var timer = window.setInterval(function () {
      attempts += 1;
      var counter = document.getElementById("busuanzi_value_page_pv");

      if ((counter && counter.textContent.trim() && counter.textContent.trim() !== "...") || attempts >= 20) {
        window.clearInterval(timer);
        window.setTimeout(openPdf, 250);
      }
    }, 150);

    window.setTimeout(openPdf, 4000);
  })();
</script>
