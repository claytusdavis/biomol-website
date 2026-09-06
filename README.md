# Molecular Biology, Life Sciences (MBMLS)

Course companion site, migrated from a Dreamweaver-authored site previously served
from `fohs.bgu.ac.il` at Ben-Gurion University of the Negev.

The site is entirely static — HTML and one stylesheet, no JavaScript and no server
code. It is published with GitHub Pages.

**Entry point:** [`mbmls/mbmls_HTMLs/mbmlshome.html`](mbmls/mbmls_HTMLs/mbmlshome.html)
(the root `index.html` redirects there).

## Layout

The original directory structure is preserved deliberately, so that every relative
link in the pages (`../../Images/…`, `../mbmls_PDFs/…`) keeps working unchanged.

```text
index.html               redirect to the course home page
teachtemplatestyles.css  the single shared stylesheet
Images/                  shared images and lecture maps
mbmls/
  mbmls_HTMLs/           the 24 course pages
  mbmls_PDFs/            study guides, handouts, lab material
MCB/
  MCB_HTMLs/             six "medical perspective" pages linked from the lectures
  MCB_pdfs/              study guides and journal articles for those pages
mbmed/, dbee/            two PDFs and one movie referenced from the lectures
```

## What was changed during migration

- The PHP login gate was removed; the site is now static and open.
- Six broken links inherited from the original site were repaired.
- Dreamweaver's stale absolute `file:///` references were removed.
- Publisher-copyrighted material is not redistributed here: the *Molecular Biology
  of the Cell* 6th ed. animations and the scanned chapters from Cooper, *The Cell*.
  Their links were unwrapped to plain text and marked *[not available on this site]*,
  so the reading list still reads correctly.
- Unreferenced files from the original folder were not carried over.

Dreamweaver template markers (`<!-- InstanceBegin … -->`) and Library item
comments are left in place; they are inert in the browser.
