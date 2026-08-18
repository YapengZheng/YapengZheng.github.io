# Yapeng Zheng's Personal Website

A simple, clean personal website for Yapeng Zheng, PhD student in Economics at CUHK.

## Features

- Clean, minimal single-page design
- No build step required
- Fast loading
- Mobile responsive
- Simple HTML/CSS only

## Structure

- `index.html` - Homepage with all essential information
- `CV.tex` - LaTeX source for the CV
- `files/CV.pdf` - Compiled CV (deployed)
- `Yapengzheng_CV.pdf` - Compiled CV (root copy)

## Updating the CV

The CV is generated from `CV.tex`. To update it:

```bash
xelatex CV.tex
cp CV.pdf files/CV.pdf
cp CV.pdf Yapengzheng_CV.pdf
```

## Local Development

Open `index.html` directly in a browser, or serve it locally:

```bash
python -m http.server 4000
```

Then visit `http://localhost:4000`

## Deployment

This site is automatically deployed to GitHub Pages when pushed to the main branch.
