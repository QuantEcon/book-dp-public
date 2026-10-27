# Dynamic Programming Volumes 1 and 2

Public repo for the **Dynamic Programming** books by [Thomas J.
Sargent](http://www.tomsargent.com/) and [John
Stachurski](https://johnstachurski.net/).

| Folder | Description |
|--------|-------------|
| website | HTML files that build the website |
| pdf | PDF of the book |
| code | Public source of `py` and `jl` code |
| slides | Public source of supporting slides |

## PDF

The PDFs are available in `pdf/`

Comments and feedback are welcome.
The easiest way to provide feedback is to open an issue above.

## Website

This repository hosts the public book website. 

## Citation

Please cite the Cambridge University Press editions, including when working
from the free PDFs:

- Sargent, Thomas J. and John Stachurski (2025). *Dynamic Programming: Finite
  States*. Cambridge University Press. https://doi.org/10.1017/9781009540780
- Sargent, Thomas J. and John Stachurski (forthcoming, 2027). *Dynamic
  Programming: General States*. Cambridge University Press.

BibTeX entries are in [`website/cite/dp.bib`](website/cite/dp.bib) and at
[dp.quantecon.org/#cite](https://dp.quantecon.org/#cite).

### Keeping the citation in step

The citation appears in several places across three repositories. When it
changes — Volume II's DOI and final year, for instance — update all of them.

In this repository:

- `website/index.html`: the "How to cite" section, the `citation_*` meta
  tags and the JSON-LD
- `website/cite/dp1.bib`, `dp2.bib` and `dp.bib`
- `website/llms.txt`: the "How to cite" section
- `CITATION.cff`
- this README

In each volume's MyST edition (`mystmd/` on the `mystmd-conversion` branch
of book-dp1 and book-dp2):

- `index.md` and `licensing.md`: the "How to cite" sections
- `myst.yml`: the footer, and `doi:` (Volume I has it; add it for
  Volume II once Cambridge mints one)
- `scripts/build_llms_txt.py`: `HOW_TO_CITE`, which must match the section
  in `website/llms.txt` word for word

On the MyST pages, write a DOI as `doi:10.1017/…` text, not as a doi.org
link: mystmd turns any doi.org link into an automatically generated
reference fetched at build time.
