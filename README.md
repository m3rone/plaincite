# plaincite

CLI app that generates citations and references in plaintext files using Bib(La)TeX bibliography and CSL (written in Rust. Fancy)

## What?

You can use placeholders (like `[@author2024]`, markdown/pandoc style bibtex citekeys) in your plaintext file (.txt, .html, whatever you want as long as it does not have `[@validcitekey]` in it for things that are not citations) and supply a BibTeX/BibLaTeX bibliography file and a CSL file for your preferred citation style. 

The app is really only useful for numerical styles like IEEE, Vancouver, AMA, Nature, etc as whatever reference management software you use (Zotero, Mendeley, MyBib, etc) can just do author year citations for you.

Basically RTF scan feature in Zotero but for plaintext files.

## Installation

Right now, you can't. It's not ready.

## Usage

First, export your bibliography to BibTeX or BibLaTeX format, doesnt matter (or at least probably won't matter when I'm writing the app). Make sure the file you have the citations in has correct citekeys in the correct format.

And then probably something like 

```sh
plaincite --bib /path/to/bibliography.bib --csl /path/to/ieee.csl --input /path/to/input.html --output /path/to/output.html
```

It's not ready yet though. Maybe star it and come back later. I'm learning Rust as I'm writing this, unfortunately.

## Contributions

Everything welcome
