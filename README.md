# CCNC 2016 Presentation
**Secure Proximity-Based Identity Pairing using an Untrusted Signalling Service**

To be presented in the Session is Consumer Communications and Networking session of CCNC 2016.

14:00 - 15:30, 11th January 2016, Sunset 6, Planet Hollywood, Las Vegas. Talk duration should be about 15 mins.

You'll need LaTeX, pdflatex, beamer and make to build the presentation PDF.

When editing, the main text goes in `main.tex`. Bibliography items in `main.bib`. Images (PDF, PNG, JPEG) go in the `figures` folder.

To build the document:
```
main
```

This essentially performs the following.

```
pdflatex main
bibtex main
pdflatex main
pdflatex main
```

This should build a PDF file main.pdf of the presentation.

You can use `make clean` to remove temporary build files.

To turn on/off generation of the notes pages, change the flag in the ``documentclass`` declaration at the top of `main.tex` so it matches one of the following.

```
\documentclass[handout, notes=hide]{beamer}
\documentclass[handout, notes=show]{beamer}
```
