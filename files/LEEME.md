# Como usar esta carpeta

Archivos: main.tex (manuscrito anonimo), portada.tex (titulo + autores, se sube aparte), referencias.bib.

## Antes de compilar
Copia en esta misma carpeta, desde la plantilla oficial de SAGE (Overleaf o Author Gateway):
- sagej.cls
- SageH.bst
- SAGE_Logo (archivo de imagen que trae la plantilla)
No los modifiques (las reglas de uso de SAGE no lo permiten).

## Compilar (VS Code + LaTeX Workshop o terminal)
pdflatex main -> bibtex main -> pdflatex main -> pdflatex main
Nota: sagej usa natbib + BibTeX (SageH.bst), no biblatex/biber.
Citas: \citep{llave}  \citet{llave}

## Pendientes
- Reemplazar cada \relleno{...} con tu texto, en ingles.
- Confirmar en las Submission guidelines de la revista: plantilla/clase, estilo de referencias, limite de palabras, declaraciones.
- Subir main.pdf (anonimo), portada aparte y los .bib/.bst si la revista los pide.
