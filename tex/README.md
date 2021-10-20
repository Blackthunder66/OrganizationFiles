# TeX / LaTeX / BibTeX

## Content

- References harmonized for my group in (a huge) .bib file: [references_all.bib](biblio/references_all.bib)

- Snippets used for LaTeXing with Sublime (to be adapted for VSCode).

- Plain TeX templates

|[article.tex](draft-article/article.tex)| [exam.tex](draft-exam/exam.tex)| [scribe.tex](draft-scribe/scribe.tex) |
| ----------- |----------- |----------- |
|[<img src="../sharedimages/article.png" width="210" height="150">](draft-article/article.tex)|[<img src="../sharedimages/examen.png" width="210" height="150">](draft-exam/exam.tex)|[<img src="../sharedimages/scribe.png" width="210" height="150">](draft-scribe/scribe.tex)|


- Beamer TeX templates

|[beamer_tl_js.tex](draft-beamer/beamer_tl_js.tex) |[beamer_js.tex](draft-beamer/beamer_js.tex) | [beamer_tl.tex](draft-beamer/beamer_tl.tex)|
| ----------- | ----------- |----------- |
|[<img src="../sharedimages/beamer_tl_js.png" width="320" height="180">](draft-beamer/beamer_js.tex)|[<img src="../sharedimages/beamer_js.png" width="320" height="180">](draft-beamer/beamer_tl.tex)|[<img src="../sharedimages/beamer_tl.png" width="320" height="180">](draft-beamer/beamer_tl.tex)|



## Text Editor

Among the useful tools a modern editor (like [VSCode](https://code.visualstudio.com/) or [Sublime Text](https://www.sublimetext.com/)).
On top of that useful tools connected to LaTeX include, in particular useful tools include
- snippets
- multi-cursors
- forward/backward search: so you can click the generated pdf and find the tex location in your document (something now common with Overleaf). With VSCode, it can be done with a Ctrl+click, simply add to `settings.json` the entry:
```json
"latex-workshop.synctex.synctexjs.enabled": true,
```

For more VSCode help see for instance:
<https://danmackinlay.name/notebook/vs_code_for_latex.html>

## Additional tools

- https://www.tablesgenerator.com/ : to create LaTeX tables from copy/paste values or .csv files
- Inkscape (see for more information in the [Inkscape](../inkscape/README.md) section): useful for sketching figures with, especially with the [TexText](https://inkscape.org/~jcwinkler/%E2%98%85textext) extension.
- latexdiff : allows to visualize the diff in the pdf (useful for revision / v2 in a publication):

	`file1.tex file2.tex > diff.tex`

	Then, you can compile the file diff.tex and you get some nice difference file in the output pdf.


## Latex tips

1. Tools for Latex: Table generator http://www.tablesgenerator.com/ and  OCR for Latex formulas https://mathpix.com/

2. **Warning** font style :
```math
SNR \neq $SNR$
```

3. Add space on which you optimize:
```math
\min_{x \in X}
```
is **good**,
```math
\min_{x}
```
is *forbidden*.

4. **Always use**  *\enspace* at the of align/equation environments; e.g., :
```math
\begin{align}
x + 3 \enspace.
\end{align}
```
and not
```math
\begin{align}
x + 3.
\end{align}
```

## English rules
1. **HARMONIZE notation**
1. isn't -> **is not**, can't -> **can not**, let's -> **let us**
1. **Do not use** "I", "my". **Use** "royal", "we".
1. **Never** start a sequence by a formula.
1. **Use . , ;** at the end of a formula.
1. **Refrain** for using "will".
1. "permit" no so popular, **use** "allow".
1. **Number should often be a letter**: "3 times larger" -> "three times larger"
1. Notation without **s** for math.
1. Present tense, third person: "he, she, it", **add* an "s" at the end.

1. **Define** (almost) all "symbols you use".
1. **Define** concepts in correct order.
