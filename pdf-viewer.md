---
layout: default
title: PDF Viewer
permalink: /pdf-viewer.html
---

<script type="text/javascript">
  const urlParams = new URLSearchParams(window.location.search);
  const pdfFile = urlParams.get('file');
  
  if (pdfFile) {
    setTimeout(function() {
      window.location.href = "/pdf/" + pdfFile;
    }, 100);
  } else {
    window.location.href = "/";
  }
</script>

<div style="text-align: center; padding: 50px;">
  <p>Loading PDF...</p>
  <p>If the download doesn't start, <a href="javascript:history.back()">click here to go back</a>.</p>
</div>