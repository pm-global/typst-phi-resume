# typst-phi-resume
Resume template in typst using a golden ratio design system

Two parameters drive the entire document:
- body-size: base font size; everything visual derives from this
- ratio: proportional step between sizes/spaces (golden, ≈ 1.618)

Golden Ratio closed form, calculated on compile:
- ```ratio = (1 + calc.sqrt(5)) / 2```

![https://github.com/pm-global/typst-phi-resume](https://github.com/pm-global/typst-phi-resume/blob/main/resume.png)

## requirements
1. typst (2 options):
- if you have brew: ```$ brew install typst ```
- or, download from typst: [Go to typst downloads](https://typst.app/open-source/#download) 
2. Text Gyre Termes font: [Download Text Gyre Termes from GUST.org](https://www.gust.org.pl/projects/e-foundry/tex-gyre/termes/tg_termes-otf-2_609-31_03_2026.zip)

## how-to
Use the template:
- Scroll to // HEADER
- Edit the template entries with your info, save
- ```typst compile ./resume.typ``` to generate a PDF of the resume

Edit the template itself:
- Change only the body-size to adjust the entire document
  - increase body-size for shorter resumes
- Changing other definitions / variables will probably break the document 

Change the font:
- Install the font on your system
- change the font line
  ```(font: "TeX Gyre Termes", size: body-size)```
- ```label-size``` may need to be adjusted, it was based on default font measurements

Assisted by Claude Opus 4.7
