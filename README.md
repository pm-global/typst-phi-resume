# typst-phi-resume
Resume template in typst using a design system based on the golden ratio

Two parameters drive the entire document:
- body-size: base font size; everything visual derives from this
- ratio: proportional step between sizes/spaces (golden, ≈ 1.618)

Golden Ratio closed form, calculated on compile:
```ratio = (1 + calc.sqrt(5)) / 2```

## requirements
typst
```
brew install typst
```
text gyre termes (font) - Thanks to Gust.org
[https://www.gust.org.pl/projects/e-foundry/tex-gyre/termes](https://www.gust.org.pl/projects/e-foundry/tex-gyre/termes/tg_termes-otf-2_609-31_03_2026.zip)

## how-to
Use the template:
- Scroll to // HEADER
- Edit the template entries with your info, save
- ```typst compile resume.typ``` to generate a PDF of the resume

Edit the template itself:
- change only the body-size to adjust the entire document
- 

Change the font:
- Install the font you want to use on your system
- change the font line to your font
  ```(font: "TeX Gyre Termes", size: body-size)```
- ```label-size``` may need to be adjusted, was based on default font measurements
