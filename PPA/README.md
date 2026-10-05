# Gobernanza y prevención de la corrupción en el Perú

Proyecto de artículo académico preparado para una posible presentación a *Public Policy and Administration* (SAGE). El repositorio contiene las fuentes LaTeX, versiones de trabajo para envío, notas por bloques, materiales de referencia y los productos de compilación.

## Estado actual

El manuscrito fuente es `files/manuscript/main.tex`. Mantiene `\author{}` vacío y está anonimizado en su fuente. El título, el cuerpo y los encabezados están en español; el abstract y las keywords permanecen en inglés, conforme a la última instrucción de trabajo. Esto **no coincide con el requisito de idioma inglés que se había indicado inicialmente para la revista**. Confirmar con la revista si aceptaría español o traducir el cuerpo antes de enviar.

El conteo con `texcount` fue de 6.646 palabras (6.473 en texto y 173 en encabezados), sin referencias. El conteo puede variar según las reglas de la revista y no debe tomarse como su conteo oficial.

La última compilación local de las fuentes se encuentra en `files/build/generated/main.pdf` y `files/build/generated/portada.pdf`. La compilación comprobó que las citas de `main.tex` se resuelven mediante BibTeX y Sage Harvard. `sagej.cls` y `SageH.bst` se conservaron sin modificaciones.

## Estructura

```text
README.md
files/
	.gitignore
	manuscript/                 Fuentes LaTeX y archivos necesarios para compilar
		main.tex                  Manuscrito anónimo
		portada.tex               Portada separada con autores y declaraciones
		referencias.bib           Base de referencias
		sagej.cls                 Clase SAGE, sin modificar
		SageH.bst                  Estilo Sage Harvard, sin modificar
	submission/
		versions-unverified/      DOCX/PDF anteriores, conservados para cotejo
			Main_Manuscript.docx
			Main_Manuscript.pdf
			Title_Page.docx
			Title_Page.pdf
	notes/                      Bloques de contenido e instrucciones antiguas
		bloque1.md
		bloque2.md
		bloque3.md
		bloque1-root-placeholder.md  Copia vacía de 0 bytes, conservada
		LEEME.md                  Guía previa, conservada como historial
	reference/
		examples/draft_Proof_hi.pdf
		other-course-material/VIDEOS-EXPOSICIONES-ING-SISTEMAS.txt
		sage-assets/SAGE_Logo.eps, SAGE_Logo.pdf
		sage-template-demo/A_demonstration_of_the_LaTeX2e_class_file_for_SAGE_Publications.zip
		sage-template-demo/A_demonstration_of_the_LaTeX2e_class_file_for_SAGE_Publications/
			readme.txt, SageH.bst, SageV.bst, Sage_LaTeX_Guidelines.tex
			SAGE_Logo.eps, SAGE_Logo.pdf, sagej.cls
		scholarone/ScholarOne Manuscripts.pdf
	build/
		generated/
			main.pdf, main.aux, main.bbl, main.blg, main.fdb_latexmk
			main.fls, main.log, main.out
			portada.pdf, portada.aux, portada.fdb_latexmk, portada.fls, portada.log
		legacy/
			main.aux, main.bbl, main.blg, main.log, main.out
			portada.bbl, portada.blg, portada.synctex.gz
```

`files/notes/bloque1-root-placeholder.md` conserva el archivo vacío de 0 bytes que estaba en la raíz. La versión con contenido es `files/notes/bloque1.md`. `files/notes/LEEME.md` se conserva como guía antigua; este README es la documentación vigente.

## Evolución del proyecto

1. Se partió de la plantilla demostrativa SAGE y de la clase `sagej.cls`, con el estilo `SageH.bst` y citas gestionadas con `natbib` y BibTeX. Se decidió mantener el manuscrito anónimo y presentar los datos de autoría en una portada separada.
2. Se definieron el tema, el título y una estructura inicial con introducción, revisión de literatura/marco analítico, metodología, hallazgos, discusión y conclusiones. Se acordó no modificar los archivos oficiales de clase y estilo.
3. Se incorporó `bloque1.md`: resumen en inglés; contexto y problema; objetivo y pregunta; contribución; revisión de literatura; tres dimensiones del marco analítico; diseño y procedimiento de revisión documental; y limitaciones metodológicas.
4. Se incorporó `bloque2.md` en Hallazgos: responsabilidades y coordinación institucional, políticas de integridad, mecanismos de prevención y control, e implementación desigual y brechas. El texto distingue documentos normativos de evidencia de control y advierte que el corpus no permite demostrar efectividad causal.
5. Se incorporó `bloque3.md` en Discusión y Conclusiones: interpretación según las tres dimensiones, implicaciones de política pública, tensiones, recomendaciones y agenda futura. Las conclusiones advierten que los estudios locales incluidos no se pueden generalizar automáticamente.
6. Se añadieron citas Sage Harvard y se ajustaron metadatos bibliográficos contrastados para Eloy Munive Pariona (2022) y *OECD Justice Review of Peru* (2024). Las referencias de autores, títulos, URL/DOI y claves deben seguir cotejándose con las fuentes originales antes de someter el artículo.
7. Se completó la portada con cinco autores, afiliación común de la Universidad Nacional de San Agustín de Arequipa, datos de correspondencia, agradecimiento al profesor y declaraciones de ética, consentimientos, conflictos, financiamiento y disponibilidad de datos.
8. Durante la preparación en ScholarOne se observó que el portal exige añadir las keywords de una en una y solicita ORCID para quien presenta el manuscrito. También rechazó los PDF cargados como Main Document y Title Page con el mensaje de tipo de archivo no permitido. La pantalla de carga del portal es la autoridad para determinar extensiones admitidas.
9. Se reorganizaron las fuentes, materiales, versiones de envío y auxiliares en las carpetas descritas arriba. La compilación pasó a `latexmk` con salida separada para no ensuciar la carpeta de fuentes.

## Compilar

Requiere una distribución LaTeX con `pdflatex`, BibTeX y `latexmk`:

```sh
cd files/manuscript
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=../build/generated main.tex
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=../build/generated portada.tex
```

`latexmk` ejecuta BibTeX para `main.tex` cuando detecta cambios en las citas o en `referencias.bib`. Los auxiliares y PDFs resultantes quedan en `files/build/generated/`; esa carpeta está excluida del control de versiones. No editar `sagej.cls` ni `SageH.bst`.

## Diagnóstico antes del envío

Los archivos de `files/submission/versions-unverified/` se conservaron como candidatos anteriores, no como paquete final garantizado. La extracción de texto no encontró nombres de autores en `Main_Manuscript.docx` ni en el PDF. Además, el texto extraído del PDF coincide con el de `files/build/generated/main.pdf`; este último se compiló desde la fuente reorganizada. El PDF fuente-compilado no muestra autores. La portada separada sí contiene los cinco nombres, como corresponde.

El portal ScholarOne rechazó los PDF al cargarlos como Main Document y Title Page, mostrando “The file type is not allowed”. Por tanto, debe usarse el DOCX como Main Document solo tras cotejarlo con `main.tex` y confirmar que siga anónimo; subir `Title_Page.docx` como Title Page. No cambiar extensiones manualmente: el tipo real debe ser el permitido por el portal.

Hay una discrepancia de alcance bibliográfico que requiere resolver: el abstract y la subsección metodológica describen un corpus de cinco documentos, mientras que los hallazgos usan además el Plan PCM 2018, la Directiva PCM 2026 y el informe de Contraloría 2020; la discusión y conclusiones citan también dos estudios académicos adicionales. Actualizar el abstract, la descripción del corpus y los criterios metodológicos para que representen el corpus real, o limitar las secciones a las cinco fuentes declaradas.

Pendientes que bloquean o requieren confirmación antes de enviar:

- Resolver la discrepancia de idioma: el requisito comunicado para la revista fue inglés, pero el cuerpo actual está en español. Abstract y keywords están en inglés.
- Cotejar `Main_Manuscript.docx` con el `main.tex` actual y confirmar anonimización y versión antes de cargarlo como Main Document. ScholarOne rechazó PDF en la pantalla observada; la extensión aceptada debe confirmarse en sus instrucciones de carga. No basta con cambiar la extensión de un archivo.
- Resolver la discrepancia entre las cinco fuentes declaradas en resumen/metodología y las fuentes adicionales citadas en hallazgos, discusión y conclusiones.
- Completar/vincular el ORCID del autor que someterá el manuscrito (ScholarOne lo marcó como obligatorio) y registrar allí a los cinco autores en el orden de la portada. En la captura de autores solo figuraba el remitente; confirmar que se hayan agregado los demás.
- Añadir las seis keywords individualmente en el portal (mínimo requerido: 3; máximo: 6) y hacerlas coincidir con el manuscrito.
- Confirmar con todos los autores que las declaraciones de conflicto de interés, financiamiento, ética y disponibilidad de datos son verdaderas; validar también el agradecimiento al profesor.
- Revisar el registro de envío y los datos bibliográficos. El PDF local `ScholarOne Manuscripts.pdf` se conserva como referencia del flujo del portal; no usarlo como prueba de envío sin verificar que incluya un número de manuscrito y una confirmación efectiva.
- Verificar los datos bibliográficos que en `referencias.bib` siguen marcados como pendientes, en particular `ramos2025politicas`, `liderazgo2025corrupcion` y `penamancillas2022integridad`. Confirmar también que todas las citas y referencias correspondan exactamente.
- El borrador de cover letter se redactó en la conversación, pero no está guardado como archivo del proyecto. Crear y revisar el archivo final para ScholarOne.

La portada fuente está en `files/manuscript/portada.tex`; contiene nombres y datos identificadores, por lo que debe cargarse únicamente como Title Page, nunca como Main Document. Los archivos en `versions-unverified/` se preservaron para cotejo y no se sobrescribieron. Los PDFs más recientes de comprobación se generan en `files/build/generated/` y no son la versión autorizada para envío mientras el idioma y las discrepancias del corpus sigan pendientes.
