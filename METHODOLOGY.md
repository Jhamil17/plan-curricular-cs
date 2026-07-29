## 7. Sistema de evaluación

Tres perfiles. Cada asignatura declara el suyo en su cabecera.

### 7.1 Perfil TEÓRICO

Aplica a: MAT-*, TEO-301, TEO-302, TEO-303, ALG-401, ALG-402, ALG-801, IAP-601, LEN-701, SEG-701.

| Instrumento | Peso | Descripción |
|---|---|---|
| Prueba de Dominio | 30% | Demostración o construcción formal terminal |
| Evaluación Parcial 1 (sem. 7) | 15% | Escrita, sin material |
| Evaluación Parcial 2 (sem. 14) | 15% | Escrita, sin material |
| Examen Final integrador (sem. 16) | 20% | Acumulativo sobre todo el ciclo |
| Problem sets semanales | 15% | 12 entregas; se descartan las 2 peores |
| Defensa en pizarra | 5% | 3 demostraciones sorteadas, en vivo, sin apuntes |

### 7.2 Perfil SISTEMAS

Aplica a: SIS-*, LEN-201, LEN-501, LEN-502, ALG-201, ALG-403, IAP-602, IAP-603, IAP-801, SEG-702, TEO-401, TEO-601, MAT-601.

| Instrumento | Peso | Descripción |
|---|---|---|
| Prueba de Dominio | 45% | Sistema construido, evaluado bajo inyección de fallos |
| Laboratorios | 20% | 5–7 labs con criterio binario de aceptación |
| Evaluación Parcial (sem. 8) | 12% | Escrita + traza a mano |
| Examen Final (sem. 16) | 13% | Escrita + depuración bajo presión |
| Code review cruzado | 10% | Revisión adversarial de la solución de un par |

### 7.3 Perfil INVESTIGACIÓN

Aplica a: INV-801, INV-802, INT-*.

| Instrumento | Peso |
|---|---|
| Artefacto entregado (paper / tesis / sistema integrador) | 60% |
| Defensa oral | 25% |
| Bitácora de investigación fechada, con hipótesis descartadas | 15% |

### 7.4 Escala

`20` reservado. `18–19` dominio excepcional. `16–17` dominio sólido. `14–15` aprobado. `<14` desaprobado. Sin curva. Sin redondeo al alza.

### 7.5 Adaptación para el estudiante sin institución

El plan asume evaluadores. Un autodidacta no los tiene, y fingir que sí vacía el sistema de evaluación. Sustituciones aceptables, en orden de preferencia:

| Instrumento original | Sustituto autodidacta | Qué se pierde |
|---|---|---|
| Evaluación escrita sin material | Exámenes finales públicos del curso fuente (MIT OCW, Berkeley, CMU publican con solucionario), cronometrados, corregidos contra rúbrica antes de ver la solución | Nada sustancial si se respeta el cronómetro |
| Defensa en pizarra | Grabación en video de la demostración sin apuntes, revisada 48 h después por uno mismo con rúbrica escrita | Presión de interrogatorio en vivo. Es una pérdida real. |
| Code review cruzado | Revisión adversarial por un modelo de lenguaje bajo el protocolo de §16, más publicación del código en un repositorio público | Juicio de un par con contexto |
| Defensa oral de integrador | Presentación grabada de 20 min + escritura de las tres objeciones más fuertes que un evaluador plantearía, con respuesta a cada una | Objeciones que no se anticipan solo |
| Paper con revisión por pares | Preprint en arXiv + solicitud explícita de crítica en la comunidad del área (§23) | Revisión formal. Sustituible parcialmente. |
| Comité de tesis | Tres lectores externos comprometidos por escrito antes de empezar la tesis, no después | Autoridad institucional |

**Regla dura de la sustitución.** El sustituto se fija **antes** de empezar la asignatura, no cuando llega el momento de evaluarse. Elegir el instrumento de evaluación después de conocer el propio nivel de preparación es la forma más común de vaciar un plan autodidacta sin notarlo.

---

# PARTE II — RÉGIMEN METODOLÓGICO

El programa trata la metodología de estudio como componente curricular, no como consejo. Los mecanismos de §8 son obligatorios y su cumplimiento se audita en la bitácora (§7.3).

**Estructura de esta parte.** §8 da el nivel conductual: qué intervenciones funcionan y cómo se instrumentan. §9–§11 dan el nivel de mecanismo: por qué funcionan, en términos de la arquitectura neural que las implementa. §12–§16 son operativos. §17 declara qué no hacer. §18 cubre el reingreso tras interrupción.

**Convención de calidad de evidencia.** Cada afirmación de §8–§11 lleva un grado:

| Grado | Significado |
|---|---|
| `■■■` | Efecto replicado en humanos, con meta-análisis o múltiples estudios independientes convergentes. Se puede usar como base de decisión. |
| `■■□` | Efecto real pero con menos replicación, tamaño de efecto discutido, o condiciones de frontera poco claras. Se usa con margen. |
| `■□□` | Mecanismo plausible extrapolado de modelos animales, hallazgo único, o construcción divulgativa útil pero no establecida. **No se usa para decidir nada; se declara porque circula y conviene saber qué estatus tiene.** |

Esta graduación es la diferencia principal entre esta versión y la 2026.1, que presentaba todo su aparato metodológico con el mismo nivel de confianza.

---

## 8. Mecanismos de aprendizaje e instrumentación

| Mecanismo | Ev. | Hallazgo central | Instrumentación obligatoria |
|---|---|---|---|
| **Práctica de recuperación** | `■■■` | Recuperar desde memoria retiene más que releer, aun cuando releer *se siente* más eficaz (Roediger & Karpicke, 2006; meta-análisis de Adesope et al., 2017: g ≈ 0.50 sobre relectura) | Ninguna sesión abre con lectura. Abre con reconstrucción en hoja en blanco de lo último visto. |
| **Espaciado** | `■■■` | El intervalo óptimo escala con el horizonte de retención objetivo; para retener un año, el intervalo útil es de semanas, no de días (Cepeda et al., 2006) | FSRS calcula el intervalo. Prohibidos los intervalos fijos y el repaso previo al examen. |
| **Intercalado** | `■■■` | Mezclar tipos de problema deprime el rendimiento durante la práctica y lo eleva en la evaluación (Rohrer & Taylor, 2007). El efecto es mayor cuando los tipos son confundibles entre sí | Bloque sabatino con problemas sin etiqueta de origen (§13.3). La selección de dominios prioriza pares confundibles, no distantes. |
| **Dificultades deseables** | `■■■` | Las condiciones que hacen la práctica más lenta y con más errores suelen mejorar la retención a largo plazo (Bjork & Bjork, 2011) | Regla de 25 minutos sin material antes de abrir cualquier fuente. |
| **Autoexplicación** | `■■■` | Explicarse cada paso de una prueba supera a leerla; el efecto viene de detectar los huecos, no de verbalizar (Chi et al., 1989) | Al leer una demostración: tapar la línea siguiente, predecirla, destapar, comparar. |
| **Ejemplos resueltos con fading** | `■■■` | El ejemplo resuelto supera al problema abierto para material nuevo; la ventaja **se invierte** con la experticia (Sweller & Cooper, 1985; Kalyuga et al., 2003) | Cada técnica nueva: 1 ejemplo completo → 2 problemas de completación → problemas abiertos. El fading es obligatorio. |
| **Efecto de generación** | `■■■` | Intentar producir la respuesta antes de verla mejora la codificación **aun cuando el intento falla** (Slamecka & Graf, 1978; Kornell et al., 2009) | Derivar antes de leer la derivación. Siempre. |
| **Hipercorrección** | `■■■` | Los errores cometidos con alta confianza son los que mejor se corrigen cuando llega el feedback (Butterfield & Metcalfe, 2001) | El protocolo de calibración (§14.3) no es contabilidad: los errores de alta confianza se marcan y generan tarjeta prioritaria. Son los eventos de mayor rendimiento del ciclo. |
| **Consolidación durante el sueño** | `■■■` | La reactivación durante el sueño consolida memoria declarativa y procedimental (Rasch & Born, 2013) | Domingo sin estudio. Recortar sueño por carga académica destruye lo estudiado esa semana: es pérdida neta, no sacrificio (§10). |
| **Calibración metacognitiva** | `■■■` | La fluidez de procesamiento se confunde sistemáticamente con dominio (Koriat & Bjork, 2005) | Predicción numérica de nota antes de cada evaluación; registro del error de calibración. |
| **Límite de capacidad** | `■■■` | La memoria de trabajo maneja ≈4 elementos independientes, no 7 (Cowan, 2001) | Ninguna tarjeta con más de 4 elementos nuevos. Toda demostración de más de 4 pasos se descompone en lemas nombrados antes de memorizarse (§11.1). |
| **Práctica deliberada** | `■■□` | La mejora exige repeticiones en el límite de competencia con feedback inmediato (Ericsson et al., 1993). **Advertencia:** el meta-análisis de Macnamara, Hambrick & Oswald (2014) encuentra que la práctica deliberada explica ≈21–26% de la varianza en música y juegos, pero solo ≈4% en educación. El mecanismo es real; su poder explicativo fue sobrevendido | La Prueba de Dominio arranca en la **semana 2**, no al final. Fallo controlado temprano. Se conserva la regla; se retira la pretensión de que la práctica deliberada baste. |

**Corrección respecto de 2026.1.** La versión anterior citaba a Ericsson sin matiz. Se añade el contrapeso de Macnamara et al. porque el documento es prescriptivo y la diferencia importa: la práctica deliberada estructurada es la mejor palanca disponible, pero atribuirle el 100% del resultado convierte cualquier fracaso en un problema moral del estudiante. No lo es. Hay varianza que la metodología no controla.

---

## 9. Sustrato neurobiológico

Por qué funcionan los mecanismos de §8. Esta sección no es interpretativa: cambia decisiones concretas de calendario, de diseño de tarjetas y de gestión de carga, y esas consecuencias se señalan en cada punto.

### 9.1 Consolidación sistémica y sistemas complementarios de aprendizaje `■■■`

El cerebro no tiene un sistema de memoria, tiene dos con propiedades opuestas. El **hipocampo** codifica rápido, de una sola exposición, con representaciones separadas entre sí. El **neocórtex** aprende lento, por exposición repetida y distribuida, con representaciones superpuestas que capturan estructura. La consolidación sistémica es la transferencia gradual del primero al segundo, y ocurre en gran parte durante el sueño mediante reactivación (Squire & Alvarez, 1995; Rasch & Born, 2013).

La formulación que interesa aquí es la de **sistemas complementarios de aprendizaje** (McClelland, McNaughton & O'Reilly, 1995): el neocórtex debe aprender de forma entrelazada porque aprender rápido y concentrado en una red de representaciones superpuestas produce **interferencia catastrófica** — lo nuevo sobrescribe lo viejo. El hipocampo existe, en este modelo, para permitir adquisición rápida sin destruir lo consolidado, y para reproducir la experiencia de forma intercalada mientras el neocórtex la integra.

**Reconocimiento obligado.** Este modelo es el ancestro directo del *experience replay* en aprendizaje por refuerzo. Cuando en IAP-603 se estudie por qué DQN necesita un buffer de repetición y no puede entrenar en línea sobre transiciones consecutivas, es el mismo argumento: entrenamiento correlacionado sobre una red de pesos compartidos destruye lo aprendido. El estudiante está sujeto a la restricción que después va a implementar.

**Consecuencias operativas.**

1. El espaciado y el intercalado no son trucos de estudio: son la política de entrenamiento que la arquitectura exige. Estudiar un tema en bloque masivo es el equivalente a entrenar sin buffer de repetición.
2. Una asignatura estudiada en bloque concentrado y luego abandonada durante meses queda en estado hipocampal, no consolidada. Es exactamente lo que produce la sensación de "yo esto lo llevé pero no me quedó nada": no es falla de esfuerzo, es falta de reactivación distribuida.
3. Por eso el plan prohíbe cursar una asignatura y cerrarla: el mazo FSRS de cada asignatura **sigue activo hasta la graduación** (§12.3), no hasta el examen final.

### 9.2 Etiquetado y captura sináptica `■■□`

En modelos animales, una estimulación débil que por sí sola produciría solo potenciación transitoria puede producir potenciación duradera si ocurre **cerca en el tiempo** de una estimulación fuerte en la misma población neuronal. La explicación estándar: la estimulación débil deja un "tag" local, y captura las proteínas relacionadas con plasticidad que la estimulación fuerte manda a sintetizar (Frey & Morris, 1997; síntesis en Redondo & Morris, 2011).

**Estado de la evidencia.** Sólido en roedor, con evidencia conductual en humanos consistente pero indirecta. Se declara `■■□` por eso: la extrapolación a "estudiar material menor junto a material mayor" es razonable, no demostrada.

**Consecuencia operativa.** En el diseño de bloques (§13.1), el material de baja intensidad no se agrupa aparte: se coloca **adyacente** al bloque de máxima dificultad del día y del mismo dominio conceptual. Concretamente: la revisión de notación y definiciones de TEO-302 va inmediatamente después del bloque de construcción de reducciones, no en un bloque separado de "repaso ligero". Si el efecto existe en humanos, se aprovecha; si no, no se pierde nada.

### 9.3 Espaciado con mecanismo celular `■■□`

El efecto conductual del espaciado (§8) tiene correlato a nivel de plasticidad: los protocolos de estimulación **espaciada** producen potenciación de larga duración más estable que los masivos con el mismo número total de estímulos, y la diferencia depende de síntesis de proteínas y de vías de señalización tipo CREB. El espaciado no es una limitación de la atención humana: es una propiedad del sustrato.

**Consecuencia operativa.** Refuerza la prohibición de intervalos fijos de §12: si el mecanismo es de consolidación molecular y no de aburrimiento, entonces el intervalo correcto es función del estado de la traza, que es exactamente lo que FSRS estima y lo que un multiplicador fijo ignora.

### 9.4 Error de predicción como señal de aprendizaje `■■■`

El aprendizaje asociativo está impulsado por **discrepancia entre lo predicho y lo ocurrido**, no por exposición. La señal dopaminérgica de error de predicción de recompensa es el caso mejor caracterizado, y —de nuevo— es el ancestro directo del aprendizaje por diferencia temporal que se estudia en IAP-603.

Combinado con el efecto de hipercorrección (§8): **el evento de máximo rendimiento de aprendizaje es un error cometido con alta confianza y corregido de inmediato.** No un acierto, ni un error esperado.

**Consecuencias operativas.**

1. La regla de 25 minutos a ciegas (§13.2) existe para generar predicción antes de la información. Sin predicción no hay error de predicción y la exposición no se codifica.
2. En la bitácora, los errores se clasifican por confianza previa además de por tipo. Un error cometido con confianza alta se marca `HC` y genera tarjeta el mismo día, con prioridad sobre cualquier otra.
3. Consultar la solución antes de intentar no es "ahorrar tiempo": es cancelar la señal que produce el aprendizaje. Es la justificación mecanística de §16.

### 9.5 Reconsolidación: recuperar modifica la traza `■■□`

Recuperar una memoria no es leerla: la vuelve momentáneamente lábil y exige re-estabilizarla. La ventana de labilidad es la razón por la que la práctica de recuperación es tan potente —y también por la que es peligrosa mal ejecutada.

**Consecuencia operativa, y es dura.** Recuperar incorrectamente y **no corregir en el momento** no deja la memoria como estaba: la reescribe con el error incorporado. De ahí tres reglas:

1. Ninguna sesión de recuperación termina sin verificación contra fuente. Recuperar sin verificar es peor que no recuperar.
2. Prohibido "creo que era así, luego lo confirmo". La confirmación es parte de la operación, no un pendiente.
3. En FSRS, una tarjeta fallada se revisa el mismo día con la respuesta correcta delante, no solo se reprograma.

### 9.6 Curiosidad y estado de codificación `■■□`

Los estados de alta curiosidad se asocian con mayor actividad hipocampal y mejor memoria **incluso para material incidental** presentado durante ese estado (Gruber, Gelman & Ranganath, 2014). El hallazgo es influyente y tiene seguimientos, pero la base es acotada.

**Consecuencia operativa.** Es una razón adicional, independiente del efecto de generación, para abrir toda unidad con el problema y no con la solución: el enunciado sin resolver instala el estado en el que el material posterior se codifica mejor. En la práctica: cada unidad de cada asignatura abre con el problema abierto que la motivó históricamente, no con la definición.

### 9.7 Estrés, glucocorticoides y la estructura que el plan necesita `■■■`

El estrés agudo y moderado alrededor del momento de codificación puede mejorar la consolidación. La elevación **crónica** de glucocorticoides tiene el efecto contrario: deteriora la función hipocampal y el desempeño en memoria declarativa, que es precisamente el sistema del que depende todo este programa.

**Consecuencia operativa, y es la razón neurobiológica de la corrección de §3.** Un régimen de 84–91 h/semana sostenido durante años no es "duro": es un protocolo de elevación crónica de cortisol aplicado sobre el hipocampo. El plan quedaría dependiendo de la estructura que él mismo estaría degradando. Las semanas pico de §3.5 son aceptables por ser agudas y acotadas; un régimen pico permanente no lo es. Esto no es una recomendación de bienestar añadida al final: es una restricción de ingeniería del propio plan.

### 9.8 Neurogénesis hipocampal adulta en humanos `■□□`

Se declara explícitamente como **contestada**. Sorrells et al. (2018) reportan que la neurogénesis hipocampal en humanos cae a niveles indetectables en la infancia; Boldrini et al. (2018), con metodología distinta, reportan persistencia hasta edad avanzada. El desacuerdo no está resuelto.

**Por qué figura aquí.** Porque una parte importante de la divulgación sobre "ejercicio y neurogénesis" se presenta como establecida cuando no lo está. Las recomendaciones de ejercicio de §10.4 se sostienen en evidencia conductual y de volumen hipocampal en humanos, **no** en neurogénesis. Si mañana se resuelve que no hay neurogénesis adulta en humanos, esas recomendaciones no cambian. Ese es el criterio: no apoyar una decisión en un mecanismo en disputa cuando existe evidencia directa del efecto.

### 9.9 "Modo focalizado" y "modo difuso" `■□□`

La dicotomía popularizada en la divulgación sobre aprendizaje (y muy difundida en cursos de estudio para CS) no es un hallazgo de neurociencia con ese nombre. Lo que existe: la red por defecto está activa en reposo y durante el pensamiento no dirigido, y hay evidencia de **incubación** —dejar un problema y volver mejora la tasa de solución en cierto tipo de problemas de insight.

**Consecuencia operativa, acotada.** Se conserva la práctica —dejar reposar una demostración atascada y retomarla— porque el efecto de incubación tiene soporte conductual. Se retira el vocabulario de "modos", porque nombrar mal un mecanismo lleva a inferencias falsas sobre él. La regla operativa es: **tras 45 minutos sin avance estructural en una demostración, se cierra y se retoma al día siguiente.** No "se cambia a modo difuso".

---

## 10. Sueño, cronobiología y sustrato físico

Esta sección es nueva. Está aquí porque es la única parte del régimen donde el incumplimiento no se compensa con más esfuerzo.

### 10.1 Arquitectura del sueño y qué consolida cada fase `■■■`

El sueño no es homogéneo. Los ciclos duran ≈90 minutos y su composición cambia a lo largo de la noche: el **sueño de ondas lentas (SWS)** se concentra en el primer tercio; el **sueño REM** en el último. Esto tiene consecuencias distintas para el material de este programa:

| Fase | Predomina | Consolida preferentemente | Material del plan afectado |
|---|---|---|---|
| **NREM / SWS** | Primer tercio de la noche | Memoria declarativa; reactivación hipocampo→neocórtex, acoplada a oscilación lenta y husos | Definiciones, enunciados de teoremas, hechos, estructura de demostraciones |
| **REM** | Último tercio | Memoria procedimental, integración en esquemas, generalización | Fluidez en manipulación algebraica, depuración, reconocimiento de patrones de prueba, transferencia entre dominios |

**Consecuencia operativa, y es contraintuitiva.** Dormir 5 horas en lugar de 8 no recorta el 37% de la consolidación de forma uniforme: recorta **desproporcionadamente el REM**, porque el REM está al final. Es decir, la privación parcial de sueño golpea con más fuerza exactamente lo que este programa más necesita —la integración, la fluidez procedimental y la transferencia— y relativamente menos la memorización de enunciados. Un estudiante que duerme poco puede seguir rindiendo en preguntas de definición mientras pierde capacidad de resolver problemas nuevos, y va a interpretar eso como que "sabe la teoría pero no le salen los ejercicios". La causa puede estar en el horario de sueño, no en el método de estudio.

### 10.2 Privación de sueño y capacidad de codificar `■■■`

El daño no es solo retrospectivo. Una noche de privación de sueño **antes** del aprendizaje deteriora la codificación hipocampal del material nuevo (Yoo et al., 2007). Es decir: no se pierde solo lo estudiado ayer, se pierde la capacidad de adquirir lo de hoy.

**Consecuencia operativa.** Estudiar de noche a costa del sueño para adelantar material tiene un costo compuesto: degrada la consolidación de lo ya visto **y** la adquisición de lo siguiente. Es la operación de peor rendimiento disponible en todo el régimen, y el plan la prohíbe explícitamente. La regla de §3.5 —el pico se absorbe recortando tarjetas nuevas, nunca sueño— se sostiene en este hallazgo.

### 10.3 Siestas y ventanas de reposo `■■□`

- Siesta breve (**10–20 min**, sin entrar en sueño profundo): recupera alerta y desempeño; efecto sobre consolidación modesto.
- Siesta de ciclo completo (**≈90 min**): incluye SWS y algo de REM; hay evidencia de beneficio de consolidación comparable a una fracción de noche.
- Rango intermedio (**30–60 min**): riesgo de despertar en sueño profundo con inercia de sueño prolongada. Es el peor uso del tiempo de los tres.

**Consecuencia operativa.** Si se usa siesta, se usa a 20 minutos o a 90, no en medio. En el horario de §13.1, la ventana natural es después del bloque de práctica de la tarde.

### 10.4 Ejercicio aerobio `■■□`

El ejercicio aerobio regular se asocia con mejor desempeño en memoria y función ejecutiva y con mayor volumen hipocampal en humanos (Erickson et al., 2011, con incremento ≈2% en adultos mayores tras un año de entrenamiento aerobio). Los tamaños de efecto en adultos jóvenes sanos son más discutidos y los meta-análisis recientes son más conservadores que la primera ola de estudios.

Sobre el momento: hay evidencia de que una sesión de ejercicio **algunas horas después** de la codificación mejora la retención (van Dongen et al., 2016), pero es un estudio único que necesita replicación — `■□□` para el timing específico, `■■□` para el efecto general.

**Consecuencia operativa, deliberadamente modesta.** Se recomienda ejercicio aerobio regular como parte del régimen, calendarizado, no opcional. No se prescribe un protocolo de timing fino porque la evidencia no lo sostiene. Se declara como lo que es: una intervención con soporte razonable y sin costo de oportunidad relevante, no una palanca de rendimiento cuantificada.

### 10.5 Cronotipo y efecto de sincronía `■■□`

El desempeño en tareas cognitivas exigentes varía según la hora del día y **según el cronotipo individual**: rinde mejor en el momento óptimo de cada persona, no en un horario universal (efecto de sincronía; May & Hasher). La diferencia es mayor en tareas que requieren control inhibitorio, que es la mayoría de las de este plan.

**Consecuencia operativa, y corrige un supuesto de 2026.1.** El horario canónico de §13.1 arranca a las 08:00 y coloca ahí los bloques de mayor dificultad, con la justificación "cerebro descansado". Eso es correcto para un cronotipo matutino y falso para uno vespertino. La regla nueva:

> El horario de §13.1 fija la **estructura** (número de bloques, orden de dificultad, posición del FSRS relativa a los bloques de adquisición). Las **horas de reloj** se anclan al cronotipo propio, medido con dos semanas de registro de rendimiento en problemas cronometrados a distintas horas antes de fijar el horario. Copiar el reloj de otro es un error de calibración, no disciplina.

### 10.6 Cafeína `■■■` (mecanismo) / `■■□` (implicación operativa)

La cafeína es antagonista de receptores de adenosina: bloquea la señal de somnolencia acumulada, no la elimina. Mejora alerta y sostenimiento de atención; **no hay evidencia de que mejore la consolidación**. Su vida media es de ≈5 horas (con variación interindividual grande, mediada por CYP1A2), y el consumo tardío reduce y fragmenta el SWS.

**Consecuencia operativa.** Es una herramienta de alerta, no de aprendizaje. Consumo tardío intercambia alerta de hoy por consolidación de esta noche, que es el intercambio equivocado según §10.1. Corte práctico: ninguna ingesta dentro de las 8 horas previas al sueño.

### 10.7 Lo que esta sección no dice

No se prescriben suplementos, nootrópicos, dietas específicas ni protocolos de optimización metabólica. No porque sean irrelevantes, sino porque la evidencia disponible para adultos sanos no sostiene recomendaciones específicas al nivel de precisión del resto de este documento, y una recomendación con más precisión que su evidencia es peor que ninguna. Para cualquier decisión de salud —incluyendo sueño persistentemente malo o carga que produzca síntomas físicos— la consulta es médica, no curricular.

---

## 11. Carga cognitiva, atención y límites de procesamiento

### 11.1 Capacidad de memoria de trabajo `■■■`

El límite operativo es de **≈4 elementos independientes** (Cowan, 2001), no los 7±2 de la formulación popular de Miller. La cifra importa porque define el tamaño máximo de unidad que se puede manipular sin apoyo externo.

**Consecuencias operativas.**

1. **Diseño de tarjetas (§12.1):** ninguna tarjeta introduce más de 4 elementos nuevos. Una tarjeta con 6 casos de un teorema no es una tarjeta difícil, es una tarjeta mal construida.
2. **Descomposición de demostraciones:** toda demostración de más de 4 pasos estructurales se reescribe como una cadena de **lemas nombrados** antes de intentar retenerla. El nombre es el mecanismo de agrupamiento (*chunking*): un lema con nombre ocupa un espacio, sus tres pasos internos ocupan tres.
3. **Por qué la manipulación algebraica debe ser automática:** cada paso algebraico que aún requiere atención consciente consume uno de los cuatro espacios, y los deja sin disponibilidad para la estructura del argumento. La fluidez de bajo nivel no es adorno: es liberación de capacidad. Es la razón de que MAT-101 a MAT-104 vayan primero y se practiquen a mano.

### 11.2 Teoría de la carga cognitiva `■■■`

Tres fuentes de carga: **intrínseca** (complejidad inherente del material y su interactividad de elementos), **extrínseca** (impuesta por la presentación) y **relevante** (invertida en construir el esquema). La intervención útil es reducir la extrínseca para liberar capacidad hacia la relevante.

**Consecuencias operativas.**

1. La carga extrínseca en este programa viene sobre todo de **notación inconsistente entre fuentes**. Regla: por asignatura, se fija una notación canónica —la del libro base— y toda fuente secundaria se traduce a ella al leerla, en el momento, por escrito. Leer cuatro libros con cuatro notaciones y no traducir es pagar carga extrínseca por elección.
2. **Efecto de reversión por experticia** (§8): el andamiaje que ayuda al novato estorba al experto. Operativamente: los ejemplos resueltos se abandonan en cuanto la técnica sale sin ellos. Seguir con ejemplos resueltos después de ese punto reduce el aprendizaje, no lo aumenta.

### 11.3 Costo de cambio de tarea y residuo de atención `■■■`

Alternar entre tareas tiene un costo de reconfiguración medible, y queda un **residuo de atención** de la tarea anterior que degrada el rendimiento en la siguiente. El costo escala con la disimilitud de las tareas y con la interrupción abrupta.

**Consecuencias operativas.**

1. Los bloques de 90 minutos son de una sola asignatura. Sin excepción.
2. Notificaciones y mensajería cerradas durante bloques de adquisición. No es higiene digital genérica: es que el residuo de una interrupción de 30 segundos degrada varios minutos posteriores de trabajo.
3. **Cierre explícito.** Todo bloque termina escribiendo en una línea dónde se quedó y cuál es el siguiente paso concreto. Reduce el residuo al reabrir y elimina los primeros minutos de reorientación.

### 11.4 Sobre el bloque de 90 minutos `■□□`

La justificación habitual —"ciclos ultradianos de ≈90 minutos en vigilia" (BRAC, Kleitman)— tiene evidencia débil para vigilia. Se declara como tal.

La justificación real del bloque de 90 minutos en este plan es más modesta y suficiente: **decremento de vigilancia** en tareas sostenidas y demandantes, más la conveniencia práctica de una unidad que permite una fase de intento a ciegas de 25 minutos, una de consulta y una de consolidación escrita. El número podría ser 75 o 100 sin que cambie nada esencial. Se fija en 90 por convención, no por biología.

---

## 12. Sistema de repaso espaciado

### 12.1 Diseño de tarjetas por tipo de contenido

**Regla raíz: si la tarjeta se responde por reconocimiento, se elimina.** El mazo no es un glosario.

**Regla de capacidad (nueva, §11.1): ninguna tarjeta introduce más de 4 elementos nuevos.**

| Tipo | Anverso | Reverso | Criterio de "Good" |
|---|---|---|---|
| Teorema | Enunciado + "reconstruye la demostración" | Esqueleto de la prueba, no texto completo | Reconstruiste el esqueleto sin ver |
| Punto de quiebre | "¿Qué falla en el teorema X si elimino la hipótesis H?" | El contraejemplo concreto | Nombraste el contraejemplo, no solo "deja de valer" |
| Algoritmo | Problema + restricción | Invariante de bucle + complejidad + caso donde falla la variante ingenua | Enunciaste el invariante, no el pseudocódigo |
| Traza de sistema | Fragmento de código, estado de registros o contenido de caché | Estado tras N pasos | Predijiste antes de verificar con GDB, `perf` o valgrind |
| Derivación | Punto de partida + objetivo | Cadena de pasos | Se practica en papel. Nunca mentalmente. |
| Definición formal | El primitivo | La definición exacta | Solo irreducibles: σ-álgebra, PAC-learnable, IND-CCA2, linearizabilidad. **Máx. 15% del mazo.** |
| Contraejemplo | Afirmación falsa plausible | Contraejemplo mínimo | Máxima densidad informativa: priorizar este tipo |
| **Error de alta confianza** | El enunciado donde se falló estando seguro | La corrección + por qué la intuición previa era plausible pero falsa | **Nuevo tipo (§9.4).** Generado obligatoriamente el mismo día del error. Prioridad sobre todos los demás. |

### 12.2 Configuración operativa

Verificada contra la documentación de FSRS y de Anki el 25/07/2026.

| Parámetro | Valor | Motivo |
|---|---|---|
| Algoritmo | FSRS (nativo en Anki desde la versión 23.10) | Programa contra la curva de olvido individual, no contra multiplicadores fijos |
| Retención deseada | 0.90 | Punto de equilibrio. El rango admitido es 0.70–0.99, pero el costo es **no lineal**: pasar de 0.90 a 0.95 aproximadamente duplica las repeticiones diarias, y de 0.95 a 0.97 las vuelve a duplicar por una ganancia marginal |
| Retención óptima calculada | Consultar, no adoptar a ciegas | FSRS puede calcular la retención que minimiza tiempo total de estudio; suele caer entre 0.85 y 0.90. Si el cálculo propio da <0.85 para este material, **no** bajarla: en un programa de 5+ años la retención objetivo la fija el horizonte de uso, no el mínimo de tiempo |
| Optimización de parámetros | tras ≥1 000 reviews, máx. 1 vez/mes | Optimizar seguido persigue ruido |
| Máx. reviews/día | sin tope | Un tope crea backlog oculto que estalla |
| Control de carga | limitando **tarjetas nuevas** | Es la única palanca sana |
| Tarjetas nuevas/día | 15–25 por asignatura activa | Por encima de 30 la calidad de tarjeta cae |
| Intervalo máximo | 36 500 días | No truncar; el material del plan se usa durante toda la carrera |
| Pasos de aprendizaje | 1m 10m | Configuración estándar; añadir un paso de 1d mejora retención de la primera semana a costa de más repeticiones |
| Cambios de configuración | una variable, medida 2 semanas | Cambiar varias a la vez no produce datos |

**Advertencia de FSRS documentada.** El algoritmo se adapta a casi cualquier hábito **excepto uno**: pulsar "Hard" en lugar de "Again" cuando efectivamente se olvidó. Eso corrompe los datos de entrenamiento del modelo. En este plan, la calificación es binaria de hecho: si no se reconstruyó lo que el criterio de "Good" exige, es "Again".

### 12.3 Persistencia de mazos entre ciclos

**Regla nueva, derivada de §9.1.** El mazo de una asignatura no se archiva al aprobarla. Permanece activo hasta la graduación, con tarjetas nuevas en cero y solo repeticiones programadas. El costo en estado estacionario es de ≈15–25 min/día para todo el histórico acumulado; el beneficio es que MAT-101 sigue disponible cuando SEG-701 lo necesite, cuatro bloques después.

Archivar un mazo al aprobar la asignatura es la decisión que garantiza que el ciclo VII encuentre vacío lo que el ciclo I dejó.

---

## 13. Régimen semanal

Un solo esqueleto para todos los bloques. Las horas de reloj se anclan al cronotipo propio (§10.5); lo que se conserva es la estructura.

### 13.1 Arquitectura de bloques

Bloques de 90 minutos, de una sola asignatura (§11.3). **Máximo cuatro bloques de adquisición al día:** por encima de ese umbral la calidad de codificación cae y solo se acumula tiempo de silla.

Plantilla para ruta R1 (§14.1), con cuatro asignaturas concurrentes `A1`–`A4` y un integrador `INT`:

| Franja relativa | Lunes | Martes | Miércoles | Jueves | Viernes |
|---|---|---|---|---|---|
| **Pico 1** (bloque de mayor rendimiento propio) | A1 · Teoría | A3 · Teoría | A1 · Teoría | A3 · Teoría | A1 · Teoría |
| **Pico 2** | A2 · Teoría | A4 · Teoría | A2 · Teoría | A4 · Teoría | A2 · Teoría |
| **Cierre de mañana** (40 min) | FSRS | FSRS | FSRS | FSRS | FSRS |
| **Tarde 1** | A1 · Práctica | A3 · Práctica | A2 · Práctica | A4 · Práctica | A3 · Práctica |
| **Tarde 2** | INT · Lab | A1/A2 · Lab | INT · Lab | A3/A4 · Lab | INT · Lab |
| **Noche** (opcional según ruta) | EI dirigido | EI dirigido | EI dirigido | EI dirigido | EI libre |

| Franja | Sábado | Domingo |
|---|---|---|
| **Bloque 1** | Intercalado — dominio α | — |
| **Bloque 2** | Intercalado — dominio β | — |
| **Bloque 3** | Intercalado — dominio γ + bitácora | — |
| Resto | Libre | **Descanso absoluto** |

**Cómputo de la plantilla R1:** 20 bloques de adquisición y práctica (30 h) + 3.3 h FSRS + 10 h EI dirigido + 4.5 h sábado = **47.8 h estructuradas**, más ≈10 h de trabajo autónomo no calendarizado (lectura, problem sets, avance de Prueba de Dominio) = **≈58 h/semana**. Esta cifra sí es consistente con §14.1 y con la carga de cuatro asignaturas de las fichas.

### 13.2 Reglas duras del régimen

1. **Primera pasada a ciegas.** 25 minutos de intento sin material antes de abrir libro, apuntes o buscador. La justificación es §9.4: sin predicción no hay error de predicción.
2. **Cero relectura pasiva.** La relectura ocurre *después* de fallar la recuperación, nunca antes.
3. **Verificación obligatoria (§9.5).** Ninguna sesión de recuperación termina sin comparar contra fuente. Recuperar sin verificar reescribe la traza con el error incorporado.
4. **FSRS no acumulable.** El bloque de repaso no se pospone ni se dobla al día siguiente.
5. **Bitácora de errores con confianza.** Cada error se clasifica por tipo —concepto / álgebra / lectura del enunciado / técnica— **y por confianza previa** (alta/media/baja). Los de confianza alta se marcan `HC` y generan tarjeta el mismo día (§9.4).
6. **Un cambio por vez.** Al ajustar el método se modifica una variable y se mide dos semanas.
7. **El bloque de práctica de la tarde trabaja el material de *ayer*, no el de hoy.** Espaciado corto incorporado al horario.
8. **Cierre escrito de bloque (§11.3).** Una línea: dónde se quedó y cuál es el siguiente paso concreto.
9. **Adyacencia de material ligero (§9.2).** La revisión de notación y definiciones va inmediatamente después del bloque de máxima dificultad del mismo dominio, no en un bloque aparte.
10. **Techo de sueño inviolable.** Ninguna operación del régimen —pico de evaluación incluido— se financia con horas de sueño (§10.2).

### 13.3 Matriz de intercalado sabatino

El bloque del sábado rota tres dominios. **Criterio corregido en esta versión:** el intercalado rinde más entre técnicas **confundibles** que entre dominios distantes, porque lo que entrena es la discriminación —elegir la técnica correcta— no la ejecución. Los tríos se rediseñaron con ese criterio.

| Ciclo | Dominio α | Dominio β | Dominio γ | Confusión que entrena |
|---|---|---|---|---|
| I | Inducción débil vs fuerte vs estructural | Factorización LU vs QR vs SVD | Convergencia puntual vs uniforme | Elegir la variante correcta del mismo método |
| II | Traza x86-64 vs RISC-V | Análisis amortizado vs peor caso | Semántica small-step vs big-step | Marco de análisis correcto |
| III | Reducción many-one vs Turing | Bombeo regular vs libre de contexto | Método probabilístico vs conteo | Dirección y tipo de reducción |
| IV | Voraz vs DP vs divide y vencerás | Dualidad LP vs Farkas vs complementariedad | Capacidad de canal vs tasa de código | Paradigma de diseño correcto |
| V | Concurrencia de kernel vs de usuario | SSA vs dataflow clásico | LTL vs CTL | Nivel de abstracción correcto |
| VI | Cotas VC vs Rademacher vs PAC-Bayes | Backprop analítico vs numérico | Circuito cuántico vs clásico | Herramienta de generalización correcta |
| VII | Reducción de seguridad vs juego de indistinguibilidad | FLP vs CAP vs cotas de consenso | Tipado dependiente vs refinamiento | Modelo de imposibilidad correcto |
| VIII | Grano fino vs parametrizada vs aproximación | Leyes de escalamiento vs cotas de muestra | Crítica metodológica vs replicación | Marco de análisis de frontera |

### 13.4 Asignación de asignaturas a franjas

**Criterio.** Las franjas de mayor rendimiento propio (medidas según §10.5, no asumidas) reciben las asignaturas de dificultad 9–10. Las de dificultad 7–8 van a franjas residuales. El integrador ocupa bloques de laboratorio, nunca franjas pico.

Para la asignación concreta por ciclo, ver §14.2 (que depende de la ruta, ya que R1 lleva 4 asignaturas concurrentes y R3 lleva 2).

### 13.5 Calendario del bloque (16 semanas de contenido)

| Semana | Hito | Detalle |
|---|---|---|
| 1 | Diagnóstico | Evaluación de prerrequisitos por asignatura. Un fallo obliga a nivelación antes de la semana 3. |
| 2 | **Arranque de Pruebas de Dominio** | Todas las Pruebas de Dominio se abren aquí. Fallo controlado temprano, no entrega final. |
| 3–6 | Unidades 1–2 | Problem sets semanales desde la semana 2. |
| 7 | **Evaluación Parcial 1** | Perfil teórico. Pico de carga. |
| 8 | Evaluación Parcial · sistemas | Perfil sistemas. **Semana de calibración:** revisión del error acumulado (§14.3). |
| 9–13 | Unidades 3–5 | Avance obligatorio de Prueba de Dominio con hito verificable en la semana 11. |
| 14 | **Evaluación Parcial 2** | Perfil teórico. Pico de carga. |
| 15 | **Entrega y defensa de Pruebas de Dominio** | Pico máximo del bloque. |
| 16 | **Examen Final + cierre del Laboratorio Integrador** | Defensa oral del integrador. **Segunda semana de calibración.** |

**Semanas 7, 14 y 15:** carga +30–40% sobre la base de la ruta (§3.5). Se absorben recortando tarjetas nuevas y trabajo autónomo de otras asignaturas.

---

## 14. Rutas de titulación

Esta sección reemplaza a §11 de la 2026.1. La diferencia es que las duraciones se calculan desde el presupuesto de horas de §3.2, no se declaran.

**Fórmula.** `bloques = horas_totales / (h_semanales × semanas_por_bloque)`. Con 40 semanas de estudio efectivo al año (dejando 12 de holgura para descanso, imprevistos y reingreso), `años = horas_totales / (h_semanales × 40)`.

### 14.1 Comparación de rutas

| Ruta | h/sem | Asignaturas concurrentes | Alcance | Créditos | h totales | **Duración** |
|---|---|---|---|---|---|---|
| **R0 — 2026.1 tal como estaba escrita** | 88 | 6 | Completo | 201 | 11 300 | *Inviable. Se documenta para que no se reintente.* |
| **R1 — Institucional replicado** | 55–60 | 4 + integrador | Completo | 201 | 11 300 | **≈6.5 años** (dedicación exclusiva) |
| **R2 — Intensivo con ocupación parcial** | 35–40 | 3 | Completo | 201 | 11 300 | **≈8–9 años** |
| **R3 — Núcleo** ⭐ | 20–25 | 2 | Núcleo + integradores | 115 | 6 480 | **≈6.5–8 años** |
| **R4 — Admisión a posgrado** | 15–20 | 2 | Subconjunto orientado | 57 | 3 150 | **≈4–5 años** |
| **R5 — Fundamentos** | 20–25 | 2 | Ciclos I–IV | 100 | 5 500 | **≈5.5–7 años** |

**⭐ R3 es la ruta recomendada por defecto** para quien no tiene dedicación exclusiva. No es una versión degradada: son 6 480 horas, equivalentes en volumen a una licenciatura europea completa de 240 ECTS, con la selección hecha por criticidad estructural y no por facilidad.

**Sobre R1.** Cuatro asignaturas concurrentes es lo que MIT, CMU, Stanford y Berkeley efectivamente asignan a un estudiante a tiempo completo. Replicar el ADN institucional (§1) implica replicar también eso. Seis era el error de 2026.1.

**Sobre la honestidad de estas cifras.** Ninguna ruta completa el programa en cuatro años porque el programa no cabe en cuatro años. Un lector que necesite un título en cuatro años debe elegir R4 o R5 y saber qué está dejando fuera, no comprimir R1.

### 14.2 Composición de las rutas

**R3 — Núcleo (27 unidades, 115 créditos, 6 480 h).** Marcadas `[NÚCLEO]` en su ficha. Son las que sostienen las cadenas críticas de §5.

```
Bloque 1:  MAT-101, SIS-101                      + INT-100
Bloque 2:  MAT-104, MAT-102
Bloque 3:  SIS-201, ALG-201                      + INT-200
Bloque 4:  LEN-201, TEO-301
Bloque 5:  TEO-302, ALG-401                      + INT-300
Bloque 6:  MAT-401, SIS-503                      + INT-400
Bloque 7:  SIS-501, LEN-501                      + INT-500
Bloque 8:  IAP-601, IAP-602                      + INT-600
Bloque 9:  SEG-701, SIS-701                      + INT-700
Bloque 10: INV-801
Bloque 11: INV-802
```

Verificación de dependencias: cada bloque satisface el grafo de §5 con los prerrequisitos cumplidos en bloques anteriores. Los integradores se cursan cuando sus tres asignaturas fuente ya están aprobadas o concurrentes.

**R4 — Admisión a posgrado (12 unidades, 57 créditos, 3 150 h).** Subconjunto orientado a lo que los comités de admisión de posgrado en CS efectivamente evalúan: base matemática, base de sistemas, teoría, algoritmos y evidencia de investigación.

```
MAT-101  Matemáticas Discretas y Lógica Formal     — base de todo
MAT-102  Álgebra Lineal Computacional              — prerrequisito de ML y gráficos
MAT-104  Probabilidad y Procesos Estocásticos      — prerrequisito de ML y análisis aleatorizado
SIS-101  Programación Científica y Sistemas        — competencia de implementación
SIS-201  Arquitectura y Sistemas                   — el curso que más señal da en admisiones de sistemas
ALG-201  Estructuras de Datos y Algoritmos         — filtro estándar
ALG-401  Diseño y Análisis de Algoritmos           — filtro estándar
TEO-301  Autómatas y Computabilidad                — requisito de currículo de CS
TEO-302  Complejidad Computacional                 — señal fuerte de madurez teórica
IAP-601  Fundamentos de Aprendizaje Automático     — según área de interés
LEN-501  Compiladores                              — el proyecto de sistemas de mayor señal
INV-801  Investigación: replicación y paper        — el componente de mayor peso en admisiones
```

**Advertencia sobre R4.** Un comité de posgrado pondera investigación y cartas por encima del expediente. INV-801 no es opcional en esta ruta: es la unidad que produce la evidencia que decide. Si hay que recortar R4, se recorta IAP-601 o LEN-501, nunca INV-801.

### 14.3 Protocolo de calibración metacognitiva

Antes de cada evaluación y de cada Prueba de Dominio: predicción numérica del resultado sobre 20. Después: registro de `|predicho − real|`.

| Error de calibración | Diagnóstico | Corrección |
|---|---|---|
| ≤ 2 puntos | Calibración sana | Ninguna |
| 3–4 puntos | Deriva leve | Aumentar proporción de recuperación libre |
| ≥ 5 puntos sostenido | **Ilusión de fluidez** | El método está produciendo reconocimiento, no dominio. Suspender relectura por completo; toda sesión pasa a formato de reconstrucción en blanco. |

**Asimetría declarada.** Sobrestimar sistemáticamente es más grave que subestimar: indica que el estudio se siente productivo sin serlo (§8, Koriat & Bjork). Subestimar sistemáticamente es un problema distinto —de confianza, no de método— y no se corrige cambiando la técnica de estudio.

**Uso obligatorio de la serie.** El registro es una serie temporal, no un dato aislado. Se grafica por bloque. Una tendencia creciente del error absoluto es la única señal temprana confiable de que el régimen elegido excede la capacidad real disponible, y es la condición de disparo para bajar de ruta (§14.4).

### 14.4 Cambio de ruta

Bajar de ruta no es fracasar; es corregir una estimación. Condiciones de disparo, cualquiera de ellas:

1. Error de calibración creciente durante dos bloques consecutivos (§14.3).
2. Incumplimiento del techo de sueño más de dos veces por bloque (§13.2.10).
3. Backlog de FSRS sostenido por encima de tres días.
4. Una Prueba de Dominio reprobada por falta de tiempo, no por falta de comprensión.

**Regla de transparencia (heredada de 2026.1 y reforzada).** Un agente o asesor que recomiende bajar de ruta debe declararlo explícitamente y decir qué asignaturas quedan fuera. Sustituir en silencio el régimen completo por uno reducido es el fallo de asistencia más dañino posible en este plan: produce un estudiante que cree estar en R1.

---

## 15. Protocolo de Pruebas de Dominio

1. **Especificación antes que código.** Invariantes y contratos escritos primero, en prosa formal. Un proyecto sin invariante escrita no se inicia.
2. **Prohibido consultar la solución de referencia** antes de tener una versión propia que corra, aunque sea mal.
3. **Reproducibilidad obligatoria.** Entorno fijado, semillas fijadas, resultados regenerables desde cero. Sin esto no hay evidencia, hay anécdota.
4. **Inyección de fallos** en Pruebas de Dominio de perfil sistemas: crash en punto arbitrario, particiones de red, entradas adversariales. Un sistema que pasa el camino feliz no está terminado.
5. **Post-mortem escrito** al cerrar: qué falló, por qué la primera hipótesis era incorrecta, qué transfiere al siguiente proyecto.
6. **Predicción antes de medición.** Antes de ejecutar cualquier benchmark, se escribe el resultado esperado con su justificación analítica. El error de predicción se documenta y se explica (§9.4). Es obligatorio en todas las Pruebas de Dominio con componente de rendimiento.
7. **Instrumentación obligatoria.** En SIS-501 y SIS-701 el artefacto debe exponer, además de funcionar, las tres señales que permiten afirmar *cómo* funciona: **latencia** —como distribución, no como media: p50 y p99—, **tasa de error** bajo la inyección de fallos del punto 4, y **saturación** del recurso que primero se agota (cola de ejecutables, ocupación del buffer, ventana de replicación pendiente). Es criterio-compuerta, no ponderación: un artefacto funcionalmente correcto que no expone las tres señales tiene la Prueba de Dominio **no superada**, con la regla de no compensación de §6 aplicada sin atenuación.
8. **Contabilidad de costo.** Toda Prueba de Dominio cuyo entregable incluya un programa escrito y ejecutado por el estudiante, y cuyo costo de ejecución varíe con el tamaño de la entrada, debe acotar ese costo y declarar su escalamiento: **cómputo** (operaciones o FLOPs, contados analíticamente y medidos), **memoria** (pico y huella en función de *n*), y —donde el artefacto se entrene o se sirva sobre acelerador— **precio**, tomado del precio publicado por GPU-hora del proveedor citado y usado como constante declarada. El escalamiento se contrasta contra la complejidad ya demostrada en la misma Prueba de Dominio: una discrepancia entre costo medido y costo derivado es un error en la derivación o en la implementación, y se resuelve antes de entregar, no se anota como ruido experimental.

### 15.1 Alcance del punto 7

Las tres señales del punto 7 son las de Beyer et al. (*SRE*, cap. 6) y el método USE de Gregg. Se adoptan como **instrumento de medición de un artefacto evaluable**, no como práctica de operación de un servicio: la distinción es la que §34 acota explícitamente, y es la misma que el plan ya aplica a la inyección de fallos desde la 2026.2 —técnica de la ingeniería de fiabilidad usada como método de evaluación, sin importar el resto de la disciplina.

**Por qué es compuerta y no ponderación.** Un núcleo o una implementación de Raft de los que solo se puede afirmar que son correctos por ausencia de fallo observado es un sistema sobre el cual no se puede razonar cuantitativamente. Las competencias C3 y C4 (§2) que estas dos asignaturas acreditan son precisamente las de razonar sobre sistemas de bajo nivel y sobre distribución con modelos de falla; un artefacto no instrumentado no evidencia esa competencia, la deja indecidible. Por eso no puede compensarse con nota alta en los demás instrumentos.

### 15.2 Alcance del punto 8 — fichas afectadas

La lista se **deriva** del criterio del punto 8 aplicado a las 39 Pruebas de Dominio, y es re-derivable por cualquier lector: se incluye una ficha si y solo si su entregable contiene un programa propio cuyo costo de ejecución crece con el tamaño de la entrada.

| Área | Fichas afectadas |
|---|---|
| MAT | MAT-101, MAT-102, MAT-103, MAT-401 |
| SIS | SIS-101, SIS-201, SIS-203, SIS-501, SIS-502, SIS-503, SIS-701, SIS-702 |
| ALG | ALG-201, ALG-403 |
| LEN | LEN-201, LEN-501, LEN-502, LEN-701 |
| TEO | TEO-401, TEO-601 |
| IAP | IAP-602, IAP-603, IAP-801 |
| | **23 de 39** |

**Las 16 restantes quedan fuera por el criterio, no por omisión.** Los tres motivos, cada uno verificable contra la ficha: (a) el entregable es una demostración y la ejecución, cuando existe, solo la verifica —MAT-104, MAT-301, MAT-601, TEO-301, TEO-302, TEO-303, ALG-401, ALG-801, IAP-601, SEG-701; (b) el entregable es un artefacto de investigación, cuyo instrumento es el perfil de §7.3 —INV-801, INV-802; (c) el artefacto es ejecutable pero su costo **no** es función del tamaño de la entrada, porque opera sobre una entrada de tamaño fijo: MAT-302 (MixColumns sobre estado 4×4), SIS-202 (circuito sintetizado, cuyo presupuesto es área y camino crítico), SEG-702 (cadena ROP contra un binario dado). La decimosexta es la excepción declarada de ALG-402, abajo.

**Sobre las dos asignaturas de verificación mecanizada, y el eje que las hace cumplir.** LEN-502 y LEN-701 se incluyen, y el motivo merece explicitarse porque el primer análisis excluyó ambas. En una formalización el costo relevante **no es el del código ejecutable extraído** —ese es un subproducto— sino el de **elaborar y chequear la prueba**: tiempo de kernel, tamaño de los términos, coste de la resolución de instancias en LEN-701; número de estados alcanzables y memoria del verificador en LEN-502. Por Curry-Howard la prueba *es* un programa y el kernel que la chequea *la ejecuta*, de modo que el criterio del punto 8 se aplica sin forzarlo: hay un programa propio cuyo costo de ejecución crece con el tamaño de su entrada, donde la entrada es la formalización o el modelo.

Y son decisionales en sentido fuerte, más que buena parte de las 23. Un chequeo que tarda minutos cambia cómo se estructura una formalización y qué tácticas se evitan. Y en *model checking* el punto donde explota el espacio de estados decide si la propiedad se verificó o si solo se agotó la búsqueda — **una propiedad "verificada" por agotamiento no está verificada**, y no hay forma de saberlo sin haber acotado el costo. Es el caso donde la contabilidad de costo no acompaña al resultado: lo condiciona.

**Componentes gobernados por prerrequisitos.** Los tres componentes del punto 8 —cómputo, memoria, precio— se exigen **solo donde el grafo de §5 haya provisto los prerrequisitos para razonar sobre ellos**. Concretamente: **MAT-101 acota operaciones y contraste contra la complejidad derivada, pero no memoria**, porque es de Ciclo I con prerrequisito `∅` y la jerarquía de memoria se enseña en SIS-201 y SIS-203, tres y dos bloques después. Exigir allí una huella de memoria razonada sería inversión de prerrequisitos: pediría usar un aparato que el plan aún no entregó. El componente de precio, análogamente, se exige solo donde el artefacto se entrene o se sirva sobre acelerador (IAP-602, IAP-801, SIS-702).

**Forma del criterio en la ficha, y es un requisito.** El párrafo de cada ficha debe **nombrar la cantidad concreta que cambia una decisión** en esa asignatura, no repetir el principio general: el tamaño de bloque derivado de la caché en SIS-201, el punto de cruce contra la DFT directa en MAT-103, el número de hilos donde la escalabilidad se aparta de S(n) en ALG-403, el umbral donde la tabla de Q deja de caber en IAP-603. Un criterio de costo que se puede satisfacer produciendo una tabla de mediciones que nadie va a usar para decidir nada es contabilidad ritual, y este plan ya declara en §17 que la presunción por defecto contra una práctica es que se sienta productiva sin serlo. La medición tiene que cerrar una decisión de diseño o no tiene que estar.

**Excepción declarada.** **ALG-402 queda fuera** pese a que su Prueba de Dominio implementa el algoritmo de Karger y su costo sí escala con *n*. El motivo es de carga, no de contenido: es perfil teórico con carga `4–2–0` —cero horas de laboratorio— y su entregable evaluable es la cota de probabilidad de éxito, no un artefacto desplegable. Exigirle contabilidad de costo de infraestructura obligaría a añadirle un componente de cómputo que la ficha no declara, y eso alteraría el presupuesto de §3.2. Se declara aquí, como el plan declara la excepción de créditos de INV-801/802 en §3.1, en lugar de resolverse en silencio.

---

## 16. Uso de modelos de lenguaje

Único protocolo permitido: **revisor adversarial, nunca generador primario.**

```
1. Escribes tu solución completa.
2. Pides que la ataque: contraejemplo, caso límite, error en el paso inductivo,
   condición de carrera no considerada, supuesto implícito.
3. Defiendes o corriges. La corrección la escribes tú.
```

En demostraciones formales el modelo verifica pasos; no los produce. En código, revisa; no escribe la primera versión.

**Justificación, ahora con mecanismo.** Generar la solución con un modelo y luego "entenderla" es exactamente el patrón que el efecto de generación (§8) predice que fallará. Con §9.4 se puede decir por qué: el aprendizaje lo produce el error de predicción, y leer una solución que uno no intentó producir genera predicción nula, error nulo y por tanto codificación mínima. Se obtiene fluidez de reconocimiento —la sensación de haber entendido— con cero capacidad de producción. Es la forma más rápida de vaciar este programa desde adentro, y el instrumento que lo detecta es el error de calibración de §14.3: un estudiante que usa modelos como generador primario muestra error creciente y sostenido, porque su fluidez sube mientras su capacidad no.

**Usos permitidos.**

| Uso | Condición |
|---|---|
| Crítica adversarial de solución propia | Solución completa escrita primero |
| Verificación de pasos de una demostración propia | La demostración es propia |
| Generación de tarjetas FSRS | Solo sobre material ya dominado |
| Traducción de notación entre fuentes | Operación mecánica (§11.2) |
| Explicación de un mensaje de error del compilador | Tras haber intentado leerlo |
| Localización de bibliografía y verificación de vigencia de ediciones | Sin delegar la lectura |
| Construcción de andamiaje de estudio (calendarios, seguimiento) | No sustituye §14.3 |

**Usos prohibidos.**

| Uso | Por qué |
|---|---|
| Primera versión de código de una Prueba de Dominio | Invalida la asignatura (§6) |
| Producción de una demostración | Elimina el evento de aprendizaje |
| Resumen de material no leído | Fluidez sin codificación |
| Elección de qué estudiar sin declarar el criterio | Traslada la decisión curricular a una caja negra |
| Tarjetas sobre material no dominado | Instala reconocimiento de texto ajeno |

**Nota sobre selección de modelo.** Para el rol de revisor adversarial, la capacidad de razonamiento del modelo importa más que la velocidad: un revisor que no encuentra el hueco en una demostración no cumple la función. Para operaciones mecánicas (traducción de notación, formateo de tarjetas), el modelo más económico es suficiente. Gastar capacidad de frontera en formatear tarjetas y capacidad mínima en criticar una prueba es la asignación exactamente invertida.

---

## 17. Prácticas desacreditadas

Un documento prescriptivo debe declarar también qué no hacer. Todo lo siguiente circula en materiales de estudio de CS y no tiene el soporte que se le atribuye.

| Práctica | Estado | Qué hacer en su lugar |
|---|---|---|
| **Estilos de aprendizaje** (visual/auditivo/kinestésico) y adaptar el material al "estilo" propio | La hipótesis de emparejamiento no tiene soporte experimental (Pashler et al., 2008). Las preferencias existen; el beneficio de atenderlas no está demostrado | Elegir el formato por el contenido: una demostración se escribe, una traza de memoria se dibuja, una derivación se hace a mano |
| **"10 000 horas" como umbral de maestría** | No es lo que dice la literatura de práctica deliberada, y el meta-análisis de Macnamara et al. (2014) muestra un poder explicativo mucho menor | Contabilizar repeticiones en el límite de competencia con feedback, no horas acumuladas |
| **Subrayar y releer** como técnica principal | Utilidad baja en la revisión de Dunlosky et al. (2013); producen fluidez sin retención | Recuperación desde cero (§8) |
| **Estudio masivo previo a la evaluación** | Funciona para pasar el examen del viernes y falla para retener al mes. Está en conflicto directo con §9.1 y §9.3 | FSRS con intervalos calculados; prohibido el repaso concentrado previo (§12) |
| **Entrenamiento cerebral** como mejora general | La transferencia lejana no se sostiene (Owen et al., 2010; revisión de Simons et al., 2016). El entrenamiento mejora la tarea entrenada | Practicar el dominio objetivo |
| **"Aprender durmiendo"** (audio durante el sueño) | No funciona para material nuevo. La reactivación dirigida con señales sí es un fenómeno real de laboratorio, pero no es esto y no es operativo | Dormir. Es la intervención (§10) |
| **Beats binaurales, "música para estudiar"** como potenciadores | Evidencia débil e inconsistente. Como enmascarador de ruido puede ser útil; como potenciador cognitivo no está sostenido | Silencio o ruido enmascarado, sin atribuirle efecto de aprendizaje |
| **Cerebro izquierdo / derecho** como tipos de estudiante | Sin base. La lateralización funcional existe; la tipología de personas no se deriva de ella | Descartar el marco |
| **Multitarea con material denso** | El costo de cambio y el residuo de atención son medibles (§11.3) | Bloques de una asignatura, notificaciones cerradas |
| **Nootrópicos sin evidencia y protocolos de suplementación agresivos** | Fuera del alcance de este documento (§10.7) | Sueño, ejercicio, y consulta médica si hay un problema real |

**Criterio general.** Si una técnica de estudio hace que el estudio *se sienta* mejor y más fluido, la presunción por defecto es que reduce el aprendizaje, no que lo aumenta (§8, dificultades deseables; §14.3, ilusión de fluidez). Esa presunción se puede refutar con datos propios de calibración, y solo con eso.

---

## 18. Protocolo de reingreso tras interrupción

Toda ruta de 5+ años se interrumpe: enfermedad, trabajo, familia, agotamiento. No tener protocolo de reingreso es la causa dominante de que una interrupción de tres semanas se convierta en abandono definitivo. Esta sección es nueva y es obligatoria.

### 18.1 Regla general

**No se reinicia desde cero.** Reiniciar es la respuesta emocionalmente natural y la peor disponible: descarta consolidación real que sigue ahí y garantiza que el segundo intento se detenga en el mismo punto que el primero. Lo que se hace es **medir qué sobrevivió** y reanudar desde ahí.

### 18.2 Procedimiento por duración de la interrupción

| Interrupción | FSRS | Contenido | Reingreso |
|---|---|---|---|
| **< 1 semana** | Se procesa el backlog completo; FSRS lo maneja nativamente considerando el retraso | Sin cambios | Inmediato |
| **1–4 semanas** | Tarjetas nuevas en 0 durante una semana; procesar backlog a ritmo de 1.5× el normal hasta vaciarlo | Repetir el último problem set entregado antes de avanzar | 1 semana de transición |
| **1–6 meses** | Tarjetas nuevas en 0 hasta vaciar backlog. **No borrar el mazo ni resetear el progreso**: el historial es el activo | Diagnóstico de la última asignatura cursada con su examen final (§7.5) | 2–4 semanas |
| **> 6 meses** | Ídem. Aceptar 4–8 semanas de repeticiones intensas | Diagnóstico de las **dos** últimas asignaturas + reverificación de prerrequisitos de la siguiente vía §5 | 4–8 semanas, y revisar la ruta en §14.1 |

### 18.3 Diagnóstico de reingreso

No es un repaso, es una medición. Para la última asignatura cursada:

1. Reconstruir en hoja en blanco su Prueba de Dominio: enunciado, estrategia, invariantes principales. Sin material. 30 minutos.
2. Resolver tres problemas de su examen final, cronometrados.
3. Comparar contra la rúbrica. **Predecir la nota antes de corregir** (§14.3).

| Resultado | Interpretación | Acción |
|---|---|---|
| ≥ 14/20 | Consolidado. La interrupción no dañó lo esencial | Avanzar |
| 10–13 | Parcial. Estructura presente, detalle perdido | Dos semanas de recuperación dirigida sobre lo fallado, luego avanzar |
| < 10 | No consolidado | Recursar la asignatura. Es más rápido que arrastrarla roto hacia el siguiente bloque |

### 18.4 Interrupción por agotamiento

Caso distinto y se trata distinto. Si la interrupción vino de sobrecarga sostenida —no de un evento externo— reanudar en la misma ruta reproduce la causa. El reingreso obliga a **bajar de ruta** (§14.4) durante al menos dos bloques completos antes de considerar volver a subir, y a documentar en la bitácora qué condición se pasó por alto. Un plan de 6 años que se interrumpe cada 18 meses por agotamiento no es un plan de 6 años: es un plan de 12 con desgaste innecesario.

# PARTE III — CATÁLOGO DE ASIGNATURAS

**Cómo leer cada ficha:**

```
### CÓDIGO — Nombre                              [NÚCLEO] si aplica
Créditos · T–P–L / EI · Dificultad /10 · Perfil de evaluación
Prerrequisitos
ADN institucional: curso fuente real

Competencia terminal      → qué sabe hacer al aprobar
Unidades                  → subcursos con semanas y contenido
Prueba de Dominio         → el artefacto que decide la aprobación
Bibliografía              → base · complementaria · papers
Recursos                  → sitio del curso fuente, materiales, herramientas
Protocolo de estudio      → táctica específica de esta asignatura
```

**Escala de dificultad:** 7 = exigente · 8 = muy exigente · 9 = filtro · 10 = nivel de posgrado avanzado en la institución fuente. Los siete laboratorios integradores (INT-*) no declaran dificultad: heredan la de las asignaturas que integran.

**Lectura de la carga — importante.** El campo `Carga` de cada ficha es la carga de **esa asignatura sola**. No es sumable con las demás del mismo ciclo de contenido para obtener un régimen semanal: cuántas se cursan en simultáneo lo decide la ruta elegida en §14, no la agrupación por ciclo de §4.2. Sumar las seis fichas de un ciclo da 84–91 h/semana, que es lo que ninguna ruta propone y lo que §3.2 documenta como inviable. Ver §3.4 para la distinción entre ciclo de contenido y bloque de calendario.

**Presupuesto por asignatura.** La tabla completa de horas totales por asignatura (carga × 16 semanas) está en §26, para planificación y para recalcular cualquier ruta.

---

# CICLO I — Fundamentos Matemáticos y Programación de Sistemas

**25 créditos · 26 h lectivas/sem · 24 h EI/sem · Total ≈50 h/sem**

> **Propósito del ciclo.** Instalar el aparato matemático completo antes de que aparezca cualquier abstracción de alto nivel. El programa no enseña a programar: enseña a demostrar, y usa C con memoria manual como el sustrato donde las demostraciones se vuelven ejecutables.

---

### MAT-101 — Matemáticas Discretas y Lógica Formal — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 10 · **16 h/sem** |
| **Dificultad** | 7/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | MIT 6.1200[J] *(ex 6.042)* · UC Berkeley CS70 |

**Competencia terminal.** Construye demostraciones formales por inducción estructural, contradicción y construcción directa, y detecta el punto exacto donde una demostración incorrecta falla.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Lógica y método de prueba | Lógica proposicional · Lógica de primer orden · Deducción natural · Teoría de pruebas · Prueba directa, contrapositiva, contradicción · Errores de cuantificación |
| 2 | 4–6 | Fundamentos de conjuntos | Teoría axiomática ZFC · Relaciones, funciones, órdenes parciales · Cardinalidad · Diagonalización de Cantor |
| 3 | 7–9 | Inducción | Inducción débil, fuerte y estructural · Recursión bien fundada · Invariantes de estado · Terminación |
| 4 | 10–12 | Teoría de números | Aritmética modular · MCD y Euclides extendido · Inversos modulares · Teorema Chino del Resto · Generadores · Logaritmo discreto |
| 5 | 13–15 | Grafos y combinatoria | Conectividad, árboles, coloración, planaridad · Permutaciones y combinaciones · Principio de inclusión-exclusión · Funciones generatrices |

**Prueba de Dominio.** Demostración formal, desde axiomas ZFC, de la correctitud del algoritmo de Euclides extendido. Construcción de un solucionador SAT por resolución proposicional con prueba de terminación y análisis de complejidad empírica contrastada contra la cota teórica.

**Bibliografía.**
- **Base:** *Mathematics for Computer Science* — Lehman, Leighton & Meyer (MIT, gratuito)
- **Complementaria:** *Discrete Mathematics and Its Applications* — Rosen · *How to Prove It* — Velleman
- **Papers:** —

**Recursos.** MIT OCW 6.042J (video completo + problem sets con solución) · Berkeley CS70 notes · Automata Tutor · Lean 4 para verificar pruebas de la unidad 3.

**Protocolo de estudio.** Toda demostración se reconstruye desde el enunciado en blanco a los 3, 10 y 30 días. Es la asignatura donde el tipo de tarjeta *punto de quiebre* rinde más: para cada teorema, una tarjeta por hipótesis eliminada.

---

### MAT-102 — Álgebra Lineal Computacional — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 7/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | MIT 18.06 (Strang) |

**Competencia terminal.** Descompone matrices con control explícito del error numérico y traduce cada operación algebraica a su significado geométrico y a su costo computacional.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Espacios vectoriales | Espacios sobre campos arbitrarios · Independencia, base, dimensión · Transformaciones lineales y representación matricial · Los cuatro subespacios fundamentales |
| 2 | 4–6 | Eliminación y factorización | Eliminación Gaussiana · LU, PLU con pivoteo · Espacio nulo, rango, nulidad · Complejidad O(n³) |
| 3 | 7–9 | Ortogonalidad | Proyecciones ortogonales · Gram-Schmidt · QR · Mínimos cuadrados · Pseudoinversa de Moore-Penrose |
| 4 | 10–12 | Espectro | Valores y vectores propios · Diagonalización · Forma de Jordan · Descomposición espectral · Matrices simétricas y definidas positivas |
| 5 | 13–15 | SVD y estabilidad numérica | SVD y aplicaciones (compresión, PCA, rango bajo) · Normas matriciales · Número de condición · Estabilidad y error de redondeo |

**Prueba de Dominio.** Solver directo tipo LAPACK escrito desde cero en C para `Ax = b` con factorización LU y pivoteo parcial. Análisis de error numérico y verificación de la complejidad O(n³) por medición.

**Bibliografía.**
- **Base:** *Introduction to Linear Algebra* (6ª ed., 2023) — Strang
- **Complementaria:** *Numerical Linear Algebra* — Trefethen & Bau · *Matrix Computations* — Golub & Van Loan
- **Papers:** —

**Recursos.** MIT OCW 18.06 (curso completo en video, Strang) · MIT 18.065 (versión aplicada a datos) · Referencia BLAS/LAPACK para contrastar el solver propio.

**Protocolo de estudio.** Cada descomposición se ejecuta a mano sobre una matriz 3×3 antes de codificarla. La interpretación geométrica —qué le hace la transformación al espacio— se verbaliza en voz alta por operación, no por tema.

---

### MAT-103 — Cálculo y Análisis Real para Computación

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 7/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | MIT 18.100 |

**Competencia terminal.** Redacta demostraciones ε-δ completas y aplica análisis real al fundamento de los métodos numéricos y del procesamiento de señales.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Construcción de ℝ | Cortes de Dedekind · Completitud · Supremo e ínfimo · Densidad de ℚ |
| 2 | 4–6 | Sucesiones y series | Convergencia · Criterios · Cauchy · Series de potencias · Radio de convergencia |
| 3 | 7–9 | Continuidad y diferenciación | Continuidad ε-δ · Teorema del valor intermedio · Diferenciabilidad · Regla de la cadena multivariable · Taylor con estimación del residuo |
| 4 | 10–12 | Integración y convergencia uniforme | Integral de Riemann-Stieltjes · Convergencia uniforme · Intercambio de límites · Teorema de Arzelà-Ascoli |
| 5 | 13–15 | Análisis aplicado | Transformada de Fourier discreta y continua · Convolución · Muestreo · Métodos numéricos: Runge-Kutta, diferencias finitas |

**Prueba de Dominio.** Demostración rigurosa del Teorema de Nyquist-Shannon desde primeros principios del análisis real. Implementación de FFT radix-2 con análisis del error de punto flotante contrastado contra la cota teórica.

**Bibliografía.**
- **Base:** *Principles of Mathematical Analysis* (3ª ed.) — Rudin
- **Complementaria:** *Understanding Analysis* — Abbott (puente pedagógico hacia Rudin) · *Numerical Methods for Engineers* — Chapra & Canale
- **Papers:** —

**Recursos.** MIT OCW 18.100A/B · MIT 18.01SC para nivelación de cálculo previo · FFTW como referencia de implementación.

**Protocolo de estudio.** La asignatura de mayor densidad de ε-δ. Las pruebas se escriben completas a mano, sin abreviar cuantificadores. La abreviación temprana es la causa dominante de fallo en análisis real.

---

### MAT-104 — Probabilidad y Procesos Estocásticos — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 10 · **16 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | MIT 6.3700 *(ex 6.041)* · UC Berkeley EECS 126 · Harvard Stat 110 |

**Competencia terminal.** Analiza la complejidad esperada de algoritmos aleatorizados y modela sistemas con cadenas de Markov y teoría de colas.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Fundamentos medibles | Espacio de probabilidad (Ω, F, P) · σ-álgebras · Independencia · Probabilidad condicional · Bayes |
| 2 | 4–6 | Variables aleatorias | Discretas y continuas · Esperanza, varianza, momentos · Función generadora de momentos · Binomial, Poisson, Gaussiana, Exponencial |
| 3 | 7–9 | Teoremas límite | Desigualdades de Markov, Chebyshev, Chernoff · Ley de los grandes números (débil y fuerte) · Teorema Central del Límite con demostración |
| 4 | 10–12 | Procesos de Markov | Cadenas de Markov: clasificación de estados, ergodicidad, distribución estacionaria · Procesos de Poisson y renovación · Teoría de colas: M/M/1, M/G/1, redes de Jackson |
| 5 | 13–15 | Probabilidad en algoritmos | Monte Carlo vs Las Vegas · Hashing universal y aleatorizado · Análisis probabilístico de estructuras de datos · Concentración |

**Prueba de Dominio.** Análisis completo de la complejidad esperada del Quicksort aleatorizado + demostración de que las Skip Lists logran O(log n) en esperanza + análisis de Bloom Filters con derivación de la tasa óptima de falsos positivos. Cada resultado verificado por simulación.

**Bibliografía.**
- **Base:** *Introduction to Probability* (2ª ed.) — Blitzstein & Hwang (Harvard Stat 110)
- **Complementaria:** *Probability: Theory and Examples* — Durrett (nivel medida) · *Probability and Computing* — Mitzenmacher & Upfal
- **Papers:** —

**Recursos.** Harvard Stat 110 (video completo, gratuito) · MIT OCW 6.041 · UC Berkeley EECS 126 notes.

**Protocolo de estudio.** Toda cota se verifica por simulación antes de aceptarse. La discrepancia entre cota teórica y simulación es señal de error en la derivación, no ruido experimental.

---

### SIS-101 — Programación Científica y Sistemas — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 7/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | CMU 15-122 · MIT 6.1010 *(ex 6.009)* |

**Competencia terminal.** Escribe código C correcto por contrato, con invariantes de representación explícitas y gestión manual de memoria verificada.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelo de ejecución | Stack, heap, registros · Ciclo de compilación y enlazado · Tipos como contratos formales |
| 2 | 4–6 | Contratos e invariantes | Precondiciones y postcondiciones · Invariante de representación · Invariante de abstracción · Aserciones ejecutables |
| 3 | 7–9 | Recursión y terminación | Recursión estructural · Medida de terminación · Recursión de cola · Conversión a iteración con invariante preservado |
| 4 | 10–12 | Memoria manual | malloc/free · Punteros y aritmética de punteros · Arrays multidimensionales: row-major vs column-major · Fugas, use-after-free, double free · valgrind |
| 5 | 13–15 | Depuración a bajo nivel | GDB: breakpoints, watchpoints, inspección de memoria · Lectura de desensamblado · Sanitizers (ASan, UBSan) |

**Laboratorios.** L1 arreglos con contratos · L2 listas enlazadas con invariante · L3 tablas hash · L4 depuración de código sembrado con errores · L5 perfilado de memoria.

**Prueba de Dominio.** Slab allocator en C con free-list, coalescing de bloques libres y demostración formal de la invariante de representación mediante contratos anotados. Sometido a inyección de patrones de asignación adversariales.

**Bibliografía.**
- **Base:** *C Programming: A Modern Approach* (2ª ed.) — K.N. King
- **Complementaria:** *The C Programming Language* — Kernighan & Ritchie · *Modern C* — Gustedt (gratuito)
- **Papers:** —

**Recursos.** CMU 15-122 (sitio público con labs) · Harvard CS50x para nivelación previa · Compiler Explorer (godbolt.org) para inspeccionar el código generado.

**Protocolo de estudio.** *Predict-then-verify* obligatorio: antes de ejecutar, escribes el estado esperado de la memoria; luego lo verificas en GDB. Cada divergencia genera una tarjeta de traza.

---

### INT-100 — Laboratorio Integrador I

| | |
|---|---|
| **Créditos** | 3 |
| **Carga** | 0–0–4 / 6 · **10 h/sem** |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | MAT-101, SIS-101 (concurrentes) |

**Artefacto.** Solucionador SAT por resolución proposicional escrito en C con gestión manual de memoria, con: (a) demostración de terminación y de completitud del método de resolución, (b) análisis de complejidad empírica sobre instancias aleatorias 3-SAT contrastado contra la cota teórica, (c) identificación experimental del umbral de fase (razón cláusulas/variables ≈ 4.26) y discusión de por qué aparece.

**Integra:** MAT-101 (resolución, terminación) + SIS-101 (memoria, contratos) + MAT-104 (análisis de instancias aleatorias).

**Defensa oral.** 20 minutos: justificar el diseño de la estructura de cláusulas, el argumento de terminación y la interpretación del umbral de fase.

---

# CICLO II — Arquitectura, Bajo Nivel y Semántica

**25 créditos · 26 h lectivas/sem · 25 h EI/sem · Total ≈51 h/sem**

> **Propósito del ciclo.** Cerrar la distancia entre el programa escrito y la máquina que lo ejecuta, en las dos direcciones: hacia abajo hasta el transistor y el pipeline, hacia arriba hasta la semántica formal del lenguaje. Es el ciclo que convierte el código en un objeto matemático y en un objeto físico simultáneamente.

---

### SIS-201 — Organización y Arquitectura de Computadoras — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-101 |
| **ADN institucional** | CMU 15-213 / 18-213 — el curso de sistemas más influyente del planeta |

**Competencia terminal.** Predice el rendimiento de un programa desde su patrón de acceso a memoria y desde el comportamiento del pipeline, y explota las consecuencias de una representación mal validada.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Representación de la información | Complemento a dos · Desbordamiento · IEEE 754: precisión simple y doble, NaN, Inf, subnormales · Consecuencias de la no asociatividad del punto flotante |
| 2 | 4–6 | ISA y ensamblador x86-64 | Registros · Modos de direccionamiento · ABI System V · Aritmética, lógica, saltos · Stack frames · Convención de llamadas |
| 3 | 7–9 | Ejecución y pipeline | Etapas IF, ID, EX, MEM, WB · Hazards de datos, estructurales y de control · Forwarding · Predicción de saltos: BTB, tournament predictors · Ejecución especulativa |
| 4 | 10–12 | Jerarquía de memoria | SRAM, DRAM, disco · Localidad espacial y temporal · Caché directa, asociativa por conjuntos, totalmente asociativa · Políticas LRU, LFU, RRIP · NUMA |
| 5 | 13–15 | Optimización guiada por arquitectura | Cache-oblivious algorithms · Blocking y tiling · Prefetching · Medición con `perf` · Memory mountain |

**Laboratorios (los labs canónicos de CMU).** L1 *data lab* · L2 *bomb lab* (desensamblado) · L3 *attack lab* (buffer overflow, ROP) · L4 *cache lab* (simulador + optimización de transposición) · L5 *performance lab*.

**Prueba de Dominio.** *Attack lab* completo (explotación de stack y return-oriented programming) + *cache lab* (simulador de caché e optimización de multiplicación de matrices con maximización medida del hit rate y justificación desde el modelo de jerarquía).

**Bibliografía.**
- **Base:** *Computer Systems: A Programmer's Perspective* (3ª ed., 2016) — Bryant & O'Hallaron · **CSAPP; edición vigente**
- **Complementaria:** *Computer Architecture: A Quantitative Approach* (6ª ed.) — Hennessy & Patterson
- **Papers:** *"What Every Programmer Should Know About Memory"* — Drepper (2007)

**Recursos.** csapp.cs.cmu.edu (labs públicos con autograder local) · Compiler Explorer · `perf`, `valgrind --tool=cachegrind`, Intel VTune.

**Protocolo de estudio.** Asignatura con la mayor densidad de tarjetas de traza: estado de registros y de caché tras N instrucciones. Los labs se atacan sin escribir código el primer día — solo lectura de desensamblado y predicción en papel.

---

### SIS-202 — Circuitos Digitales y Diseño Lógico

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-101 |
| **ADN institucional** | MIT 6.1910 *(ex 6.004)* · CMU 18-240 |

**Competencia terminal.** Sintetiza un procesador funcional desde la especificación de su ISA, con análisis de temporización correcto.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Álgebra de conmutación | Axiomas de Huntington · Formas canónicas · Minimización · Mapas de Karnaugh · Quine-McCluskey |
| 2 | 4–6 | Lógica combinacional | Multiplexores, decodificadores, codificadores · Sumadores: ripple-carry, carry-lookahead · ALU · Análisis de retardo de propagación |
| 3 | 7–9 | Lógica secuencial y FSM | Latches y flip-flops D/JK/T · Máquinas de Moore vs Mealy · Síntesis de FSM · Codificación de estado, one-hot · Metaestabilidad |
| 4 | 10–12 | HDL y flujo de diseño | SystemVerilog: síntesis vs simulación · Testbenches · RTL → síntesis lógica → place-and-route · FPGAs: LUTs, routing |
| 5 | 13–15 | Temporización y microarquitectura | Setup/hold, slack, static timing analysis · Camino crítico · Pipelining del datapath · Forwarding y detección de hazards en hardware |

**Prueba de Dominio.** Procesador RISC-V RV32I en SystemVerilog con pipeline de 5 etapas, forwarding de datos, detección de hazards y predictor de saltos, sintetizable en FPGA, validado contra un banco de pruebas de conformidad de la ISA.

**Bibliografía.**
- **Base:** *Digital Design and Computer Architecture: RISC-V Edition* (2ª ed.) — Harris & Harris
- **Complementaria:** *Computer Organization and Design: RISC-V Edition* — Patterson & Hennessy · *Nand2Tetris* (Nisan & Schocken) como puente conceptual
- **Especificación:** *The RISC-V Instruction Set Manual, Volume I: Unprivileged ISA* (versión ratificada vigente)

**Recursos.** MIT OCW 6.004 · riscv.org (especificaciones oficiales) · Verilator, Icarus Verilog, GTKWave · Ripes (simulador visual de RISC-V) · riscv-tests para conformidad.

**Protocolo de estudio.** Simulación antes de síntesis; testbench antes de diseño. El *waveform* se predice en papel antes de mirarlo — el hábito de leer la forma de onda para descubrir qué hace el circuito impide entenderlo.

---

### LEN-201 — Lenguajes de Programación y Semántica — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 10 · **16 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-101, SIS-101 |
| **ADN institucional** | CMU 15-150, 15-312 · MIT 6.820 |

**Competencia terminal.** Define la semántica de un lenguaje mediante reglas de inferencia y demuestra propiedades de su sistema de tipos.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | λ-cálculo | λ-cálculo sin tipo · Reducción β y η · Confluencia (Church-Rosser) · Normalización · Codificaciones de Church · Punto fijo (Y) |
| 2 | 4–6 | Sistemas de tipos | λ-cálculo tipado simple · Seguridad de tipos: progreso y preservación · Tipos algebraicos (ADTs) · Polimorfismo paramétrico vs ad-hoc · Sistema F |
| 3 | 7–9 | Inferencia de tipos | Hindley-Milner · Unificación · Algoritmo W · Demostración de corrección y completitud · Let-polimorfismo |
| 4 | 10–12 | Semántica formal | Operacional small-step (SOS) y big-step · Denotacional: dominios de Scott, punto fijo de Tarski · Axiomática: lógica de Hoare, correctitud parcial vs total |
| 5 | 13–15 | Efectos y control | Sistemas de efectos · Mónadas · Continuaciones y transformación CPS · Correspondencia de Curry-Howard |

**Prueba de Dominio.** Demostración formal de la correctitud del algoritmo W por inducción estructural sobre derivaciones de tipo + intérprete de λ-cálculo tipado con polimorfismo paramétrico, con verificación experimental de progreso y preservación sobre un banco de programas.

**Bibliografía.**
- **Base:** *Types and Programming Languages* — Pierce (TAPL)
- **Complementaria:** *Practical Foundations for Programming Languages* (2ª ed.) — Harper · *The Formal Semantics of Programming Languages* — Winskel
- **Papers:** *"A Theory of Type Polymorphism in Programming"* — Milner (1978)

**Recursos.** CMU 15-312 notas públicas · *Software Foundations* Vol. 1 (Pierce et al., gratuito) · OCaml o Standard ML como lenguaje de implementación · Redex/PLT para prototipar semánticas.

**Protocolo de estudio.** Las reglas de inferencia se reproducen de memoria en notación de secuentes. Tarjeta estándar de la asignatura: dado un juicio de tipado, reconstruir el árbol de derivación completo.

---

### ALG-201 — Estructuras de Datos Fundamentales — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–2–2 / 9 · **16 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-101, MAT-104, SIS-101 |
| **ADN institucional** | MIT 6.1210 *(ex 6.006)* · CMU 15-210 |

**Competencia terminal.** Deriva cotas amortizadas con función potencial y selecciona estructuras a partir del análisis, no del repertorio memorizado.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Análisis amortizado | Método agregado, del banquero y del potencial · Arrays dinámicos · Contador binario · Tablas dinámicas con contracción |
| 2 | 4–6 | Árboles balanceados | BST · AVL con demostración de altura O(log n) · Rojo-Negro · Rotaciones y aumentación · B-Trees y B+-Trees para disco |
| 3 | 7–9 | Colas de prioridad | Heaps binarios y d-heaps · Fibonacci heaps: análisis amortizado de decrease-key con función potencial · Pairing heaps |
| 4 | 10–12 | Hashing | Encadenamiento vs open addressing · Hashing universal y perfecto · Cuckoo · Robin Hood · Análisis probabilístico de colisiones |
| 5 | 13–15 | Estructuras especializadas | Tries y Patricia tries · Árboles de segmento y Fenwick (BIT) · Disjoint-Set Union con union-by-rank y path compression (inversa de Ackermann) · Skip lists · van Emde Boas |

**Prueba de Dominio.** Demostración formal de que las operaciones de Fibonacci Heap son O(1) amortizado (extract-min O(log n)) mediante función potencial de Fibonacci, e implementación desde cero con medición que contraste la cota amortizada contra el peor caso individual.

**Bibliografía.**
- **Base:** *Introduction to Algorithms* (4ª ed., 2022) — Cormen, Leiserson, Rivest & Stein (CLRS)
- **Complementaria:** *Advanced Data Structures* — Brass · *Purely Functional Data Structures* — Okasaki
- **Papers:** *"Fibonacci Heaps and Their Uses in Improved Network Optimization Algorithms"* — Fredman & Tarjan (JACM 1987)

**Recursos.** MIT OCW 6.006 y 6.851 (Advanced Data Structures, Demaine) · UC Berkeley CS61B · Visualizadores: visualgo.net.

**Protocolo de estudio.** Cada estructura se implementa una vez y se **reimplementa a los 30 días desde cero**, sin mirar la versión previa. La segunda implementación es la que cuenta para la evaluación.

---

### SIS-203 — Arquitectura de Memoria y Almacenamiento

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–0–2 / 9 · **14 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-101 |
| **ADN institucional** | CMU 15-445 (fundamentos de almacenamiento) · Stanford CS145 |

**Competencia terminal.** Diseña la capa de almacenamiento de un sistema con conocimiento explícito del costo real de cada nivel de la jerarquía.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Memoria virtual | Paginación · TLB · Tablas de páginas multinivel (x86-64: PML4) · Segmentación vs paginación · Páginas grandes |
| 2 | 4–6 | Políticas de reemplazo | OPT (Bélády) como cota · LRU, LRU-K, Clock, ARC · Working set theory · Thrashing |
| 3 | 7–9 | Dispositivos | HDD: seek time, latencia rotacional · SSD: NAND, FTL, wear leveling, write amplification · NVMe · Persistent memory |
| 4 | 10–12 | Redundancia y sistemas de archivos | RAID 0/1/5/6 con análisis de MTTF · FAT, ext4, XFS · Journaling · Crash consistency · Log-structured file systems |
| 5 | 13–15 | Buffer pool | Gestión de páginas en memoria · Pinning y latching · Páginas sucias · Políticas de escritura · Prefetching de secuencias |

**Prueba de Dominio.** Buffer pool manager con política LRU-K y extendible hashing para un motor de base de datos minimalista (estilo BusTub, CMU DB Group), evaluado contra trazas reales de acceso y contra la cota OPT.

**Bibliografía.**
- **Base:** *Operating Systems: Three Easy Pieces* — Arpaci-Dusseau & Arpaci-Dusseau (OSTEP, gratuito), partes de virtualización y persistencia
- **Complementaria:** *Database Internals* — Petrov (capítulos de almacenamiento)
- **Papers:** *"The LRU-K Page Replacement Algorithm for Database Disk Buffering"* — O'Neil, O'Neil & Weikum (SIGMOD 1993) · *"ARC: A Self-Tuning, Low Overhead Replacement Cache"* — Megiddo & Modha (FAST 2003)

**Recursos.** pages.cs.wisc.edu/~remzi/OSTEP (libro completo gratuito) · 15445.courses.cs.cmu.edu · fio y blktrace para caracterizar dispositivos reales.

**Protocolo de estudio.** Cada política de reemplazo se evalúa contra una traza real y contra OPT. La métrica es la distancia al óptimo, no el hit rate absoluto: un hit rate alto sobre una traza fácil no dice nada.

---

### INT-200 — Laboratorio Integrador II

| | |
|---|---|
| **Créditos** | 2 |
| **Carga** | 0–0–3 / 5 · **8 h/sem** |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | SIS-201, SIS-202, LEN-201 (concurrentes) |

**Artefacto.** Emulador de CPU RISC-V instrumentado, con: (a) ensamblador propio cuya gramática esté especificada formalmente y su semántica definida con reglas operacionales small-step, (b) modelo de caché configurable integrado, (c) instrumentación que reporte IPC, tasa de fallos de caché y penalización por hazards, (d) un programa de prueba cuyo rendimiento se prediga analíticamente antes de medirlo, con el error de predicción documentado y explicado.

**Integra:** SIS-201 (jerarquía, pipeline) + SIS-202 (datapath) + LEN-201 (semántica operacional del ensamblador) + ALG-201 (estructuras del emulador).

**Defensa oral.** 20 minutos: justificar la discrepancia entre el rendimiento predicho y el medido, atribuyéndola a componentes específicos del modelo.
---

# CICLO III — Teoría de la Computación y Formalismo Matemático

**25 créditos · 25 h lectivas/sem · 27 h EI/sem · Total ≈52 h/sem**

> **Propósito del ciclo.** Establecer qué es computable, qué es tratable y qué es demostrable. Es el ciclo donde el programa deja de construir cosas por un semestre completo y se dedica exclusivamente a demostrar. La densidad demostrativa es máxima; la producción de código, mínima.

---

### TEO-301 — Autómatas, Lenguajes y Computabilidad — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-101 |
| **ADN institucional** | MIT 18.404[J] / 6.5400[J] — el curso de Sipser |

**Competencia terminal.** Demuestra indecidibilidad mediante reducción y determina la clase exacta a la que pertenece un lenguaje dado.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Lenguajes regulares | DFA y NFA · Equivalencia por construcción de subconjuntos · Expresiones regulares y teoremas de Kleene · Minimización (Myhill-Nerode) · Lema del bombeo |
| 2 | 4–6 | Lenguajes libres de contexto | CFG · Formas normales de Chomsky y Greibach · Autómatas de pila deterministas y no deterministas · Lema del bombeo para CFL · Ambigüedad inherente |
| 3 | 7–9 | Máquinas de Turing | Definición y variantes: multitape, no deterministas, con oráculo · Equivalencia de modelos · Tesis de Church-Turing · Máquina universal |
| 4 | 10–12 | Decidibilidad | Lenguajes decidibles vs reconocibles · Problema de la parada por diagonalización · Reducciones many-one · Teorema de Rice |
| 5 | 13–15 | Indecidibilidad avanzada | Post Correspondence Problem · Indecidibilidad en gramáticas · Grado de Turing · Jerarquía aritmética (introducción) |

**Prueba de Dominio.** Demostración completa y encadenada de: (a) indecidibilidad del Problema de la Parada por diagonalización, (b) Teorema de Rice desde la reducción al Halting Problem, (c) indecidibilidad del PCP. Cada reducción presentada con la dirección justificada explícitamente.

**Bibliografía.**
- **Base:** *Introduction to the Theory of Computation* (3ª ed.) — Sipser
- **Complementaria:** *Introduction to Automata Theory, Languages, and Computation* — Hopcroft, Motwani & Ullman
- **Papers:** *"On Computable Numbers, with an Application to the Entscheidungsproblem"* — Turing (1936)

**Recursos.** MIT OCW 18.404J (video completo, Sipser) · Automata Tutor (verificación automática de construcciones) · JFLAP.

**Protocolo de estudio.** Las reducciones se practican en dirección inversa: dado el resultado, reconstruir qué se reduce a qué y por qué esa dirección y no la contraria. Invertir la dirección de la reducción es el error más frecuente y el más caro de la asignatura.

---

### TEO-302 — Teoría de la Complejidad Computacional — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 12 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | TEO-301 (concurrente permitido) |
| **ADN institucional** | UC Berkeley CS172 · MIT 6.1400[J] *(ex 6.045)* · MIT 6.5400 |

**Competencia terminal.** Clasifica problemas en clases de complejidad mediante reducción y distingue con precisión lo demostrado de lo conjeturado.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Clases de tiempo y espacio | TIME(f), SPACE(f) · P, NP, co-NP, PSPACE, EXPTIME · Definición por certificado y por máquina no determinista · Teoremas de jerarquía de tiempo y espacio |
| 2 | 4–6 | NP-completitud | Reducciones polinomiales (≤ₚ) · Teorema de Cook-Levin con demostración completa · Cadena canónica: SAT → 3-SAT → Clique → Independent Set → Vertex Cover → Hamiltonian Path |
| 3 | 7–9 | Espacio | Teorema de Savitch: NSPACE(f) ⊆ SPACE(f²) · Teorema de Immerman-Szelepcsényi · PSPACE-completitud: QBF/TQBF · L, NL y NL-completitud |
| 4 | 10–12 | Aleatoriedad y circuitos | BPP, RP, co-RP, ZPP · Teorema de Adleman: BPP ⊆ P/poly · Circuitos booleanos: tamaño y profundidad · NC y AC · Teorema de Valiant |
| 5 | 13–15 | Más allá de NP | Jerarquía polinomial · #P y Teorema de Toda · Complejidad de comunicación · Complejidad de consultas: certificado, sensibilidad, grado |

**Prueba de Dominio.** Demostración de Cook-Levin desde la codificación del cómputo como fórmula + demostración del Teorema de Savitch + construcción de la jerarquía polinomial mediante oráculos y análisis de su relación con P vs NP (incluyendo por qué la relativización obstruye ciertas técnicas de prueba).

**Bibliografía.**
- **Base:** *Computational Complexity: A Modern Approach* — Arora & Barak
- **Complementaria:** *Computational Complexity* — Papadimitriou · *The Nature of Computation* — Moore & Mertens
- **Papers:** *"The Complexity of Theorem-Proving Procedures"* — Cook (STOC 1971) · *"Relativizations of the P =? NP Question"* — Baker, Gill & Solovay (1975)

**Recursos.** Arora & Barak (borrador gratuito en la web de Princeton) · Complexity Zoo · Berkeley CS172 notes.

**Protocolo de estudio.** Mapa de clases dibujado de memoria cada semana, con las inclusiones **conocidas** en trazo continuo y las **conjeturadas** en trazo punteado. Confundir ambas es el fallo conceptual central de la asignatura y la causa de argumentos circulares en los exámenes.

---

### MAT-301 — Teoría de Grafos y Combinatoria Avanzada

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-101, MAT-104 |
| **ADN institucional** | MIT 18.217 · CMU 21-701 |

**Competencia terminal.** Aplica el método probabilístico para demostrar existencia y deriva cotas exactas sobre estructuras combinatorias.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Conectividad y flujo | Teorema de Menger · Flujo máximo: Ford-Fulkerson, Edmonds-Karp, Push-Relabel · Algoritmo de Dinic con análisis exacto O(V²E) por grafos de nivel · Max-flow min-cut |
| 2 | 4–6 | Emparejamiento | Bipartito: teorema de Hall, Hopcroft-Karp O(E√V) · Emparejamiento general: algoritmo blossom de Edmonds · Teorema de Tutte |
| 3 | 7–9 | Coloración y planaridad | Número cromático · Cota de Brooks · Teorema de Vizing · Coloración de listas · Planaridad: Kuratowski-Wagner · Boyer-Myrvold · Genus y grafos en superficies |
| 4 | 10–12 | Método probabilístico | Primer y segundo momento · Lovász Local Lemma simétrico y asimétrico · Desaleatorización · Números de Ramsey · Cotas por conteo |
| 5 | 13–15 | Estructuras avanzadas | Grafos expanders: expansión de arista y de vértice, gap espectral · Polinomio de Tutte · Matroides: definición axiomática, teorema del greedy · Teorema de Szemerédi (enunciado) |

**Prueba de Dominio.** Demostración del Lovász Local Lemma en sus versiones simétrica y asimétrica, con aplicación a coloración de hipergrafos + demostración de que el algoritmo de Dinic es O(V²E) mediante análisis de fases con grafos de nivel.

**Bibliografía.**
- **Base:** *Graph Theory* (5ª ed.) — Diestel (gratuito para lectura en línea)
- **Complementaria:** *The Probabilistic Method* — Alon & Spencer · *Modern Graph Theory* — Bollobás
- **Papers:** *"A Constructive Proof of the General Lovász Local Lemma"* — Moser & Tardos (JACM 2010)

**Recursos.** diestel-graph-theory.com · MIT OCW 18.217 · NetworkX y SageMath para verificar construcciones sobre instancias pequeñas.

**Protocolo de estudio.** El método probabilístico se practica en formato "existencia sin construcción": demostrar que existe, luego intentar construirlo explícitamente y fracasar conscientemente. Esa asimetría entre existencia y construcción es el contenido real de la unidad 4.

---

### MAT-302 — Álgebra Abstracta para Computación

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-101 |
| **ADN institucional** | MIT 18.703 · UC Berkeley Math 113 |

**Competencia terminal.** Construye y opera en cuerpos finitos, y reconoce la estructura algebraica que subyace a un esquema criptográfico o a un código corrector.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Grupos | Axiomas, subgrupos, cocientes · Homomorfismos · Teoremas de isomorfía · Teorema de Lagrange · Grupos cíclicos |
| 2 | 4–6 | Acciones y permutaciones | Teorema de Cayley · Órbitas y estabilizadores · Lema de Burnside · Enumeración de Pólya · Grupos de simetría |
| 3 | 7–9 | Anillos | Dominio íntegro · Ideales y cocientes · Anillos de polinomios · Aritmética en ℤ/nℤ · φ de Euler · Pequeño teorema de Fermat |
| 4 | 10–12 | Cuerpos finitos | GF(p) y GF(pⁿ) · Polinomios irreducibles · Construcción de GF(2ⁿ) · Elemento primitivo · Aplicación a AES (MixColumns) y a Reed-Solomon |
| 5 | 13–15 | Galois y representaciones | Extensiones de cuerpos · Grupo de Galois · Correspondencia de Galois · Teoría de representaciones: Maschke, caracteres · Transformada de Fourier sobre grupos finitos |

**Prueba de Dominio.** Construcción formal de GF(2⁸) con aritmética de polinomios irreducibles, e implementación de MixColumns de AES verificada contra los vectores de prueba de FIPS 197 + demostración de que el orden del grupo de Galois de una extensión finita es igual a su grado sobre el cuerpo base.

**Bibliografía.**
- **Base:** *Abstract Algebra* (3ª ed.) — Dummit & Foote
- **Complementaria:** *Algebra* — Artin · *A Computational Introduction to Number Theory and Algebra* — Shoup (gratuito)
- **Estándar:** FIPS 197 (especificación de AES)

**Recursos.** shoup.net/ntb (libro completo gratuito) · SageMath para aritmética en cuerpos finitos · MIT OCW 18.703.

**Protocolo de estudio.** Cada estructura abstracta se ancla en dos instancias concretas: una criptográfica (que reaparece en SEG-701) y una de códigos (que reaparece en TEO-401). Sin el anclaje, el material no transfiere y se olvida entre ciclos.

---

### TEO-303 — Lógica Matemática y Teoría de Modelos

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-101 |
| **ADN institucional** | UC Berkeley Math 125A · MIT 18.510 |

**Competencia terminal.** Sostiene la distinción entre sintaxis y semántica en toda argumentación formal, y demuestra los teoremas límite de la lógica de primer orden.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Sistemas formales | Sintaxis y semántica · Satisfacibilidad y validez · Deducción (⊢) vs consecuencia semántica (⊨) · Sistemas de Hilbert vs deducción natural |
| 2 | 4–6 | Completitud y compacidad | Teorema de Completitud de Gödel (1930) · Teorema de Compacidad y consecuencias · Löwenheim-Skolem hacia abajo y hacia arriba · Paradoja de Skolem |
| 3 | 7–9 | Incompletitud | Numeración de Gödel · Aritmetización de la sintaxis · Primer Teorema de Incompletitud · Segundo Teorema · Teorema de Tarski sobre indefinibilidad de la verdad |
| 4 | 10–12 | Automatización | Teorema de Herbrand · Forma normal de Skolem · Resolución de primer orden y su completitud (Robinson) · Unificación |
| 5 | 13–15 | Teoría de modelos y lógicas no clásicas | Isomorfismo, subestructuras, ultrapotencias · Teorema de Łoś-Tarski · Tipos y espacios de tipos · Lógica modal · LTL y CTL · Model checking: algoritmo de Tarjan |

**Prueba de Dominio.** Demostración del Primer Teorema de Incompletitud mediante construcción explícita de la sentencia de Gödel y aritmetización de la sintaxis + formalización del Teorema de Completitud de primer orden, con discusión de por qué ambos resultados no se contradicen.

**Bibliografía.**
- **Base:** *Mathematical Logic* — Ebbinghaus, Flum & Thomas
- **Complementaria:** *Gödel's Incompleteness Theorems* — Smullyan · *A Mathematical Introduction to Logic* — Enderton · *Model Theory* — Chang & Keisler
- **Papers:** *"Über formal unentscheidbare Sätze..."* — Gödel (1931), en traducción anotada

**Recursos.** Berkeley Math 125A notes · *Logic and Proof* (Avigad et al., con Lean 4) · Prover9/Mace4 para experimentar con resolución.

**Protocolo de estudio.** La distinción ⊢ / ⊨ se sostiene explícitamente en cada tarjeta y en cada línea de cada demostración. El colapso de esa distinción es el fallo universal en esta asignatura y produce demostraciones que parecen correctas y no lo son.

---

### INT-300 — Laboratorio Integrador III

| | |
|---|---|
| **Créditos** | 2 |
| **Carga** | 0–0–3 / 5 · **8 h/sem** |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | TEO-301, TEO-302, MAT-301 (concurrentes) |

**Artefacto.** Documento formal de 15–25 páginas con una cadena de reducciones verificada de extremo a extremo: desde un problema combinatorio natural (elegido de MAT-301) hasta 3-SAT, y desde ahí hasta un lenguaje indecidible. Requisitos: (a) cada paso con la dirección de la reducción justificada, (b) análisis de qué se preserva y qué se pierde en cada reducción, (c) identificación del punto exacto donde cada reducción deja de funcionar si se debilita una hipótesis, (d) implementación ejecutable de al menos dos de las reducciones, con verificación sobre instancias.

**Integra:** TEO-301 (reducciones de decidibilidad) + TEO-302 (reducciones polinomiales) + MAT-301 (el problema fuente) + TEO-303 (rigor de la formalización).

**Defensa oral.** 25 minutos en pizarra: reconstruir dos reducciones de la cadena sin apuntes y responder a un ataque del comité sobre una hipótesis debilitada.

---

# CICLO IV — Algoritmos, Optimización y Teoría de la Información

**25 créditos · 25 h lectivas/sem · 27 h EI/sem · Total ≈52 h/sem**

> **Propósito del ciclo.** Convertir el aparato teórico del ciclo III en capacidad de diseño. Es el ciclo bisagra: entra teoría pura y sale la habilidad de producir algoritmos con cotas demostradas, que es el requisito de entrada de todo lo que viene después.

---

### ALG-401 — Diseño y Análisis de Algoritmos — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ALG-201, MAT-104 |
| **ADN institucional** | MIT 6.1220[J] / 18.410[J] *(ex 6.046)* |

**Competencia terminal.** Diseña un algoritmo para un problema no visto, enuncia su invariante, demuestra su correctitud y deriva su complejidad exacta.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Divide y vencerás | Recurrencias · Teorema Maestro con demostración · Método de Akra-Bazzi · Mergesort, heapsort · Cota inferior Ω(n log n) por árbol de decisión · Selección determinista |
| 2 | 4–6 | Programación dinámica | Subestructura óptima · Solapamiento de subproblemas · Memoización vs bottom-up · LCS, LIS, Edit Distance, Knapsack, Matrix Chain · Reconstrucción de la solución |
| 3 | 7–9 | Greedy y matroides | Correctitud por exchange argument · Matroides y el teorema del greedy · Huffman · Scheduling · Cuándo greedy falla y por qué |
| 4 | 10–12 | Algoritmos de grafos | Dijkstra con Fibonacci heaps O(E + V log V) · Bellman-Ford · Floyd-Warshall · MST: Kruskal con DSU, Prim · SCC: Tarjan, Kosaraju · Flujo y matching |
| 5 | 13–15 | Geometría y cadenas | Convex hull: Graham, Jarvis · Intersección de segmentos por sweep line · KMP, Z-algorithm, Aho-Corasick · Suffix arrays y suffix trees |

**Prueba de Dominio.** Demostración de correctitud de Dijkstra mediante invariante de bucle, con análisis exacto usando Fibonacci heaps + demostración de que Knapsack 0/1 no admite solución greedy pero la versión fraccionada sí, con el exchange argument explícito y el contraejemplo mínimo para la versión entera.

**Bibliografía.**
- **Base:** CLRS (4ª ed.) + *Algorithm Design* — Kleinberg & Tardos
- **Complementaria:** *Algorithms* — Dasgupta, Papadimitriou & Vazirani (gratuito) · *Competitive Programming* — Halim (para volumen de práctica)
- **Papers:** —

**Recursos.** MIT OCW 6.046J · Stanford Algorithms Specialization (Roughgarden) · Codeforces y AtCoder para práctica cronometrada · Stanford CS161.

**Protocolo de estudio.** Formato de tarjeta canónico: problema → **invariante**, nunca problema → pseudocódigo. Un algoritmo memorizado sin su invariante no está aprendido. Práctica diaria obligatoria: un problema no visto, cronometrado a 45 minutos.

---

### ALG-402 — Algoritmos Avanzados y Geometría Computacional

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 12 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ALG-401 (concurrente permitido) |
| **ADN institucional** | MIT 6.5210[J] / 18.415[J] *(ex 6.854, Karger)* · Stanford CS261 |

**Competencia terminal.** Deriva razones de aproximación ajustadas y construye la instancia que las alcanza.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Flujo avanzado y LP | Scaling algorithms · Min-cost flow · Programación lineal: simplex, dualidad débil y fuerte · Teorema de Farkas · Método del elipsoide · Relajaciones LP con redondeo |
| 2 | 4–6 | Aproximación | Razón de aproximación · PTAS y FPTAS · Set Cover greedy con cota ln(n) e instancia ajustada · Vertex Cover 2-aproximación · Christofides (3/2) para TSP métrico · Relajaciones SDP: Goemans-Williamson |
| 3 | 7–9 | Aleatorización y online | Fingerprinting · Freivalds · Karger min-cut con análisis de probabilidad de éxito · Análisis competitivo · Método del potencial · Problema del k-servidor · Paging online |
| 4 | 10–12 | Geometría computacional | Triangulación · Diagramas de Voronoi (algoritmo de Fortune) · Delaunay · Sweep line · Intersección de semiplanos · Búsqueda de rango |
| 5 | 13–15 | Memoria externa y cadenas | External memory: B-trees, sorting, scanning · Cache-oblivious: multiplicación de matrices, funnelsort · Suffix arrays con SA-IS · FM-index · Compresión con Burrows-Wheeler |

**Prueba de Dominio.** Implementación del algoritmo de Karger con análisis riguroso de la probabilidad de éxito y del número de repeticiones necesarias + demostración de la dualidad fuerte de la programación lineal mediante el Teorema de Farkas.

**Bibliografía.**
- **Base:** *Randomized Algorithms* — Motwani & Raghavan
- **Complementaria:** *The Design of Approximation Algorithms* — Williamson & Shmoys (gratuito) · *Computational Geometry: Algorithms and Applications* — de Berg et al. · *Approximation Algorithms* — Vazirani
- **Papers:** *"Improved Approximation Algorithms for Maximum Cut..."* — Goemans & Williamson (JACM 1995) · *"Global Min-cuts in RNC..."* — Karger & Stein

**Recursos.** designofapproxalgs.com (libro gratuito) · MIT 6.5210 (notas de Karger) · Stanford CS261 · CGAL para contrastar implementaciones geométricas.

**Protocolo de estudio.** Para cada algoritmo de aproximación se construye la instancia que alcanza la cota ajustada. Sin esa instancia, la cota es un número memorizado y no se entiende por qué el algoritmo no puede hacerlo mejor.

---

### MAT-401 — Álgebra Lineal Numérica y Optimización — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-102, MAT-103 |
| **ADN institucional** | Stanford EE364A/B (Boyd) · MIT 18.085 |

**Competencia terminal.** Reconoce convexidad, formula el dual de un problema y deriva la tasa de convergencia de un método de primer orden.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Convexidad | Conjuntos y funciones convexas · Operaciones que preservan convexidad · Funciones conjugadas · Reconocimiento de problemas convexos disfrazados |
| 2 | 4–6 | Dualidad | Dualidad de Lagrange · Gap de dualidad · Dualidad fuerte y condición de Slater · Condiciones KKT · Complementary slackness · Interpretación económica |
| 3 | 7–9 | Métodos de primer orden | Descenso de gradiente: convergencia para funciones L-suaves y μ-fuertemente convexas · Momentum · Nesterov con análisis O(1/k²) · Descenso de coordenadas · Métodos proximales |
| 4 | 10–12 | Métodos de segundo orden e interior | Newton: convergencia cuadrática local · Cuasi-Newton (BFGS) · Barrera logarítmica · Punto interior primal-dual · Complejidad de iteración |
| 5 | 13–15 | Optimización estocástica y no suave | SGD: convergencia en esperanza · Varianza reducida (SVRG) · Norma-1: LASSO, Basis Pursuit · Subgradiente · Min-max y teorema minimax · Relajaciones LP/SDP en optimización combinatoria |

**Prueba de Dominio.** Demostración de que el método acelerado de Nesterov logra O(1/k²) frente a O(1/k) del gradiente estándar + implementación de un solver de programación cuadrática con restricciones de igualdad mediante multiplicadores de Lagrange, validado contra CVXPY.

**Bibliografía.**
- **Base:** *Convex Optimization* — Boyd & Vandenberghe (gratuito)
- **Complementaria:** *Numerical Optimization* — Nocedal & Wright · *Lectures on Convex Optimization* — Nesterov · *First-Order Methods in Optimization* — Beck
- **Papers:** —

**Recursos.** web.stanford.edu/~boyd/cvxbook (libro + slides + video de EE364A) · CVXPY · MOSEK/ECOS para contrastar.

**Protocolo de estudio.** Asignatura puente hacia el ciclo VI. Cada resultado se etiqueta al aprenderlo con dónde reaparece en aprendizaje automático: KKT→SVM, dualidad→kernel trick, SGD→entrenamiento de redes. El etiquetado se hace ahora, no al llegar al ciclo VI.

---

### ALG-403 — Computación Paralela y Distribuida

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | ALG-201, SIS-201 |
| **ADN institucional** | CMU 15-210 · Stanford CS149 · MIT 6.106 *(ex 6.172)* |

**Competencia terminal.** Analiza un algoritmo paralelo en términos de trabajo y span, y demuestra la linearizabilidad de una estructura concurrente.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelos de cómputo paralelo | PRAM: EREW, CREW, CRCW y simulaciones mutuas · Modelo Work-Span (Cilk) · Ley de Brent · Paralelismo = W/S · Amdahl y Gustafson |
| 2 | 4–6 | Algoritmos paralelos | Prefix sums (scan) · Mergesort paralelo · List ranking · BFS paralelo (PBFS) · Redes de ordenamiento: Batcher bitonic |
| 3 | 7–9 | Arquitectura de memoria compartida | UMA vs NUMA · Coherencia de caché: MSI, MESI, MOESI · False sharing y padding · Modelos de consistencia: sequential consistency, TSO, release consistency |
| 4 | 10–12 | Sincronización | Mutexes, semáforos, barreras, variables de condición · Lock-free y wait-free · CAS, LL/SC · ABA problem · Memoria transaccional: STM, HTM |
| 5 | 13–15 | Planificación y GPU | Work-stealing scheduler y su cota · OpenMP · Modelo de ejecución GPU: warps, divergencia, ocupancia · Introducción a CUDA |

**Prueba de Dominio.** Suma de prefijos paralela con análisis exacto de W(n) = O(n) y S(n) = O(log n), verificado por medición de escalabilidad + cola MPMC lock-free con demostración de linearizabilidad y con banco de pruebas de estrés bajo reordenamiento de memoria.

**Bibliografía.**
- **Base:** *The Art of Multiprocessor Programming* (2ª ed.) — Herlihy, Shavit, Luchangco & Spear
- **Complementaria:** *Introduction to Parallel Computing* — Kumar et al. · *Structured Parallel Programming* — McCool, Reinders & Robison
- **Papers:** *"Scheduling Multithreaded Computations by Work Stealing"* — Blumofe & Leiserson (JACM 1999) · *"Linearizability: A Correctness Condition for Concurrent Objects"* — Herlihy & Wing (TOPLAS 1990)

**Recursos.** CMU 15-210 · Stanford CS149 · MIT 6.106 · ThreadSanitizer, `perf`, Intel Inspector · Cilk / OpenCilk.

**Protocolo de estudio.** Todo argumento de correctitud concurrente se escribe primero como historia de ejecución con entrelazado explícito, antes de codificar. Los bugs de concurrencia no se depuran: se previenen en la especificación, porque no son reproducibles.

---

### TEO-401 — Teoría de la Información y Códigos

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-104, MAT-302 |
| **ADN institucional** | MIT 6.441[J] · Stanford EE376A |

**Competencia terminal.** Deriva la capacidad de un canal y construye códigos que se aproximen a ella, cuantificando la brecha.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Medidas de información | Entropía H(X) · Entropía conjunta y condicional · Información mutua I(X;Y) · Divergencia KL · Desigualdad de procesamiento de datos · Desigualdad de Fano |
| 2 | 4–6 | Codificación de fuente | Códigos de prefijo · Desigualdad de Kraft · Huffman y su optimalidad · Codificación aritmética · Primer Teorema de Shannon · AEP y conjuntos típicos |
| 3 | 7–9 | Capacidad de canal | Definición C = max I(X;Y) · Canal simétrico binario · Segundo Teorema de Shannon con demostración por codificación aleatoria · Recíproco · Canal gaussiano: C = ½ log(1+SNR) |
| 4 | 10–12 | Códigos correctores | Distancia de Hamming · Cotas: Singleton, Hamming, Gilbert-Varshamov · Códigos lineales: matriz generadora y de paridad, código dual · Códigos cíclicos: BCH · Reed-Solomon sobre GF(2ⁿ) |
| 5 | 13–15 | Códigos modernos y complejidad | LDPC y sum-product (belief propagation) · Códigos polares (introducción) · Teorema de Slepian-Wolf · Complejidad de Kolmogorov · MDL · Incompresibilidad y su uso como método de prueba |

**Prueba de Dominio.** Demostración completa del Teorema de Codificación de Canal (existencia de códigos aleatorios que alcanzan la capacidad) + implementación de codificador y decodificador Reed-Solomon con el algoritmo de Berlekamp-Welch, medido sobre canal simulado con la brecha respecto a la capacidad cuantificada.

**Bibliografía.**
- **Base:** *Elements of Information Theory* (2ª ed.) — Cover & Thomas
- **Complementaria:** *Information Theory, Inference, and Learning Algorithms* — MacKay (gratuito) · *Essential Coding Theory* — Guruswami, Rudra & Sudan (borrador gratuito)
- **Papers:** *"A Mathematical Theory of Communication"* — Shannon (Bell System Technical Journal, 1948)

**Recursos.** inference.org.uk/mackay/itila (MacKay completo, gratuito) · Stanford EE376A · Galois field libraries para validar la aritmética de MAT-302.

**Protocolo de estudio.** Las cotas de Shannon se contrastan siempre contra códigos reales implementados. La brecha entre cota y práctica es el objeto de estudio de la unidad 5, no un defecto de la implementación.

---

### INT-400 — Laboratorio Integrador IV

| | |
|---|---|
| **Créditos** | 2 |
| **Carga** | 0–0–3 / 5 · **8 h/sem** |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | ALG-403, TEO-401, MAT-302 (concurrentes) |

**Artefacto.** Codificador/decodificador Reed-Solomon paralelizado, con: (a) aritmética de GF(2⁸) implementada desde la construcción algebraica de MAT-302, (b) paralelización con análisis exacto de trabajo y span según ALG-403, (c) medición de escalabilidad contra la predicción de la ley de Brent, con la discrepancia atribuida a componentes específicos (contención, false sharing, overhead de planificación), (d) verificación de la tasa de corrección contra la cota de Singleton sobre canal simulado.

**Integra:** MAT-302 (cuerpos finitos) + TEO-401 (códigos y capacidad) + ALG-403 (paralelismo y análisis W/S) + ALG-401 (análisis de complejidad).

**Defensa oral.** 20 minutos: explicar por qué la escalabilidad medida se desvía de la predicción teórica, con evidencia de perfilado.
---

# CICLO V — Sistemas Complejos: SO, Compiladores, Redes y Bases de Datos

**25 créditos · 26 h lectivas/sem · 28 h EI/sem · Total ≈54 h/sem**

> **Propósito del ciclo.** El ciclo de mayor carga de construcción del programa. Cuatro sistemas completos se escriben desde cero en paralelo, y una asignatura de métodos formales verifica propiedades de los otros tres. Aquí la malla deja de ser asignaturas paralelas y se convierte en una pila: el compilador genera código para el kernel, y el verificador demuestra que el planificador no bloquea.

---

### SIS-501 — Sistemas Operativos Internos — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 12 · **19 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-201, SIS-203, ALG-403 |
| **ADN institucional** | CMU 15-410 · MIT 6.1810 *(ex 6.S081 / 6.828)* |

**Competencia terminal.** Construye un núcleo funcional con planificación, memoria virtual y sistema de archivos, y razona sobre sus propiedades de seguridad y ausencia de bloqueo.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Procesos y arranque | Arranque y modo protegido · PCB · Cambio de contexto · ABI de llamadas al sistema · Trampas, interrupciones y excepciones |
| 2 | 4–6 | Planificación | FCFS, SJF, Round Robin · CFS/EEVDF de Linux · Prioridades e inversión de prioridad · Métricas: utilización, throughput, turnaround, equidad · Planificación en multiprocesador |
| 3 | 7–9 | Concurrencia en el núcleo | Semáforos, mutex, monitores, variables de condición · Condiciones de Coffman · Detección por grafo de recursos · Prevención · Algoritmo del banquero · Bloqueo en vivo |
| 4 | 10–12 | Memoria virtual | Paginación y tablas multinivel · Manejo de fallos de página · Demand paging y swap · mmap · Copy-on-write · TLB shootdown en SMP |
| 5 | 13–15 | Persistencia y aislamiento | VFS · Inodos · Journaling ext4 · Crash consistency · io_uring y epoll · Drivers: interrupciones y DMA · Anillos de privilegio x86 · seccomp-bpf, namespaces, cgroups |

**Laboratorios.** L1 llamadas al sistema · L2 planificador · L3 paginación · L4 copy-on-write fork · L5 hilos a nivel de usuario · L6 sistema de archivos · L7 red o mmap.

**Prueba de Dominio.** Núcleo minimalista completo (base xv6 o PintOS) con: planificador de hilos reales, memoria virtual con paginación y COW, y sistema de archivos con journaling. Sometido a inyección de fallos por corte de energía simulado en punto arbitrario, con análisis formal de ausencia de deadlock en la jerarquía de bloqueos.

**Bibliografía.**
- **Base:** *Operating Systems: Three Easy Pieces* — Arpaci-Dusseau & Arpaci-Dusseau (gratuito) + código fuente comentado de xv6
- **Complementaria:** *Lions' Commentary on UNIX 6th Edition* · *Understanding the Linux Kernel* — Bovet & Cesati · *Operating Systems: Principles and Practice* — Anderson & Dahlin
- **Papers:** *"The UNIX Time-Sharing System"* — Ritchie & Thompson (CACM 1974)

**Recursos.** pdos.csail.mit.edu/6.828 (xv6 + labs completos) · pages.cs.wisc.edu/~remzi/OSTEP · QEMU + GDB para depuración de núcleo · CMU 15-410 (PintOS).

**Protocolo de estudio.** La asignatura de mayor carga cognitiva del programa. Regla estricta: **un subsistema por semana**, con la especificación escrita antes del código. Nunca depurar dos subsistemas simultáneamente — en un núcleo, dos bugs simultáneos producen síntomas que no corresponden a ninguno de los dos.

---

### LEN-501 — Diseño de Compiladores — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | LEN-201, TEO-301, SIS-201 |
| **ADN institucional** | Stanford CS143 · CMU 15-411 |

**Competencia terminal.** Construye un compilador completo con optimizaciones que preservan la semántica demostrablemente.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Análisis léxico y sintáctico | Regex → NFA (Thompson) → DFA (construcción de subconjuntos) · Gramáticas LL(1) · LR(0), SLR(1), LALR(1), LR(1) · Construcción de tablas · Recuperación de errores |
| 2 | 4–6 | Análisis semántico | AST · Tabla de símbolos y ámbitos · Sistemas de tipos · Chequeo e inferencia (algoritmo W de LEN-201) · Errores semánticos |
| 3 | 7–9 | Representación intermedia | IR de tres direcciones · SSA · Dominadores y fronteras de dominancia · Inserción de funciones φ · Salida de SSA |
| 4 | 10–12 | Análisis y optimización | Dataflow: reaching definitions, live variables, available expressions · Retículo y punto fijo · Eliminación de código muerto · Propagación de constantes y de copias · LICM · Análisis de variables de inducción · Desenrollado · Análisis de alias: Andersen vs Steensgaard |
| 5 | 13–15 | Generación de código | Selección de instrucciones · Asignación de registros por coloración de grafos de interferencia · Spilling · Convenciones de llamada x86-64 · Planificación de instrucciones · Peephole · SIMD |

**Prueba de Dominio.** Compilador completo y funcional desde un lenguaje tipo C simplificado hasta x86-64, con: análisis léxico, parsing LALR(1), inferencia de tipos, representación SSA, al menos cuatro optimizaciones dataflow y asignación de registros por coloración. Cada optimización acompañada de un test de regresión que falla si la optimización rompe la semántica.

**Bibliografía.**
- **Base:** *Engineering a Compiler* (3ª ed., 2022) — Cooper & Torczon
- **Complementaria:** *Modern Compiler Implementation in ML* — Appel · *Compilers: Principles, Techniques, and Tools* — Aho, Lam, Sethi & Ullman (el "dragon book") · *SSA-based Compiler Design* — Rastello & Bouchez (gratuito)
- **Papers:** *"Efficiently Computing Static Single Assignment Form and the Control Dependence Graph"* — Cytron et al. (TOPLAS 1991)

**Recursos.** web.stanford.edu/class/cs143 · CMU 15-411 · LLVM (documentación de IR y de pases) · Compiler Explorer · Alive2 para verificar que una optimización preserva semántica.

**Protocolo de estudio.** La suite de regresión se escribe **antes** que la optimización. Toda optimización aceptada sin test que la contradiga es una fuente de bugs que aparecerán a diez pases de distancia.

---

### SIS-502 — Redes de Computadoras: Protocolos y Arquitectura

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-201, MAT-104 |
| **ADN institucional** | Stanford CS144 · MIT 6.829 |

**Competencia terminal.** Implementa una pila de protocolos desde la especificación y razona sobre control de congestión con modelos analíticos.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Capas física y enlace | Codificación Manchester, 4B5B · Modulación · Ethernet: CSMA/CD, exponential backoff con análisis de carga · Switching · STP · VLAN |
| 2 | 4–6 | Capa de red | IPv4 e IPv6 · CIDR y agregación · Fragmentación · TTL · NAT · ICMP · Forwarding vs routing |
| 3 | 7–9 | Enrutamiento | RIP como Bellman-Ford distribuido · OSPF como Dijkstra distribuido · BGP como path vector · Políticas y estabilidad · Convergencia y bucles transitorios |
| 4 | 10–12 | Transporte | Máquina de estados completa de TCP · Three-way handshake · Control de flujo por ventana deslizante · Control de congestión: AIMD, slow start, congestion avoidance, CUBIC, BBR · Modelo analítico de throughput de TCP · UDP |
| 5 | 13–15 | Aplicación y seguridad de transporte | DNS: jerarquía, resolución iterativa vs recursiva, caché · HTTP/1.1, HTTP/2 con HPACK, HTTP/3 sobre QUIC · TLS 1.3: handshake, ECDHE · SDN y OpenFlow · DHT (Kademlia), BitTorrent |

**Prueba de Dominio.** Router IP con tabla de enrutamiento y plano de forwarding + implementación de TCP sobre UDP en espacio de usuario, con control de congestión AIMD, retransmisión con estimación adaptativa de RTT y detección de pérdidas. Evaluado bajo pérdida, reordenamiento y latencia variable inyectadas.

**Bibliografía.**
- **Base:** *Computer Networks: A Top-Down Approach* (8ª ed.) — Kurose & Ross
- **Complementaria:** *Computer Networks: A Systems Approach* — Peterson & Davie (gratuito) · *TCP/IP Illustrated, Vol. 1* — Fall & Stevens
- **Papers:** *"Congestion Avoidance and Control"* — Jacobson & Karels (SIGCOMM 1988) · *"BBR: Congestion-Based Congestion Control"* — Cardwell et al. (ACM Queue 2016)

**Recursos.** cs144.github.io (labs completos de construcción de TCP) · systemsapproach.org (libro gratuito) · Wireshark · mininet · RFCs 793, 9293, 9000 (QUIC), 8446 (TLS 1.3).

**Protocolo de estudio.** Toda máquina de estados se dibuja de memoria antes de implementarla. La captura con Wireshark se contrasta siempre contra la predicción hecha leyendo el RFC — nunca al revés.

---

### SIS-503 — Bases de Datos: Motores e Internals — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-203, ALG-201 |
| **ADN institucional** | CMU 15-445 / 645 (Andrew Pavlo) |

**Competencia terminal.** Construye un motor relacional transaccional con recuperación ante fallos y control de concurrencia demostrablemente serializable.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelo y almacenamiento | Álgebra relacional · Cálculo relacional de tuplas y de dominio · Formato de página y de tupla · Almacenamiento por filas vs por columnas · Compresión |
| 2 | 4–6 | Índices | B+-Trees: estructura, división, fusión, concurrencia por latch crabbing · Hash extensible y lineal · LSM-trees y estrategias de compactación · Índices de cobertura |
| 3 | 7–9 | Ejecución de consultas | Modelo Volcano de iteradores · Ejecución vectorizada · Joins: Nested Loop, Block Nested Loop, Sort-Merge con análisis exacto de I/O, Hash Join (Grace, Hybrid) · Agregación y ordenamiento externos |
| 4 | 10–12 | Optimización | Estimación de cardinalidad · Histogramas y sketches · Estadísticas · Optimización basada en costos (Selinger, System R) · Reordenamiento de joins · Materialización tardía |
| 5 | 13–15 | Transacciones y recuperación | ACID · 2PL y 2PL estricto · Detección y prevención de deadlock · Niveles de aislamiento · Snapshot isolation y sus anomalías (write skew) · MVCC · WAL · ARIES: Analysis, Redo, Undo |

**Prueba de Dominio.** Motor de base de datos completo desde cero (referencia: BusTub de CMU) con buffer pool manager, tabla hash extensible, índice B+Tree concurrente, motor de ejecución con join y agregación, control de concurrencia por 2PL y recuperación ARIES. Validado con inyección de crash en punto arbitrario y verificación de serializabilidad sobre historias generadas.

**Bibliografía.**
- **Base:** *Database Internals* — Alex Petrov
- **Complementaria:** *Database System Concepts* (7ª ed.) — Silberschatz, Korth & Sudarshan · *Readings in Database Systems* ("Red Book", 5ª ed., gratuito) · *Transaction Processing* — Gray & Reuter
- **Papers:** *"Architecture of a Database System"* — Hellerstein, Stonebraker & Hamilton (2007) · *"ARIES: A Transaction Recovery Method..."* — Mohan et al. (TODS 1992) · *"Access Path Selection in a Relational DBMS"* — Selinger et al. (SIGMOD 1979)

**Recursos.** 15445.courses.cs.cmu.edu (curso completo en video + proyectos BusTub con autograder) · redbook.io · PostgreSQL como referencia de implementación madura.

**Protocolo de estudio.** Ningún componente se considera terminado antes de someterlo a inyección de fallos en punto arbitrario. La recuperación es la especificación, no una función añadida al final.

---

### LEN-502 — Verificación Formal y Métodos Formales

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | LEN-201, TEO-303 |
| **ADN institucional** | CMU 15-414 · MIT 6.820 |

**Competencia terminal.** Especifica una propiedad temporal, la verifica mecánicamente y interpreta el contraejemplo cuando falla.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Lógica temporal | Estructuras de Kripke · LTL: sintaxis, semántica, operadores · CTL y CTL* · Expresividad comparada · Especificación de safety y liveness |
| 2 | 4–6 | Model checking | Autómatas de Büchi · Construcción del producto · Model checking explícito · BDDs: construcción, operaciones, reducción, ordenamiento de variables · Model checking simbólico |
| 3 | 7–9 | Model checking acotado y abstracción | Unrolling y codificación SAT · SMT: DPLL(T), teorías de arrays, bitvectors, funciones no interpretadas · CEGAR · Interpretación de contraejemplos |
| 4 | 10–12 | Verificación deductiva | Lógica de Hoare: reglas, consecuencia, bucle con variante e invariante · Correctitud parcial vs total · Weakest precondition (Dijkstra) · Separation Logic: frame rule, bi-abduction |
| 5 | 13–15 | Análisis estático | Interpretación abstracta: retículos, funciones monótonas, conexiones de Galois · Widening y narrowing · Dominios numéricos: intervalos, octágonos, poliedros · Precisión vs escalabilidad |

**Prueba de Dominio.** Verificación formal del algoritmo de exclusión mutua de Peterson en LTL usando SPIN, con interpretación del contraejemplo al debilitar una condición + prueba de correctitud de heapsort con lógica de Hoare e invariantes formalizados y mecanizados en Lean 4 o Rocq.

**Bibliografía.**
- **Base:** *Principles of Model Checking* — Baier & Katoen
- **Complementaria:** *Software Foundations* Vol. 1–3 — Pierce et al. (gratuito) · *The Calculus of Computation* — Bradley & Manna · *Model Checking* (2ª ed.) — Clarke et al.
- **Papers:** *"Separation Logic: A Logic for Shared Mutable Data Structures"* — Reynolds (LICS 2002)

**Recursos.** SPIN/Promela · TLA+ y TLC (Lamport) · Z3 y CVC5 · Lean 4 con mathlib · Rocq (antes Coq) · Dafny · Frama-C.

**Protocolo de estudio.** El asistente de pruebas se usa **después** de tener la prueba en papel, nunca para descubrirla. Buscar la prueba mediante tácticas produce dependencia de la herramienta sin comprensión, y colapsa en cuanto la herramienta no encuentra el camino.

---

### INT-500 — Laboratorio Integrador V

| | |
|---|---|
| **Créditos** | 2 |
| **Carga** | 0–0–3 / 5 · **8 h/sem** |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | SIS-501, LEN-501, LEN-502 (concurrentes) |

**Artefacto.** Pila vertical verificada: (a) el compilador de LEN-501 genera código para el núcleo de SIS-501, compilando al menos un programa de usuario no trivial que se ejecute correctamente sobre él; (b) una propiedad de seguridad del planificador del núcleo —ausencia de deadlock en la jerarquía de bloqueos, o exclusión mutua en una sección crítica— se modela en Promela o TLA+ y se verifica con LEN-502; (c) el contraejemplo obtenido al debilitar deliberadamente una condición se analiza y se traza hasta la línea de código correspondiente.

**Integra:** SIS-501 (núcleo) + LEN-501 (compilador) + LEN-502 (verificación) + ALG-403 (razonamiento concurrente).

**Defensa oral.** 30 minutos: mostrar el programa compilado ejecutándose sobre el núcleo propio y explicar el contraejemplo del modelo debilitado, mapeándolo al código real.

---

# CICLO VI — Inteligencia Artificial Teórica y Aprendizaje Automático

**25 créditos · 25 h lectivas/sem · 26 h EI/sem · Total ≈51 h/sem**

> **Propósito del ciclo.** Aprendizaje automático desde sus fundamentos matemáticos, no desde bibliotecas. Toda derivación se hace a mano antes de codificarse, y toda arquitectura se implementa sin frameworks de alto nivel al menos una vez. La computación cuántica y la geometría diferencial entran aquí porque comparten el mismo aparato de álgebra lineal y de variedades.

---

### IAP-601 — Fundamentos Matemáticos del Aprendizaje Automático — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-104, MAT-401, ALG-401 |
| **ADN institucional** | Stanford CS229 · UC Berkeley CS189 — vertiente teórica |

**Competencia terminal.** Deriva cotas de generalización y demuestra la convergencia de los algoritmos de aprendizaje que usa.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Teoría del aprendizaje | Marco PAC: clase de concepto, complejidad muestral · Consistencia · Dimensión VC: shattering, teorema de Vapnik-Chervonenkis · Complejidad de Rademacher · Compensación sesgo-varianza formalizada |
| 2 | 4–6 | Modelos lineales | OLS y sus propiedades (Gauss-Markov, BLUE) · Regularización L1/L2 y su interpretación bayesiana · Regresión logística: MLE, gradiente, Hessiano · GLMs y familia exponencial |
| 3 | 7–9 | Métodos de kernel | SVM de margen duro y suave · Dualidad de Lagrange aplicada (conexión con MAT-401) · Truco del kernel · Teorema de Mercer · Kernels válidos: RBF, polinomial, Matérn · Procesos Gaussianos |
| 4 | 10–12 | Modelos generativos y latentes | Estimación no paramétrica: k-NN con análisis asintótico · Algoritmo EM con prueba de convergencia · Mezclas gaussianas · Modelos gráficos: redes bayesianas, campos aleatorios de Markov · Inferencia exacta vs aproximada |
| 5 | 13–15 | Inferencia aproximada y ensembles | Inferencia variacional: ELBO, mean-field · MCMC: Metropolis-Hastings, Gibbs, diagnóstico de convergencia · Boosting: AdaBoost con prueba de margen · Bagging · Gradient Boosting |

**Prueba de Dominio.** Demostración del teorema fundamental de la teoría PAC (cota de generalización vía dimensión VC) + derivación completa del dual del SVM con kernel + prueba de convergencia del algoritmo EM para mezclas gaussianas. Cada resultado instanciado numéricamente.

**Bibliografía.**
- **Base:** *Understanding Machine Learning: From Theory to Algorithms* — Shalev-Shwartz & Ben-David (gratuito)
- **Complementaria:** *The Elements of Statistical Learning* (2ª ed.) — Hastie, Tibshirani & Friedman (gratuito) · *Pattern Recognition and Machine Learning* — Bishop · *Probabilistic Machine Learning* — Murphy (gratuito)
- **Papers:** *"A Training Algorithm for Optimal Margin Classifiers"* — Boser, Guyon & Vapnik (COLT 1992)

**Recursos.** cs229.stanford.edu (notas y problem sets) · Berkeley CS189 · probml.github.io (Murphy, gratuito) · scikit-learn solo como referencia de contraste, nunca como implementación primaria.

**Protocolo de estudio.** Cada cota se instancia numéricamente: ¿cuántas muestras exige para ε = 0.05 y δ = 0.05? El número suele ser absurdamente grande, y esa es la lección — la teoría acota, no predice el comportamiento práctico.

---

### IAP-602 — Redes Neuronales Profundas: Teoría y Arquitecturas — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | IAP-601 (concurrente permitido) |
| **ADN institucional** | Stanford CS231N y CS224N · MIT 6.S191 |

**Competencia terminal.** Deriva analíticamente el gradiente de cualquier capa y construye arquitecturas modernas sin frameworks de alto nivel.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Diferenciación y optimización | Diferenciación automática: modo forward vs reverse, grafos de cómputo, tape-based AD · Derivación exacta de gradientes para capas densas · Gradient checking numérico · SGD, Adam/AdamW con análisis de convergencia · Schedules |
| 2 | 4–6 | Estabilidad del entrenamiento | Vanishing y exploding gradients: análisis espectral del Jacobiano · Inicialización (Xavier, He) · Batch norm, layer norm, RMSNorm · Conexiones residuales y su efecto sobre el paisaje de pérdida · Teorema de aproximación universal (Cybenko, Hornik) |
| 3 | 7–9 | Arquitecturas convolucionales y recurrentes | Convolución vs correlación cruzada · Campo receptivo · Conteo de parámetros · AlexNet → VGG → ResNet → EfficientNet · RNN y BPTT · LSTM: compuertas y flujo de gradiente · GRU |
| 4 | 10–12 | Atención y Transformers | Scaled dot-product attention con análisis O(n²d) · Multi-head · Codificación posicional: absoluta, RoPE, ALiBi · Arquitectura completa del Transformer · **FlashAttention y su análisis de complejidad de I/O** |
| 5 | 13–15 | Arquitecturas actuales y fenómenos | **State space models: S4, Mamba** · **Atención lineal** · **Mixture-of-experts: routing y balanceo de carga** · Double descent y benign overfitting · Lottery ticket hypothesis · Escalamiento de la profundidad |

**Prueba de Dominio.** Transformer encoder-decoder completo implementado desde cero en numpy o JAX, sin frameworks de alto nivel, con el backward pass derivado analíticamente a mano y validado con gradient checking numérico, entrenado sobre una tarea de traducción de secuencias con análisis de la curva de convergencia.

**Bibliografía.**
- **Base:** *Understanding Deep Learning* — Simon J.D. Prince (MIT Press, 2023; gratuito)
- **Complementaria:** *Deep Learning: Foundations and Concepts* — Bishop & Bishop (2023) · *Dive into Deep Learning* — Zhang et al. (gratuito). *Deep Learning* — Goodfellow, Bengio & Courville (2016) se retiene **solo como referencia histórica**: su cobertura de arquitecturas está obsoleta.
- **Papers:** *"Attention Is All You Need"* — Vaswani et al. (NeurIPS 2017) · *"Deep Residual Learning for Image Recognition"* — He et al. (CVPR 2016) · *"FlashAttention"* — Dao et al. (NeurIPS 2022) · *"Mamba: Linear-Time Sequence Modeling with Selective State Spaces"* — Gu & Dao (2023)

**Recursos.** udlbook.github.io (Prince, gratuito con notebooks) · cs231n.stanford.edu · web.stanford.edu/class/cs224n · d2l.ai · JAX y numpy únicamente para la Prueba de Dominio.

**Protocolo de estudio.** El backward pass se deriva a mano en papel para cada capa nueva **antes** de codificarla, y se valida con gradient checking numérico. Usar autograd sin haber derivado a mano al menos una vez es el atajo que vacía esta asignatura por completo.

---

### IAP-603 — Inteligencia Artificial: Búsqueda, Planificación y Razonamiento

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-104, ALG-401 |
| **ADN institucional** | UC Berkeley CS188 · Stanford CS221 — vertiente teórica |

**Competencia terminal.** Demuestra propiedades de optimalidad y convergencia de agentes de búsqueda y de aprendizaje por refuerzo.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Búsqueda | BFS, DFS, costo uniforme · A*: admisibilidad, consistencia, completitud y optimalidad con demostración · IDA*, RBFS, SMA* · Diseño de heurísticas y dominancia |
| 2 | 4–6 | Búsqueda adversarial | Minimax · Poda alfa-beta con análisis del factor de ramificación efectivo · Expectimax · MCTS y UCT con la cota de confianza superior |
| 3 | 7–9 | Satisfacción de restricciones | CSP · Backtracking con heurísticas de orden · Arc consistency (AC-3) · Forward checking · Búsqueda local: GSAT, WalkSAT · Planificación: STRIPS, PDDL, orden parcial |
| 4 | 10–12 | Razonamiento probabilístico | Redes bayesianas · Inferencia exacta por eliminación de variables · Belief propagation · HMM: forward-backward, Viterbi, Baum-Welch como caso de EM |
| 5 | 13–15 | Decisión y refuerzo | MDP · Ecuaciones de Bellman · Value iteration y policy iteration con prueba de convergencia por contracción · Q-learning con análisis de convergencia · TD y SARSA · Policy gradient: REINFORCE, Actor-Critic, PPO |

**Prueba de Dominio.** Demostración formal de la optimalidad de A* con heurística admisible y consistente, incluyendo el contraejemplo que muestra por qué la admisibilidad sola no basta para grafos + agente de Q-learning con convergencia demostrada al óptimo en un MDP finito donde el óptimo se calcula en forma cerrada.

**Bibliografía.**
- **Base:** *Artificial Intelligence: A Modern Approach* (4ª ed.) — Russell & Norvig
- **Complementaria:** *Reinforcement Learning: An Introduction* (2ª ed.) — Sutton & Barto (gratuito) · *Algorithms for Decision Making* — Kochenderfer et al. (gratuito)
- **Papers:** *"Bandit Based Monte-Carlo Planning"* — Kocsis & Szepesvári (ECML 2006)

**Recursos.** inst.eecs.berkeley.edu/~cs188 (proyectos Pacman) · incompleteideas.net/book (Sutton & Barto gratuito) · algorithmsbook.com · Gymnasium para entornos.

**Protocolo de estudio.** Toda propiedad de convergencia se verifica empíricamente en un entorno de juguete donde el óptimo es calculable en forma cerrada. Sin ese contraste no hay verificación: hay confianza en que el código está bien.

---

### TEO-601 — Computación Cuántica: Teoría y Algoritmos

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-102, MAT-302, TEO-302 |
| **ADN institucional** | MIT 8.370[J] / 18.435[J] · UC Berkeley CS294 |

**Competencia terminal.** Deriva algoritmos cuánticos desde primeros principios y sitúa BQP respecto de las clases clásicas.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Formalismo | Espacios de Hilbert · Notación de Dirac: bras, kets, operadores · Producto tensorial · Qubit y esfera de Bloch · Medición y colapso · Entrelazamiento y desigualdad de Bell |
| 2 | 4–6 | Circuitos | Unitariedad y reversibilidad · Hadamard, Pauli, CNOT, Toffoli, T · Universalidad de conjuntos de compuertas · Rotaciones en SU(2) · Teorema de Solovay-Kitaev · No-cloning |
| 3 | 7–9 | Algoritmos fundamentales | Deutsch-Jozsa · Bernstein-Vazirani · Simon · Quantum Fourier Transform con construcción O(n²) · Estimación de fase |
| 4 | 10–12 | Shor y Grover | Reducción de factorización a order-finding · Shor completo con análisis de probabilidad de éxito · Grover: O(√N), interpretación geométrica, optimalidad de la cota · Amplitude amplification |
| 5 | 13–15 | Errores y complejidad | Código de Shor · Formalismo de estabilizadores · Toric code · Umbral de tolerancia a fallos · BQP y QMA · Relación con P, NP, PSPACE · Muestreo de circuitos aleatorios |

**Prueba de Dominio.** Derivación completa del algoritmo de Shor desde la reducción de factorización a order-finding, pasando por la QFT sobre ℤ_N, hasta el análisis de probabilidad de éxito y el número esperado de repeticiones + simulador clásico de circuitos cuánticos de n qubits con complejidad O(4ⁿ poly(n)), validado factorizando un semiprimo pequeño.

**Bibliografía.**
- **Base:** *Quantum Computation and Quantum Information* — Nielsen & Chuang (edición aniversario)
- **Complementaria:** *Quantum Computing Since Democritus* — Aaronson · *Quantum Computation Lecture Notes* — Preskill (Caltech Ph219, gratuito)
- **Papers:** *"Polynomial-Time Algorithms for Prime Factorization..."* — Shor (SIAM J. Comput. 1997) · *"A Fast Quantum Mechanical Algorithm for Database Search"* — Grover (STOC 1996)

**Recursos.** MIT OCW 8.370 · theory.caltech.edu/~preskill/ph219 · Qiskit y Cirq para simulación · scottaaronson.blog para discusión crítica de afirmaciones de supremacía.

**Protocolo de estudio.** Cada algoritmo se simula clásicamente con n pequeño antes de razonar sobre n grande. El álgebra lineal de MAT-102 se recupera explícitamente aquí: es exactamente el mismo objeto matemático, y tratarlo como algo nuevo duplica el costo de aprendizaje.

---

### MAT-601 — Geometría Diferencial y Álgebra Tensorial para Aprendizaje

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-103, MAT-401 |
| **ADN institucional** | Stanford CS468 · MIT 18.950 |

**Competencia terminal.** Formula problemas de optimización sobre variedades y deriva el gradiente natural desde la métrica de Fisher.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Variedades | Cartas y atlas · Funciones suaves · Espacio tangente · Campos vectoriales · Corchete de Lie · Derivada de Lie |
| 2 | 4–6 | Formas diferenciales | k-formas · Producto exterior · Derivada exterior · Teorema de Stokes generalizado · Cohomología de De Rham (introducción) |
| 3 | 7–9 | Geometría Riemanniana | Tensor métrico · Geodésicas · Conexión de Levi-Civita · Símbolos de Christoffel · Transporte paralelo · Curvatura: Riemann, Ricci, escalar |
| 4 | 10–12 | Geometría de la información | Variedad estadística · Métrica de Fisher-Rao · Divergencia KL como geometría · Conexiones duales · Gradiente natural (Amari) · Dualidad exponencial-mixta |
| 5 | 13–15 | Grupos de Lie y aplicaciones | Grupos de matrices · Álgebra de Lie · Exponencial de matrices · Representación adjunta · Optimización sobre variedades (Stiefel, Grassmann) · Geometría del paisaje de pérdida en redes neuronales |

**Prueba de Dominio.** Derivación del gradiente natural desde la métrica de Fisher-Rao sobre la variedad de distribuciones + demostración de que converge más rápido que el gradiente estándar en términos de geometría de la información, con verificación empírica sobre la variedad de gaussianas.

**Bibliografía.**
- **Base:** *Differential Geometry of Curves and Surfaces* — do Carmo
- **Complementaria:** *Information Geometry and Its Applications* — Amari · *Introduction to Smooth Manifolds* — J.M. Lee · *Optimization Algorithms on Matrix Manifolds* — Absil, Mahony & Sepulchre (gratuito)
- **Papers:** *"Natural Gradient Works Efficiently in Learning"* — Amari (Neural Computation 1998)

**Recursos.** press.princeton.edu/absil (libro gratuito) · Pymanopt / Geomstats para experimentación · Stanford CS468.

**Protocolo de estudio.** La asignatura más abstracta del programa y la de mayor riesgo de estudio superficial. Regla: todo objeto se calcula explícitamente en S² **y** en la variedad de gaussianas antes de darse por comprendido. Sin las dos instancias, el objeto es una notación.

---

### INT-600 — Laboratorio Integrador VI

| | |
|---|---|
| **Créditos** | 2 |
| **Carga** | 0–0–3 / 5 · **8 h/sem** |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | IAP-602, MAT-601 (concurrentes) |

**Artefacto.** Estudio experimental sobre el Transformer de IAP-602: (a) entrenar la misma arquitectura bajo régimen de gradiente estándar y bajo una aproximación del gradiente natural (K-FAC o similar) derivada según MAT-601, (b) medir y comparar las curvas de convergencia, (c) contrastar la generalización empírica contra la cota teórica de IAP-601 y documentar la magnitud de la brecha, (d) reporte con protocolo de reproducibilidad completo: semillas, entorno, hiperparámetros, varianza entre corridas.

**Integra:** IAP-601 (cotas de generalización) + IAP-602 (arquitectura y entrenamiento) + MAT-601 (gradiente natural) + MAT-401 (teoría de convergencia).

**Defensa oral.** 25 minutos: justificar por qué la brecha entre cota teórica y desempeño empírico tiene la magnitud observada, sin recurrir a "la teoría es pesimista" como explicación.
---

# CICLO VII — Criptografía, Seguridad y Sistemas Distribuidos

**25 créditos · 26 h lectivas/sem · 28 h EI/sem · Total ≈54 h/sem**

> **Propósito del ciclo.** El ciclo donde el argumento formal se vuelve la defensa contra un adversario real. Criptografía y sistemas distribuidos comparten la misma estructura de razonamiento: definir el modelo de adversario o de falla, y demostrar qué es imposible antes de construir lo que sí lo es.

---

### SEG-701 — Criptografía: Fundamentos Matemáticos y Protocolos — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 12 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-302, MAT-104, TEO-302 |
| **ADN institucional** | UC Berkeley CS276 · MIT 6.5620 / 18.425 *(ex 6.875)* · Stanford CS255 |

**Competencia terminal.** Construye argumentos de seguridad como reducciones formales desde una suposición computacional, y detecta cuándo un esquema carece de ese argumento.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Marco formal | Juegos de seguridad · Ventaja del adversario · Seguridad perfecta (one-time pad) vs computacional · Funciones de un solo sentido (OWF) como suposición central · Predicados hardcore |
| 2 | 4–6 | Primitivas simétricas | PRG: stretch e indistinguibilidad · PRF: construcción desde PRG por árbol GGM · PRP y cifrados de bloque · AES y su análisis algebraico en GF(2⁸) (conexión con MAT-302) · Modos de operación · MAC y HMAC · Cifrado autenticado (AEAD) |
| 3 | 7–9 | Nociones de seguridad y clave pública | IND-CPA, IND-CCA1, IND-CCA2 · Relaciones entre nociones · RSA y su análisis (OAEP) · ElGamal · Diffie-Hellman: suposiciones CDH y DDH · Curvas elípticas: grupo de puntos sobre GF(p), ECDLP, ECDSA, EdDSA |
| 4 | 10–12 | Hash y pruebas de conocimiento | Modelo del oráculo aleatorio y sus límites · Resistencia a colisiones · Merkle-Damgård vs esponja (SHA-3/Keccak) · Zero-knowledge: completitud, solidez, ZK por simulación · Protocolos sigma · Fiat-Shamir · Compromisos · Oblivious Transfer |
| 5 | 13–15 | Criptografía post-cuántica y avanzada | **Problemas reticulares: SIS, LWE, Ring-LWE** · **Estándares NIST: ML-KEM (FIPS 203), ML-DSA (FIPS 204), SLH-DSA (FIPS 205)** · Firmas basadas en hash · **Encriptación completamente homomórfica: BGV, CKKS, bootstrapping** · Computación multipartita segura (introducción) |

**Prueba de Dominio.** Demostración formal de que ningún cifrado de clave pública puede ser IND-CCA2 sin padding apropiado (con el ataque explícito como contraejemplo constructivo) + construcción de un protocolo de identificación Σ con demostración de las tres propiedades, incluyendo el simulador explícito para zero-knowledge.

**Bibliografía.**
- **Base:** *A Graduate Course in Applied Cryptography* — Boneh & Shoup (gratuito)
- **Complementaria:** *Introduction to Modern Cryptography* (3ª ed.) — Katz & Lindell · *Foundations of Cryptography* Vol. 1–2 — Goldreich · *Serious Cryptography* (2ª ed.) — Aumasson (perspectiva de implementación)
- **Estándares:** FIPS 197 (AES) · FIPS 202 (SHA-3) · FIPS 203/204/205 (post-cuántica)
- **Papers:** *"New Directions in Cryptography"* — Diffie & Hellman (1976) · *"On Lattices, Learning with Errors..."* — Regev (JACM 2009)

**Recursos.** toc.cryptobook.us (Boneh & Shoup gratuito) · crypto.stanford.edu/~dabo/courses/cs255 · csrc.nist.gov/projects/post-quantum-cryptography · CryptoHack y cryptopals para práctica de ataques · SageMath para aritmética de curvas y retículos.

**Protocolo de estudio.** Toda prueba de seguridad se escribe como reducción explícita: *adversario que rompe el esquema → adversario que rompe la suposición*. Formato de tarjeta único de la asignatura: "dado este esquema roto, construye el adversario contra la suposición subyacente". Memorizar el enunciado de seguridad sin la reducción no sirve para nada en esta asignatura.

---

### SIS-701 — Sistemas Distribuidos: Teoría y Construcción — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-501, SIS-502, ALG-403 |
| **ADN institucional** | MIT 6.5840 *(ex 6.824)* · CMU 15-440 |

**Competencia terminal.** Implementa un protocolo de consenso correcto bajo fallas y demuestra qué garantías son imposibles en el modelo dado.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelos e imposibilidades | Modelos de sincronía: síncrono, asíncrono, parcialmente síncrono · Modelos de falla: crash-stop, omisión, bizantino · **Teorema FLP con demostración completa** · Teorema CAP con demostración · Detectores de fallos |
| 2 | 4–6 | Tiempo y causalidad | Relojes de Lamport · Relojes vectoriales (Mattern, Fidge) · Relación happened-before · Cortes consistentes · Snapshot de Chandy-Lamport |
| 3 | 7–9 | Modelos de consistencia | Linearizabilidad · Serializabilidad · Consistencia secuencial · Consistencia causal · Consistencia eventual · Jerarquía completa y sus costos · CRDTs |
| 4 | 10–12 | Consenso | Paxos: Single-Decree y Multi-Paxos, safety y liveness · Raft: elección de líder, replicación de log, compactación, cambio de configuración · Replicación de máquinas de estado · Viewstamped Replication · BFT: PBFT con análisis de f ≤ ⌊(n−1)/3⌋ |
| 5 | 13–15 | Sistemas reales | DHT: Chord con análisis de O(log n) saltos · Sistemas de archivos distribuidos: GFS, Ceph · Transacciones distribuidas: 2PC, 3PC · Spanner y TrueTime · Protocolos gossip y modelos epidémicos |

**Laboratorios.** L1 MapReduce · L2 Raft: elección de líder · L3 Raft: replicación de log · L4 Raft: persistencia y compactación · L5 servicio clave-valor tolerante a fallos · L6 fragmentación (sharding).

**Prueba de Dominio.** Demostración completa del Teorema FLP + implementación funcional del protocolo Raft con prueba de que mantiene la propiedad de log matching bajo fallas de crash arbitrarias. Evaluado bajo particiones de red, reordenamiento y pérdida de mensajes inyectados de forma determinista y reproducible.

**Bibliografía.**
- **Base:** *Designing Data-Intensive Applications* (**2ª ed., marzo 2026**) — Kleppmann & Riccomini
- **Complementaria:** *Distributed Systems* (4ª ed.) — van Steen & Tanenbaum (gratuito) · *Introduction to Reliable and Secure Distributed Programming* — Cachin, Guerraoui & Rodrigues
- **Papers:** *"Impossibility of Distributed Consensus with One Faulty Process"* — Fischer, Lynch & Paterson (JACM 1985) · *"In Search of an Understandable Consensus Algorithm"* — Ongaro & Ousterhout (USENIX ATC 2014) · *"Paxos Made Simple"* — Lamport (2001) · *"Time, Clocks, and the Ordering of Events"* — Lamport (CACM 1978) · *"Spanner: Google's Globally-Distributed Database"* — Corbett et al. (OSDI 2012)

**Recursos.** pdos.csail.mit.edu/6.824 (labs completos en Go + video) · distributed-systems.net (van Steen gratuito) · raft.github.io (visualización) · TLA+ para especificar el protocolo antes de implementarlo · Jepsen como referencia de metodología de testing.

**Protocolo de estudio.** Toda implementación se somete a particiones y reordenamiento de mensajes inyectados de forma determinista. Un Raft que pasa el camino feliz no está implementado: está esbozado. Especificar en TLA+ antes de codificar reduce el tiempo total, no lo aumenta.

---

### SEG-702 — Seguridad de Sistemas y Ataques a Bajo Nivel

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-201, SIS-501 |
| **ADN institucional** | CMU 15-330 · UC Berkeley CS161 · Stanford CS155 |

**Competencia terminal.** Construye un modelo de amenaza explícito y deriva de él tanto el ataque como la mitigación.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelado de amenaza | Definición de adversario y de sus capacidades · Superficie de ataque · Trust boundaries · Principios de diseño seguro (Saltzer & Schroeder) · Análisis de riesgo |
| 2 | 4–6 | Vulnerabilidades de memoria | Buffer overflow en stack y heap · Use-after-free · Double free · Format string · Integer overflow · Explotación: control de RIP, shellcode |
| 3 | 7–9 | Mitigaciones y evasión | DEP/NX · Stack canaries · ASLR y PIE · CFI · Return-oriented programming · Formato ELF, PLT/GOT, lazy binding · Bypass de cada mitigación |
| 4 | 10–12 | Canales laterales y protocolo | Timing attacks sobre RSA · Cache-timing: Flush+Reload, Prime+Probe · Spectre y Meltdown: análisis microarquitectural · Padding oracle · BEAST, CRIME · Bleichenbacher sobre PKCS#1 · Criptoanálisis diferencial y lineal |
| 5 | 13–15 | Análisis y modelos formales | Fuzzing guiado por cobertura (AFL++) · Ejecución simbólica y concólica (KLEE, angr) · Ingeniería inversa: estático vs dinámico · SQL injection, XSS, CSRF, SSRF a nivel de protocolo · Bell-LaPadula y Biba con demostración de propiedades |

**Prueba de Dominio.** Explotación completa de un binario Linux x86-64 con PIE, ASLR y stack canaries activos, mediante cadena ROP construida desde primeros principios (sin herramientas automáticas de generación de cadenas) + demostración matemática del ataque de padding oracle, explicando por qué CBC sin autenticación es estructuralmente inseguro.

**Bibliografía.**
- **Base:** *Computer Security: Art and Science* (2ª ed.) — Bishop
- **Complementaria:** *The Art of Software Security Assessment* — Dowd, McDonald & Schuh · *Practical Binary Analysis* — Andriesse · *The Shellcoder's Handbook*
- **Papers:** *"Smashing the Stack for Fun and Profit"* — Aleph One (Phrack 49, 1996) · *"Spectre Attacks: Exploiting Speculative Execution"* — Kocher et al. (S&P 2019) · *"The Protection of Information in Computer Systems"* — Saltzer & Schroeder (1975)

**Recursos.** pwn.college (curso estructurado de explotación) · picoCTF · Ghidra, radare2, pwntools, GDB con pwndbg · AFL++, KLEE, angr · **Máquina virtual aislada obligatoria.**

**Protocolo de estudio.** Trabajo exclusivamente sobre binarios y entornos propios, aislados en máquina virtual sin red. La asignatura se estudia **desde el modelo de amenaza hacia el exploit**, nunca al revés: memorizar técnicas sin modelo produce operadores de herramientas, no investigadores de seguridad.

---

### LEN-701 — Tipos Dependientes y Verificación Mecanizada

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–2–2 / 10 · **17 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | LEN-201, LEN-502, TEO-303 |
| **ADN institucional** | CMU 15-317 y 15-819 · MIT 6.826 |

**Competencia terminal.** Expresa una especificación como tipo y produce un programa cuya corrección es consecuencia de que tipa.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Curry-Howard extendida | Proposiciones como tipos, pruebas como programas · Lógica intuicionista vs clásica · Sistema F: polimorfismo de segundo orden, normalización fuerte · Parametricidad (Reynolds) |
| 2 | 4–6 | Tipos dependientes | Π-tipos y Σ-tipos · Tipo identidad · Teoría de tipos de Martin-Löf · Universos y su jerarquía · Cálculo de Construcciones · Sort checking |
| 3 | 7–9 | Asistentes de prueba | Lean 4 y su biblioteca mathlib · Rocq (antes Coq) · Tácticas y procedimientos de decisión · Reflexión por cómputo · Extracción de código certificado |
| 4 | 10–12 | Teoría de tipos homotópica | Igualdad como camino · Axioma de univalencia · Tipos inductivos superiores · Interpretación de los tipos como espacios · Consecuencias para el razonamiento sobre estructuras |
| 5 | 13–15 | Sistemas de tipos aplicados | Refinement types: Liquid Haskell, subtipado con SMT · Efectos algebraicos y handlers · Free monads · Session types: protocolos como tipos · Sistemas subestructurales: lineales, afines, relevantes · Rust como sistema afín en producción |

**Prueba de Dominio.** Formalización completa en Lean 4 (o Rocq) de la correctitud de mergesort, incluyendo preservación de contenido (permutación) y de orden, con extracción de código ejecutable certificado y verificación de que el código extraído se comporta como el especificado.

**Bibliografía.**
- **Base:** *Software Foundations* Vol. 1–3 — Pierce et al. (gratuito)
- **Complementaria:** *Homotopy Type Theory: Univalent Foundations of Mathematics* — The Univalent Foundations Program (gratuito) · *Mathematics in Lean* (mathlib, gratuito) · *Certified Programming with Dependent Types* — Chlipala (gratuito) · *Practical Foundations for Programming Languages* — Harper
- **Papers:** *"Propositions as Types"* — Wadler (CACM 2015)

**Recursos.** softwarefoundations.cis.upenn.edu · leanprover-community.github.io · homotopytypetheory.org/book · Zulip de Lean para consultas · Agda y Idris 2 como alternativas de exploración.

**Protocolo de estudio.** Toda formalización arranca por el **enunciado del tipo**, antes que por la prueba. Si el tipo está mal formulado, la prueba es irrelevante — y un tipo mal planteado que sin embargo tipa es el error dominante y el más difícil de detectar de esta asignatura.

---

### SIS-702 — Computación de Alto Rendimiento y Arquitecturas Especializadas

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | ALG-403, SIS-201 |
| **ADN institucional** | Stanford CS315A · MIT 6.106 *(ex 6.172)* · CMU 15-418/618 |

**Competencia terminal.** Explica cada optimización de rendimiento desde un modelo cuantitativo y alcanza una fracción justificada del límite teórico del hardware.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelos de rendimiento | Roofline: intensidad aritmética, límite por memoria vs por cómputo · Amdahl refinado con overhead de comunicación · Medición correcta: varianza, warm-up, efectos de frecuencia |
| 2 | 4–6 | Optimización en CPU | SIMD: AVX-512, vectorización automática y manual, operaciones de carril · Loop tiling y blocking multinivel · Análisis del working set · Prefetching de hardware y software · Row buffer locality en DRAM |
| 3 | 7–9 | Arquitectura GPU | Modelo SIMT · Warps y divergencia · Ocupancia · Jerarquía de memoria: global, shared, L1/L2 · Memory coalescing · Bank conflicts |
| 4 | 10–12 | Programación CUDA | Modelo de ejecución y de memoria · Optimización de kernels · Streams y solapamiento · Tensor cores · Cuantización: INT8, FP16, BF16, FP8 · Perfilado con Nsight |
| 5 | 13–15 | Escala distribuida | Redes de interconexión: bisection bandwidth, fat-tree, torus, routing · MPI: punto a punto y colectivos (barrier, broadcast, reduce, all-reduce) · Modelos SPMD y BSP · Paralelismo de datos, de tensor y de pipeline |

**Prueba de Dominio.** Multiplicación de matrices densa (GEMM) en CUDA que alcance ≥90% de la eficiencia del roofline teórico de la GPU disponible, mediante uso de memoria compartida, vectorización y ocultamiento de latencia. Cada paso de optimización documentado con medición antes/después y explicación causal desde el modelo.

**Bibliografía.**
- **Base:** *Programming Massively Parallel Processors* (4ª ed.) — Kirk, Hwu & El Hajj
- **Complementaria:** *Computer Architecture: A Quantitative Approach* (6ª ed.) — Hennessy & Patterson · *Performance Analysis and Tuning on Modern CPUs* — Bakhvalov (gratuito)
- **Papers:** *"Roofline: An Insightful Visual Performance Model"* — Williams, Waterman & Patterson (CACM 2009)

**Recursos.** CMU 15-418 (video completo) · MIT 6.106 · Documentación del vendor de la GPU disponible (**verificar generación y guía de tuning vigente**) · Nsight Compute, `perf`, likwid · CUTLASS como referencia de GEMM optimizado.

**Protocolo de estudio.** Ninguna optimización se acepta sin medición antes/después **y** sin explicación causal desde el modelo roofline. Optimizar sin modelo es superstición: produce mejoras que no se transfieren y regresiones que no se explican.

---

### INT-700 — Laboratorio Integrador VII

| | |
|---|---|
| **Créditos** | 2 |
| **Carga** | 0–0–3 / 5 · **8 h/sem** |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | SEG-701, SIS-701, SIS-702 (concurrentes) |

**Artefacto.** Almacén clave-valor distribuido y autenticado: (a) replicación con el Raft de SIS-701, (b) autenticación de operaciones mediante el protocolo Σ de SEG-701, con la demostración de sus tres propiedades adjunta, (c) validación criptográfica por lotes acelerada en GPU según SIS-702, con análisis roofline de la ganancia, (d) auditoría de la superficie de ataque bajo el modelo de amenaza de SEG-702, incluyendo al menos un ataque encontrado y mitigado, (e) evaluación bajo particiones de red con verificación de linearizabilidad de las historias generadas.

**Integra:** SIS-701 (consenso) + SEG-701 (protocolo de autenticación) + SIS-702 (aceleración) + SEG-702 (modelo de amenaza) + LEN-502 (verificación del protocolo).

**Defensa oral.** 30 minutos: presentar el ataque encontrado, su mitigación, y justificar por qué la mitigación no rompe ninguna de las tres propiedades del protocolo Σ.

---

# CICLO VIII — Frontera de Investigación y Síntesis

**26 créditos · 20 h lectivas/sem · 32 h EI/sem · Total ≈52 h/sem**

> **Propósito del ciclo.** El ciclo invierte la estructura: menos horas lectivas, más trabajo autónomo. La tesis ocupa bloques largos continuos, no slots fraccionados, porque el trabajo de investigación no admite fragmentación en unidades de 90 minutos.

---

### ALG-801 — Complejidad Fina y Algoritmos de Frontera

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 12 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ALG-402, TEO-302 |
| **ADN institucional** | MIT 6.890 *(R. Williams & V. Vassilevska Williams)* · UC Berkeley CS294 |

**Competencia terminal.** Demuestra cotas inferiores condicionadas y sitúa un problema dentro del grafo de hipótesis de complejidad fina.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Hipótesis y reducciones finas | SETH y ETH · Orthogonal Vectors Conjecture · 3-SUM hardness · APSP-equivalencias · Reducciones que preservan el exponente |
| 2 | 4–6 | Cotas inferiores condicionadas | SETH-hardness de Edit Distance, LCS, Fréchet distance · Consecuencias para problemas de cadenas y de grafos · Barreras a la mejora de exponentes |
| 3 | 7–9 | Dureza de aproximación | Teorema PCP: enunciado y construcción · Long Code · Reducciones gap-introducing · Clique (no n^(1−ε)) · Set Cover (ln n ajustado) · Unique Games Conjecture y sus implicaciones para Vertex Cover y Max-Cut |
| 4 | 10–12 | Algoritmos para datos masivos | Streaming: Morris, Flajolet-Martin, AMS sketch · Count-Min · Johnson-Lindenstrauss y reducción de dimensión · Property testing: ε-tester y complejidad de consultas · Algoritmos sublineales |
| 5 | 13–15 | Tratabilidad parametrizada y complejidad algebraica | FPT y jerarquía W · Treewidth y DP sobre descomposición arbórea · Kernelización y cotas inferiores de kernel · Circuitos aritméticos · Permanent vs Determinant (Valiant) · Strassen y cotas inferiores de multiplicación de matrices |

**Prueba de Dominio.** Demostración formal de que Edit Distance no admite algoritmo de tiempo O(n^(2−ε)) salvo que SETH sea falsa, con la reducción explícita desde OV + construcción completa de un PCP para un lenguaje NP-completo con gap 1/2.

**Bibliografía.**
- **Base:** *Computational Complexity: A Modern Approach* — Arora & Barak
- **Complementaria:** *Parameterized Algorithms* — Cygan et al. (gratuito) · *The Probabilistic Method* — Alon & Spencer
- **Papers:** *"Fine-Grained Algorithms and Complexity"* (survey) — Vassilevska Williams · *"Edit Distance Cannot Be Computed in Strongly Subquadratic Time"* — Backurs & Indyk (STOC 2015) · *"Probabilistic Checking of Proofs"* — Arora & Safra (JACM 1998)

**Recursos.** MIT 6.890 (notas públicas) · people.csail.mit.edu/virgi (surveys y slides) · ECCC (Electronic Colloquium on Computational Complexity) para papers recientes.

**Protocolo de estudio.** Cada reducción se dibuja como nodo en un diagrama de dependencias condicionales. La estructura del campo **es** ese grafo; memorizar resultados aislados sin la estructura no permite ni reconocer ni construir reducciones nuevas.

---

### IAP-801 — Modelos de Lenguaje: Teoría y Escalamiento

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | IAP-602, SIS-702 |
| **ADN institucional** | **Stanford CS336 — *Language Modeling from Scratch* (Liang & Hashimoto, edición Spring 2026)** · MIT 6.S965 |

**Competencia terminal.** Construye la pila completa de un modelo de lenguaje y razona cuantitativamente sobre el compromiso entre cómputo, datos y parámetros.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Tokenización y contabilidad de recursos | BPE y variantes byte-level · Patologías de tokenización · Contabilidad de FLOPs, memoria y ancho de banda · Presupuesto de cómputo del entrenamiento |
| 2 | 4–6 | Arquitectura y sistemas | Transformer decoder-only en detalle · Normalización y ubicación de la norma · RoPE · Atención agrupada (GQA/MQA) · Kernels y FlashAttention · **Mixture-of-experts: routing, balanceo de carga, capacidad** · Paralelismo de datos, tensor, pipeline y secuencia |
| 3 | 7–9 | Leyes de escalamiento | Kaplan et al.: relaciones potenciales entre pérdida, parámetros, datos y cómputo · Chinchilla: punto óptimo de cómputo · Derivación desde primeros principios estadísticos · **Crítica de las "habilidades emergentes": dependencia de la métrica (Schaeffer et al.)** |
| 4 | 10–12 | Datos y alineamiento | Curación y deduplicación · Contaminación de benchmarks · RLHF con PPO: KL como regularización, reward hacking · DPO y métodos sin modelo de recompensa · RLAIF / Constitutional AI · **RL con recompensa verificable y cómputo en tiempo de inferencia** |
| 5 | 13–15 | Inferencia e interpretabilidad | KV-cache · Decodificación especulativa · Cuantización: GPTQ, AWQ · Batching continuo y PagedAttention · **Interpretabilidad mecanística: superposición, monosemanticidad, sparse autoencoders, análisis de circuitos** · Memorización y capacidad · Jailbreaking y prompt injection como problema formal |

**Prueba de Dominio.** Derivación analítica de las leyes de escalamiento desde primeros principios estadísticos + implementación de un Transformer decoder-only con KV-cache y decodificación especulativa, con predicción teórica de la mejora de throughput contrastada contra la medición real y la discrepancia explicada desde el modelo roofline de SIS-702.

**Bibliografía.**
- **Base:** Materiales públicos de Stanford CS336 (lecturas, assignments y video de la edición vigente)
- **Complementaria:** *Understanding Deep Learning* — Prince (base arquitectónica) · *Speech and Language Processing* (3ª ed. en borrador) — Jurafsky & Martin (gratuito)
- **Papers:** *"Attention Is All You Need"* — Vaswani et al. (2017) · *"Scaling Laws for Neural Language Models"* — Kaplan et al. (2020) · *"Training Compute-Optimal Large Language Models"* — Hoffmann et al. (2022) · *"Are Emergent Abilities of Large Language Models a Mirage?"* — Schaeffer, Miranda & Koyejo (NeurIPS 2023) · *"Toy Models of Superposition"* — Elhage et al. (Anthropic, 2022) · *"Direct Preference Optimization"* — Rafailov et al. (NeurIPS 2023)

**Recursos.** cs336.stanford.edu (**verificar edición vigente**) · web.stanford.edu/~jurafsky/slp3 · transformer-circuits.pub · Papers with Code y ECCC/arXiv para seguimiento.

**Protocolo de estudio.** Asignatura de vida media corta. Los papers se leen con el protocolo de tres pasadas (Keshav) y toda afirmación empírica se marca explícitamente como **replicada** o **no replicada**. Solo lo estructural entra al mazo FSRS —arquitectura, contabilidad de recursos, derivaciones—; lo coyuntural (números de un modelo concreto, resultados de un benchmark) no entra nunca.

---

### INV-801 — Seminario de Investigación: Metodología y Literatura Primaria

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–2–0 / 12 · **16 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | 90 créditos aprobados |
| **ADN institucional** | Seminario doctoral de MIT, CMU, Stanford y Berkeley, adaptado a pregrado |

**Competencia terminal.** Lee un paper de conferencia top identificando sus supuestos ocultos, replica su resultado central y escribe un paper propio evaluable por pares.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Lectura crítica | Protocolo de tres pasadas (Keshav) · Anatomía de un paper de conferencia · Identificación de la contribución real vs la declarada · Supuestos ocultos · Límites de validez |
| 2 | 4–7 | **Replicación I** | Selección de un paper con resultado empírico · Reconstrucción del experimento desde cero · Documentación de toda discrepancia con lo publicado |
| 3 | 8–11 | **Replicación II** | Segundo paper, área distinta · Análisis comparativo de la calidad de reporte entre ambos |
| 4 | 12–13 | Escritura científica | Estructura de un paper en NeurIPS, STOC, SOSP, OSDI, CCS o S&P · Redacción de la contribución · Trabajo relacionado · Reporte de resultados negativos |
| 5 | 14–16 | Revisión por pares | Proceso, criterios, conflictos de interés · Redacción de reviews · Rebuttal · Problemas abiertos: P vs NP, UGC, complejidad del Permanent · Ética: privacidad diferencial, fairness formal |

**Prueba de Dominio.** Dos replicaciones completas documentadas + un paper original de al menos 8 páginas en formato ACM/IEEE con contribución teórica o experimental novedosa, sometido a un proceso de revisión por pares simulado con criterios de conferencia real, incluyendo respuesta a los reviews.

**Bibliografía.**
- **Base:** *The Craft of Research* (5ª ed.) — Booth, Colomb, Williams et al.
- **Complementaria:** *Writing for Computer Science* (3ª ed.) — Zobel · *The Elements of Style* — Strunk & White
- **Papers:** *"How to Read a Paper"* — Keshav (SIGCOMM CCR 2007) · *"You and Your Research"* — Hamming (Bell Labs, 1986) · *"How to Write a Great Research Paper"* — Peyton Jones

**Recursos.** ACM Digital Library · IEEE Xplore · arXiv · ECCC · DBLP · Actas abiertas: USENIX, NeurIPS Proceedings, OpenReview · Zotero para gestión bibliográfica · Overleaf con plantillas ACM/IEEE.

**Protocolo de estudio.** Un paper replicado vale más que diez leídos. Cuota mínima del ciclo: **dos replicaciones completas desde cero**, con reporte explícito de las discrepancias encontradas. Las discrepancias son el resultado, no un fallo de la replicación.

---

### INV-802 — Proyecto de Investigación de Síntesis (Tesis)

| | |
|---|---|
| **Créditos** | 8 |
| **Carga** | 0–0–6 / 20 · **26 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | INV-801, 160 créditos aprobados |
| **ADN institucional** | MIT UROP · CMU Senior Thesis · Stanford Honors Program |

**Competencia terminal.** Produce y defiende una contribución original que sintetiza al menos tres áreas del programa.

**Fases**

| Fase | Sem. | Hito |
|---|---|---|
| 1 | 1–2 | Delimitación del problema y revisión del estado del arte · Identificación de la laguna |
| 2 | 3–4 | Formalización: definición precisa, modelo matemático, criterio de éxito falsable |
| 3 | 5–10 | Desarrollo: implementación del sistema o construcción de la prueba · Bitácora diaria fechada |
| 4 | 11–12 | Evaluación: diseño experimental, validación, búsqueda activa de contraejemplos |
| 5 | 13–14 | Análisis teórico: correctitud, complejidad, convergencia según corresponda |
| 6 | 15 | Redacción completa · Revisión por el asesor |
| 7 | 16 | **Defensa ante comité de ≥3 doctores** |

**Prueba de Dominio.** Tesis de 40–80 páginas con contribución original demostrable: algoritmo nuevo con análisis, resultado teórico nuevo, sistema nuevo evaluado rigurosamente, o prueba formal nueva. Defensa oral aprobada. Artefacto reproducible desde cero por un tercero.

**Requisitos de forma.** Sintetiza ≥3 áreas del programa. Todo resultado experimental acompañado de código, semillas y entorno. Toda afirmación teórica acompañada de su demostración completa o de la cita exacta si es conocida.

**Bibliografía.** Determinada por el tema. Mínimo 40 referencias primarias, de las cuales ≥15 de los últimos 5 años.

**Recursos.** Manual de estilo ACM o IEEE · Zenodo o repositorio institucional para el artefacto · Tesis de referencia de programas de honores en la ACM Digital Library.

**Protocolo de estudio.** Bitácora de investigación diaria y fechada, **con las hipótesis descartadas incluidas**. Las hipótesis muertas son el registro más valioso del proceso y el que sistemáticamente se pierde. Se evalúa con 15% del peso final (§7.3).

---

### Optativa de Profundización

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | variable · **≈14 h/sem** |
| **Prerrequisitos** | según la asignatura elegida |

Una asignatura de ≥4 créditos, aprobada por el comité, alineada con el tema de la tesis. Debe tener el mismo estándar de Prueba de Dominio que el resto del programa: un artefacto o demostración terminal, no un trabajo de lectura.

**Catálogo sugerido de optativas y su curso fuente:**

| Optativa | ADN institucional |
|---|---|
| Estructuras de Datos Avanzadas | MIT 6.851 (Demaine) |
| Gráficos por Computadora y Rendering Físico | MIT 6.837 · Stanford CS348 |
| Visión por Computador Geométrica | Stanford CS231A · CMU 16-720 |
| Robótica y Control Óptimo | CMU 16-745 · MIT 6.832 |
| Bioinformática Algorítmica | MIT 6.047 |
| Teoría de Juegos Algorítmica | Stanford CS364A (Roughgarden) |
| Privacidad Diferencial | Harvard CS208 · Penn |
| Bases de Datos Avanzadas y Nuevas Arquitecturas | CMU 15-721 (Pavlo) |
| Compiladores para Aprendizaje Automático | Stanford CS217 · MLIR/TVM |
| Criptografía Aplicada y Protocolos de Cómputo Seguro | Stanford CS355 · Berkeley CS294 |
| Teoría de Códigos Avanzada | Berkeley CS294 (Guruswami) |
| Arquitectura de Computadores Avanzada | CMU 18-740 · Berkeley CS252 |
---


# PARTE IV — RECURSOS

