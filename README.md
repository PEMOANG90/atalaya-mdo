# Atalaya MDO

Suite académica de análisis para operaciones multidominio. Un solo archivo (`index.html`) que corre en el navegador, sin IA, sin servidores y sin conexión.

**Sitio:** https://pemoang90.github.io/atalaya-mdo/

## Uso rápido

Pega una noticia en **Análisis rápido** y pulsa **Analizar noticia**. El sitio muestra qué se afectó, qué puede venir después, qué hacer primero y qué tan confiable parece la noticia, con un reporte listo para copiar o imprimir.

Los cuatro módulos se alimentan de la misma noticia: la cascada (M1) califica los cursos de acción (M3) y prepara un ejercicio de mesa (M2) que arranca con la noticia; la confiabilidad del texto (M4) ajusta la legitimidad y el peso de la comunicación.

## Fuentes abiertas

El botón **Consultar fuentes abiertas** busca, sin claves ni cuentas, información pública relacionada con la noticia:

| Fuente | Qué aporta |
| --- | --- |
| GDELT | Cobertura en medios de los últimos 7 días (corroboración) |
| Open-Meteo | Viento, lluvia y oleaje en el lugar detectado |
| NOAA SWPC | Clima espacial (afectación a GPS y satélites) |
| USGS | Sismos cercanos de magnitud 4.5 o mayor |
| NASA EONET | Eventos naturales activos en la región |
| Wikipedia | Contexto del lugar |

Las condiciones relevantes (oleaje alto, ráfagas fuertes, tormenta geomagnética, sismo cercano) se agregan automáticamente al análisis de los cuatro módulos. Solo se envían el lugar y palabras clave, no el texto completo.

## Módulos avanzados

| Módulo | Qué hace |
| --- | --- |
| **M1 · Cascada multidominio** | Describe el incidente con tus palabras o elige uno de ejemplo. Mapa de 20 infraestructuras en 6 dominios (espacial, ciberespacio, terrestre, marítimo, aéreo y cognitivo). Simula cómo se propaga una falla, con cronología, puntos de estrangulamiento y la mitigación de mayor efecto. |
| **M2 · Ejercicio de mesa** | Seis turnos con eventos en distintos dominios, decisiones con consecuencias diferidas y una evaluación final con bitácora. |
| **M3 · Cursos de acción** | Matriz de decisión ponderada con prueba de sensibilidad de los pesos. |
| **M4 · Dominio cognitivo** | Marca en un texto las señales de manipulación narrativa y sugiere pasos de verificación. |

Cada módulo genera un reporte que puede copiarse, imprimirse o guardarse como PDF.

## Aviso

Proyecto académico. Los modelos, pesos, escenarios y textos de ejemplo son ficticios y simplificados; los resultados son propuestas para discusión, no predicciones ni evaluaciones oficiales.
