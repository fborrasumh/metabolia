# MetabolIA

Bioquímica II (1024, Grado en Medicina): problemas con solución calculada, test tipo examen y tutor con IA. Aplicación web de un solo fichero (`index.html`), sin servidor.

**Usar la app:** https://fborrasumh.github.io/metabolia/

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23591721.svg)](https://doi.org/10.5281/zenodo.23591721)

**Idiomas:** español (por defecto), inglés y portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

App de estudio de **Bioquímica II (código 1024)**, segundo semestre del primer curso del Grado en Medicina de la Universidad Miguel Hernández de Elche, construida a partir de su guía docente oficial del curso 2026-2027.

- **Temario de la guía:** unidades, temas y objetivos de aprendizaje copiados literalmente de la guía, con la asociación objetivo-unidad que fija la propia guía.
- **11 tipos de problemas con solución calculada por código:** ΔG°′ de transferencias redox, ATP de la fosforilación oxidativa, rendimiento en ATP de glucosa, glucógeno, piruvato, lactato y acetil-CoA (con lanzaderas), coste de la gluconeogénesis, β-oxidación de ácidos grasos saturados e insaturados, cuerpos cetónicos, coste del ciclo de la urea, balance nitrogenado, gasto energético (Mifflin-St Jeor), energía de una comida y cociente respiratorio. Cada tipo genera variantes reproducibles a partir de una semilla; acepta coma o punto decimal, tolera un redondeo pequeño y reconoce errores típicos declarados para cada problema (cocientes invertidos, ln en lugar de log, relaciones P/O antiguas, factores olvidados, unidades desplazadas un factor 1000, signos…), explicando cuál se ha cometido. Pista conceptual y solución paso a paso.
- **Test tipo examen:** 25 preguntas de cinco opciones (en tres idiomas), con las reglas de la guía: +1 por acierto, −0,20 por error, 0 en blanco. Modos por unidad, simulacro y repaso espaciado (cajas de Leitner).
- **Tutor con IA que no da la respuesta:** responde con una explicación breve y una pregunta guía. No recibe la solución del problema y, además, el código elimina cualquier frase que contenga una cifra de la solución o de un paso intermedio, o que anuncie «la respuesta es…». Si cita la guía, el código comprueba que la cita existe literalmente.
- **Preguntas nuevas con IA:** se aceptan solo si tienen cinco opciones distintas, una respuesta válida, explicación y una cita literal de la guía; llevan la etiqueta «IA · sin revisar».
- **Progreso** por unidad y por objetivo de la guía; informe en Word, CSV y copia de seguridad JSON (sin claves).
- **Ejemplo sin clave** que muestra el tutor con una fuga de la solución eliminada por el código.

## Cómo se usa la IA

Es opcional: temario, problemas, tests y progreso funcionan sin IA y sin conexión. Para el tutor y las preguntas nuevas, cada persona usa su propia clave de OpenAI, Google Gemini o Anthropic Claude, que se guarda solo en su navegador.

## Privacidad

Todo el progreso se guarda en el navegador (IndexedDB). Solo sale hacia el proveedor de IA lo que se envía al tutor o al generar preguntas: el mensaje del estudiante (con correos, DNI y teléfonos enmascarados), el enunciado del problema y fragmentos públicos de la guía docente. Antes del primer envío de cada sesión se muestra una muestra de lo que sale y se pide confirmación.

## Límites

- No sustituye a las clases, a las prácticas ni a la bibliografía de la guía.
- Los problemas usan los modelos simplificados de los libros de texto (constantes de pKa a 25 °C, P/O de 2,5 y 1,5, carga por grupo totalmente protonado o desprotonado, etc.).
- El diagnóstico de errores reconoce solo los errores típicos declarados; otros errores se marcan como «no es correcto» sin explicación específica.
- Las explicaciones del tutor y las preguntas generadas por IA pueden contener errores conceptuales que el código no puede detectar: el código verifica las citas y las cifras, no la corrección científica de cada frase.
- Las traducciones al inglés y al portugués no han sido revisadas por hablantes nativos.
- Probado con IA simulada (OpenAI, Gemini y Claude) en Chromium de escritorio y móvil; no se ha probado con una clave real.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche), Luis Miguel Gutiérrez Pérez (Universidad Miguel Hernández de Elche), José Heliodoro Villanueva Roig (Universidad Miguel Hernández de Elche) y Juan Antonio Reig Macià (Universidad Miguel Hernández de Elche).

A partir de la guía docente de Bioquímica II (código 1024) del Grado en Medicina de la UMH, curso 2026-2027, y de su profesorado.

ORCID: Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573) · Luis Miguel Gutiérrez Pérez [0000-0002-0512-7858](https://orcid.org/0000-0002-0512-7858) · José Heliodoro Villanueva Roig [0000-0002-4057-2113](https://orcid.org/0000-0002-4057-2113) · Juan Antonio Reig Macià [0000-0002-5947-7183](https://orcid.org/0000-0002-5947-7183)

## Cómo citar

Borrás Rocher, Fernando; Gutiérrez Pérez, Luis Miguel; Villanueva Roig, José Heliodoro; Reig Macià, Juan Antonio (2026). *MetabolIA* (v1.0.0) [Software]. DOI: [10.5281/zenodo.23591721](https://doi.org/10.5281/zenodo.23591721)

## Licencia

MIT. Véase [LICENSE](LICENSE).
