# Minería de procesos, ERP, ROI y Kardex: ¿mejora garantizada del desempeño organizacional?

> **DOCUMENTO DE TRABAJO — BORRADOR PROVISIONAL.** No es una versión final. Todo el contenido está sujeto a revisión según se lean las fuentes.
>
> **Marcadores:** **[PENDIENTE]** falta desarrollar · **[BUSCAR FUENTE]** falta evidencia · **[VERIFICAR]** comprobar contra la fuente · **[REVISAR TESIS]** la evidencia podría modificar la tesis · **[POSIBLE EJEMPLO]** ejemplo, no evidencia · **[DISCUTIR]** requiere análisis · **[CONECTAR]** relacionar con otro concepto o argumento.
>
> **Convención de citas provisional:** se usa `[F x.y]` para remitir a la numeración de la lista de fuentes del final. Las cifras tomadas de las fichas deben **[VERIFICAR]** contra el texto original antes de citarse.

---

## 1. Introducción

### 1.1. Contextualización y delimitación del tema

Las organizaciones registran cada vez más sus operaciones en sistemas de información como los ERP (*Enterprise Resource Planning*). Estos sistemas dejan huellas digitales (compras, aprobaciones, ingresos y salidas de almacén) que pueden analizarse para comprender cómo se ejecutan realmente los procesos. La minería de procesos aprovecha esas huellas, conocidas como registros de eventos (*event logs*), para reconstruir el proceso real, detectar desviaciones e identificar cuellos de botella.

El ensayo se delimita a la relación entre cuatro elementos: la minería de procesos, los sistemas ERP, el control de inventarios (con el Kardex como ejemplo concreto) y el ROI como criterio de evaluación económica. A ellos se suma la dimensión organizacional y humana. **[PENDIENTE]** Precisar si se acotará a un sector (por ejemplo, manufactura, minería o servicios públicos) o se mantendrá un enfoque general.

### 1.2. Antecedentes y relevancia

La literatura reciente sugiere que existe una brecha entre *detectar* un problema y *resolverlo*. Una revisión sistemática identifica siete desafíos que dificultan convertir los hallazgos de la minería de procesos en mejoras efectivas, entre ellos la falta de apoyo de la alta dirección y la resistencia al cambio [F 1.1]. En paralelo, la investigación sobre ERP muestra resultados mixtos entre la inversión y el desempeño organizacional [F 3.1].

El tema es relevante porque las organizaciones que invierten en estas tecnologías esperan resultados, y esas expectativas pueden ser mayores que lo que la evidencia respalda. **[BUSCAR FUENTE]** Datos sobre adopción de minería de procesos y ERP en el contexto peruano o latinoamericano, si se quiere justificar la relevancia local.

### 1.3. Problema o cuestión que se plantea

Si la minería de procesos permite identificar ineficiencias con precisión, cabría esperar que su implementación mejore el desempeño. Sin embargo, esa expectativa supone que los datos son adecuados, que la organización puede actuar sobre lo detectado y que el resultado compensa la inversión.

**Pregunta central (provisional):** ¿La implementación de minería de procesos garantiza una mejora del desempeño organizacional, o su impacto depende de otros factores del sistema empresarial?

### 1.4. Objetivo del ensayo

Analizar, a partir de literatura académica, en qué medida el impacto de la minería de procesos depende de la calidad de los datos provenientes de sistemas como el ERP, de factores organizacionales y humanos, y de la evaluación económica de las mejoras. **[PENDIENTE]** Ajustar la redacción cuando se definan los argumentos finales.

### 1.5. Tesis o idea central

**Tesis provisional:** La implementación de la minería de procesos, por sí sola, no garantiza una mejora integral del desempeño organizacional, ya que sus resultados dependen de la interacción de múltiples factores: los recursos disponibles, las capacidades organizacionales, el contexto operativo, la gestión de los procesos, las condiciones del trabajador y el nivel de madurez tecnológica. Los sistemas ERP y el Kardex pueden aportar la infraestructura y los datos necesarios para el análisis, mientras que el ROI permite evaluar el impacto económico de las mejoras.

**[REVISAR TESIS]** Las fichas de fuentes sugieren una formulación posible: la minería de procesos como condición *habilitante pero no suficiente*. Esta versión reconoce de forma explícita que la herramienta sí puede identificar desviaciones objetivas. Decidir si se adopta tras leer las fuentes.

---

## 2. Desarrollo

### 2.1. Marco conceptual

Los cuatro conceptos se presentan como eslabones de una misma cadena, no como definiciones aisladas:

```text
ERP
↓ generación y centralización de datos
event logs
↓ extracción y preparación
minería de procesos
↓ identificación de desviaciones / cuellos de botella
decisiones y posibles mejoras (requieren capacidad organizacional)
↓
resultados organizacionales
↓
evaluación mediante ROI
```

**[CONECTAR]** Cada flecha es un punto donde la cadena puede romperse. Los tres argumentos del ensayo se apoyan en tres de esas rupturas posibles: datos deficientes (flecha ERP → *event logs*), incapacidad de actuar (decisiones → resultados) y rentabilidad no demostrada (resultados → ROI).

#### 2.1.1. Minería de procesos

Conjunto de técnicas que analizan registros de eventos para descubrir, verificar y mejorar procesos tal como ocurren en la práctica. Su valor diagnóstico consiste en contrastar el proceso *real* con el proceso *supuesto*. **[BUSCAR FUENTE]** Definición de un autor de referencia del campo para citarla de forma directa.

Punto clave para el ensayo: la minería de procesos es una herramienta de **diagnóstico**. Que sea una condición para mejorar no significa que garantice la mejora.

#### 2.1.2. Sistemas ERP

Sistemas que integran procesos de distintas áreas (compras, ventas, inventario, finanzas) sobre una base de datos común. En este ensayo interesan en dos papeles: como **fuente de datos** para la minería de procesos y como **objeto de implementación** que ya está condicionado por recursos, capacitación y cambio organizacional [F 3.2].

**[DISCUTIR]** Si el ERP está mal implementado o es poco usado, los datos que alimentan la minería de procesos también lo estarán.

#### 2.1.3. Retorno de la inversión (ROI)

Indicador que relaciona el beneficio económico obtenido con el costo de la inversión. En el ensayo sirve para distinguir entre "mejorar un proceso" y "justificar económicamente la inversión". **[BUSCAR FUENTE]** Referencia sobre cómo se calcula el ROI en proyectos de tecnologías de la información y sus limitaciones (por ejemplo, beneficios intangibles o costos ocultos de implementación).

**[VERIFICAR]** Si alguna de las fuentes reunidas calcula un ROI explícito para minería de procesos. En la lista actual no se identifica ninguna que lo haga directamente.

#### 2.1.4. Kardex

Registro de entradas, salidas y saldos de existencias, que permite la trazabilidad de los movimientos de inventario. En la literatura internacional el término más habitual es *inventory control systems* [F 5.1], por lo que conviene indicar esa equivalencia al introducir el concepto.

En el ensayo funciona como **ejemplo concreto** de registro operativo del que puede extraerse un *event log* (cada movimiento tiene actividad, fecha y responsable). **[CONECTAR]** Con el Argumento 1: un Kardex mal alimentado produce una imagen deformada del proceso de almacén.

**[POSIBLE EJEMPLO]** *Ejemplo hipotético:* una empresa registra en su ERP cada solicitud de material, su aprobación y la salida del almacén. La minería de procesos revela que muchas solicitudes se aprueban fuera de orden. Pero si parte de las salidas se anotan después en el Kardex (o no se anotan), el análisis ve una versión incompleta del proceso. Este ejemplo no constituye evidencia empírica.

---

### 2.2. Argumento 1 — La minería de procesos depende de la calidad del sistema de información

**Idea a defender:** La capacidad de la minería de procesos para generar mejoras está condicionada por la calidad, disponibilidad y representatividad de los datos que proporcionan sistemas como los ERP.

Una posible línea de razonamiento es la siguiente. La minería de procesos solo ve lo que queda registrado. Si los datos están incompletos, son ruidosos o están mal extraídos, el modelo resultante puede representar de forma inadecuada el proceso real. La revisión de preprocesamiento de *event logs* señala que las técnicas de preparación tienen alto impacto en el desempeño de las tareas de minería de procesos y que el ruido y la incompletitud son problemas frecuentes [F 2.1]. Un preprint más reciente sostiene que la calidad de los datos es uno de los desafíos más apremiantes y cataloga 29 desafíos en la generación de *event logs* [F 2.2] **[VERIFICAR]**.

Desde el lado del ERP, el estudio con modelado de ecuaciones estructurales reporta que la calidad de datos e información predice significativamente el desempeño organizacional [F 3.1] **[VERIFICAR]**. En inventarios, la literatura asocia los sistemas de control con datos más exactos, aunque el efecto depende de la calidad del registro, la integración y el uso efectivo del sistema [F 5.1, F 5.2].

Quedan abiertas dos cuestiones:

- Las actividades manuales o informales pueden quedar fuera del registro digital. **[BUSCAR FUENTE]** Evidencia específica sobre actividades no capturadas en *event logs* derivados de ERP.
- Una ruta de razonamiento posible es la ausencia de relación directa entre "tener un ERP" y "tener datos aptos para minería". **[DISCUTIR]**

**[CONECTAR]** Este argumento prepara el Argumento 2: la calidad de los datos depende también de cómo los trabajadores los registran.

---

### 2.3. Argumento 2 — La mejora tecnológica depende de factores organizacionales y humanos

**Idea a defender:** El desempeño organizacional no depende exclusivamente de la tecnología, sino de la interacción entre tecnología, procesos, capacidades organizacionales y trabajadores.

Identificar un cuello de botella no implica que la organización pueda resolverlo de inmediato. La revisión sobre la brecha entre *insights* y mejora agrupa los obstáculos en compromiso organizacional, *expertise* y otros factores, y menciona el apoyo insuficiente de la dirección y la resistencia al cambio [F 1.1]. El modelo de madurez propuesto en otra fuente reúne gestión de proyectos, apoyo directivo, calidad de datos, recursos, *expertise*, gestión del cambio y capacitación como factores de éxito [F 1.2] **[VERIFICAR]** (la ficha indica cinco factores y 23 elementos).

La literatura ERP converge en lo mismo: el éxito depende de la preparación organizacional, el apoyo de la alta dirección y la capacitación; los obstáculos incluyen resistencia, costos, integración de datos y capacitación insuficiente [F 3.3]. Y el ajuste organizacional y la reingeniería de procesos influyen en los beneficios obtenidos del ERP [F 3.1].

**Dimensión humana (explorar con cautela).** Esta sección incorpora a los trabajadores como parte del sistema y no como un tema separado. Líneas posibles:

- **Capacitación y adaptación:** cómo influye la formación en la recuperación del desempeño tras una implementación. **[BUSCAR FUENTE]** Estudios sobre ERP que describan una intensificación inicial del trabajo seguida de recuperación con capacitación más amplia. Esta idea figura en el plan del ensayo, pero la lista actual no contiene una fuente que la respalde.
- **Resistencia al cambio y cultura:** por ejemplo, la dependencia de aprobaciones en papel. **[BUSCAR FUENTE]** Caso de implementación ERP analizado con minería de procesos que reporte problemas técnicos, de migración de datos y culturales. **[VERIFICAR]** Hasta localizarlo, no debe afirmarse como caso real.
- **Uso de los datos:** una implementación orientada solo a maximizar productividad podría producir efectos distintos según cómo se usen los datos (apoyo a la mejora o vigilancia) y según las condiciones organizacionales. Se trata de una **hipótesis de trabajo**, no de un hallazgo.

**[BUSCAR FUENTE]** No se localizó evidencia revisada por pares que demuestre directamente que la minería de procesos, usada para monitorear a los trabajadores, produzca intensificación laboral o afecte la autonomía. Términos de búsqueda sugeridos: `"process mining" AND "employee monitoring"`, `"workplace surveillance" AND "digitalization"`, `"algorithmic management" AND "work intensification"`, `"ERP implementation" AND "employee resistance"`, `"ERP implementation" AND "work stress"`.

**[REVISAR TESIS]** Si la búsqueda no encuentra respaldo empírico, esta parte debería presentarse como línea de discusión y no como argumento probado.

---

### 2.4. Argumento 3 — Identificar mejoras no equivale a demostrar rentabilidad

**Idea a defender:** Una mejora de proceso no demuestra por sí misma que la inversión tecnológica haya sido económicamente conveniente. El desempeño tiene varias dimensiones: operativa, organizacional, humana y económica.

Secuencia lógica:

```text
minería de procesos → identifica oportunidad
→ la organización implementa un cambio
→ se producen resultados
→ el ROI evalúa económicamente la inversión
```

El caso de mantenimiento minero ilustra el punto. La minería de procesos permitió detectar cuellos de botella y cuantificar una pérdida de 23 800 horas operativas anuales y un costo de no producción cercano a 1,12 millones de USD al año **[VERIFICAR]**. Pero esas cifras describen el *costo del problema diagnosticado*; no prueban que la organización haya capturado ese ahorro, que depende de implementar estrategias de mantenimiento efectivas [F 4.2]. **[DISCUTIR]** Esta diferencia entre "costo del problema" y "beneficio obtenido" es una de las ideas más útiles para sostener el argumento.

En la literatura ERP, la relación entre inversión y desempeño arroja resultados mixtos [F 3.1], y una revisión señala costos altos entre los obstáculos [F 3.3].

**[BUSCAR FUENTE]** Evidencia que calcule costos totales de proyectos de minería de procesos (licencias, extracción de datos, capacitación, tiempo del personal) frente a beneficios.

**[CONECTAR]** Con 2.1.3: el ROI solo es útil si los beneficios y costos se miden con criterios explícitos. **[PENDIENTE]**

---

### 2.5. Contraargumento y refutación

**Contraargumento.** La evidencia demuestra que la minería de procesos sí puede producir mejoras objetivas. Es una posición defendible, y la literatura ofrece casos que la respaldan:

- En un proceso de verificación de seguridad del gobierno canadiense, la minería de procesos identificó escenarios excepcionales, bucles que consumían tiempo y problemas de asignación de recursos. Tras intervenciones basadas en esos hallazgos, el tiempo de *briefing* bajó de unos 7 días a 46 horas y el tiempo total, de unos 31 a 26 días [F 4.1] **[VERIFICAR]**. Es un preprint con análisis antes y después.
- En el caso de mantenimiento minero, la técnica permitió representar el proceso y detectar ineficiencias con relevancia económica potencial [F 4.2].
- Revisiones sobre ERP e inventarios asocian estos sistemas con mejoras de eficiencia y exactitud de datos [F 3.3, F 5.1].

**Refutación.** Parte del contraargumento es válida: la minería de procesos puede ser eficaz como herramienta de diagnóstico y, cuando el diagnóstico se conecta con intervenciones concretas, puede asociarse con reducciones de tiempo. Aun así, esto no refuta la tesis, por tres razones provisionales:

1. La capacidad de **identificar** problemas no implica que la organización pueda **resolverlos** [F 1.1, F 1.2].
2. Las mejoras observadas son **locales** (un proceso, un caso) y no equivalen a desempeño organizacional integral. **[DISCUTIR]**
3. Una reducción de tiempos no demuestra que los beneficios compensen los costos y efectos derivados de la implementación. **[BUSCAR FUENTE]** ROI explícito.

**[REVISAR TESIS]** Los casos exitosos podrían ser precisamente aquellos en que se cumplieron las condiciones organizacionales señaladas en los Argumentos 1 y 2, lo que reforzaría la tesis. Pero también podría haber sesgo de publicación (se publican más los éxitos). **[VERIFICAR]** Esto requiere argumentación cuidadosa, no una afirmación directa.

---

### 2.6. Discusión y relación entre los conceptos

Los cuatro conceptos forman un sistema, no un conjunto de herramientas independientes:

| Nivel de análisis | Pregunta clave | Evidencia principal (provisional) |
|---|---|---|
| Identificar ineficiencia | ¿La minería de procesos detecta cuellos de botella? | Sí, en los casos de mantenimiento minero y servicio público [F 4.1, F 4.2] |
| Mejorar un proceso | ¿El hallazgo se convierte en una intervención efectiva? | Depende de gestión del cambio, apoyo directivo, *expertise* y recursos [F 1.1, F 1.2] |
| Mejorar el desempeño organizacional | ¿La mejora local se traduce en desempeño global? | Depende del ajuste organizacional, la calidad de datos, el contexto y el tiempo de uso [F 3.1] |
| Obtener ROI positivo | ¿Existe retorno económico verificable? | Puede haber ahorros, pero no es automático ni equivale a mejora integral |

Líneas de discusión abiertas:

- **Orientación a metas.** Una revisión sobre minería de procesos orientada a objetivos [F 1.3] sugiere que el valor del análisis depende de su vínculo con metas del negocio. Sin ese vínculo, el diagnóstico puede no tener impacto. **[CONECTAR]** Con el Argumento 3.
- **Madurez.** ¿La "madurez tecnológica" de la tesis equivale a la madurez de minería de procesos descrita en [F 1.2]? **[PENDIENTE]**
- **Implicaciones prácticas.** Si la herramienta es necesaria pero no suficiente, las organizaciones deberían evaluar su preparación (datos, capacitación, apoyo directivo, criterios de ROI) antes de invertir. **[DISCUTIR]** Evitar convertir esto en una recomendación categórica.
- **Tensión no resuelta.** ¿Puede una organización con baja madurez beneficiarse igualmente de un proyecto piloto pequeño? **[BUSCAR FUENTE]**

---

## 3. Conclusión

> **[PENDIENTE]** Esta sección debe redactarse al final, cuando las fuentes hayan sido leídas y la tesis esté confirmada o ajustada. Lo siguiente son solo líneas posibles.

### 3.1. Síntesis de los argumentos principales

Líneas posibles: (1) la calidad y representatividad de los datos condicionan la validez del diagnóstico; (2) los factores organizacionales y humanos condicionan que el diagnóstico se convierta en mejora; (3) la mejora de un proceso no equivale a rentabilidad demostrada.

### 3.2. Respuesta a la tesis

**[REVISAR TESIS]** Dependiendo de la lectura de las fuentes, la respuesta podría mantenerse como "no garantiza" o matizarse como "condición habilitante pero no suficiente". No cerrar hasta contrastar la evidencia.

### 3.3. Reflexión final

Líneas posibles: la distancia entre diagnosticar y transformar; el papel de los trabajadores en que una mejora tecnológica se sostenga; la necesidad de evaluar el retorno con criterios explícitos; límites del propio ensayo (fuentes en parte preprints, evidencia humana limitada). **[PENDIENTE]**

---

## 4. Referencias bibliográficas

> Solo fuentes proporcionadas. Falta completar autores donde no constan en las fichas. **No añadir datos que no se hayan verificado.** Convertir a entradas de `referencias.bib` al revisar cada una.

**Bloque 1 — Minería de procesos y mejora organizacional**

- **[F 1.1]** *From Process Mining Insights to Process Improvement: All Talk and No Action?* Springer, 2023. https://doi.org/10.1007/978-3-031-46846-9_15
- **[F 1.2]** *Improving Process Mining Maturity – From Intentions to Actions*. *Business & Information Systems Engineering*, 2024. https://doi.org/10.1007/s12599-024-00882-7
- **[F 1.3]** Ghasemi, M., & Amyot, D. (2020). From event logs to goals: A systematic literature review of goal-oriented process mining. *Requirements Engineering, 25*, 67–93. https://doi.org/10.1007/s00766-018-00308-3

**Bloque 2 — Calidad de datos y event logs**

- **[F 2.1]** Marin-Castro, H. M., & Tello-Leal, E. (2021). Event log preprocessing for process mining: A review. *Applied Sciences, 11*(22), 10556. https://doi.org/10.3390/app112210556
- **[F 2.2]** *Data-Related Challenges and Requirements for Event Log Generation in Process Mining: A Systematic Literature Review* (2026). arXiv:2609.04211. https://doi.org/10.48550/arXiv.2609.04211 *(preprint)*

**Bloque 3 — ERP, desempeño y factores organizacionales**

- **[F 3.1]** *The Impact of ERP Systems on Organizational Performance: The Role of Antecedents and Moderators*. *International Journal of Enterprise Information Systems*, 2024. https://doi.org/10.4018/IJEIS.329960
- **[F 3.2]** Ali, M., & Miller, L. (2017). ERP system implementation in large enterprises: A systematic literature review. *Journal of Enterprise Information Management, 30*(4), 666–692. https://doi.org/10.1108/JEIM-07-2014-0071
- **[F 3.3]** Talo, M. C., & Emanuel, A. W. R. (2025). Systematic review of enterprise resource planning (ERP) system implementation in organizations: Challenges and successes to company performance. *Bitnet: Jurnal Pendidikan Teknologi Informasi, 10*(2), 1–11. https://doi.org/10.33084/bitnet.v10i2.9603

**Bloque 4 — Evidencia a favor de mejoras demostrables**

- **[F 4.1]** *Using Process Mining to Improve Digital Service Delivery* (2024). arXiv:2409.05869. https://doi.org/10.48550/arXiv.2409.05869 *(preprint)*
- **[F 4.2]** *Towards the Application of Process Mining in the Mining Industry: An LHD Maintenance Process Optimization Case Study*. *Sustainability, 15*(10), 7974, 2023. https://www.mdpi.com/2071-1050/15/10/7974

**Bloque 5 — Kardex, inventarios y ERP**

- **[F 5.1]** *An assessment of the effect of inventory control systems on performance of mining firms in Zimbabwe*. *Cogent Business & Management*, 2024. https://doi.org/10.1080/23311975.2023.2298535
- **[F 5.2]** *Enhancing Inventory Accuracy and Operational Performance with ERP*. *Sinergi International Journal of Logistics, 2*(2), 1–14, 2024. https://doi.org/10.61194/sijl.v2i2.622

**Vacío pendiente:** fuentes empíricas sobre factores humanos (monitoreo, autonomía, carga de trabajo) en implementaciones de ERP y minería de procesos. Ver términos de búsqueda en 2.3.