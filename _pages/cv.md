---
layout: single
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<!--
  HOW TO UPDATE YOUR CV
  ----------------------
  This page just embeds a PDF. To update it:
    1. Edit cv-source/cv-template.tex (or paste your own LaTeX CV
       into that file, keeping the \begin{document} wrapper).
    2. Compile it to a PDF, e.g. `pdflatex cv-template.tex`, or
       upload it to Overleaf and click "Download PDF".
    3. Replace files/cv.pdf with the new PDF (same filename).
    4. Commit + push. That's it -- nothing else on this page
       needs to change.

  GitHub Pages can't compile LaTeX itself, so the compiled PDF
  has to be generated and committed manually. If you'd rather
  skip LaTeX entirely, you can also just export a CV from Word,
  Google Docs, etc. straight to PDF and drop it in as files/cv.pdf.

  Your previous hand-written Markdown CV content is preserved at
  _pages/cv-text-backup.md (visible at /cv-text/, not in the nav)
  in case you want to reuse any of that text.
-->

{% include base_path %}

<p>
  <a href="{{ base_path }}/files/cv.pdf" class="btn btn--large" download>
    <i class="fa fa-download" aria-hidden="true"></i> Download CV (PDF)
  </a>
</p>

<div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden;">
  <iframe src="{{ base_path }}/files/cv.pdf" width="100%" height="1000" style="border: none; display: block;">
    Your browser doesn't support embedded PDFs.
    <a href="{{ base_path }}/files/cv.pdf">Download the CV here</a> instead.
  </iframe>
</div>

<p style="font-size: 0.85em; color: #888; margin-top: 0.5em;">
  If the PDF doesn't display above (this can happen on some mobile browsers), use the download button instead.
</p>
