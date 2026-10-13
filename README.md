# Atalaya MDO

Suite académica de análisis para operaciones multidominio. Un solo archivo (`index.html`) que corre en el navegador, sin IA, sin servidores y sin conexión.

**Sitio:** https://pemoang90.github.io/atalaya-mdo/

## Uso rápido

Pega una noticia, o solo su enlace, en **Análisis rápido** y pulsa **Analizar noticia**. Con un enlace, la herramienta lee el contenido: notas web (vía Jina Reader o AllOrigins), publicaciones de X (vía FxTwitter o vxTwitter, incluida la nota que enlacen) y videos de YouTube (título y canal). El enlace funciona igual en Cascada, Cursos de acción y Dominio cognitivo, y el resultado se analiza en todos los módulos. El sitio muestra qué se afectó, qué puede venir después, qué hacer primero y qué tan confiable parece la noticia, con un reporte listo para copiar o imprimir.

¿No tienes la noticia? Debajo del cuadro de texto puedes buscarla. La búsqueda internacional lee directo el RSS de cadenas como CNN en Español, BBC Mundo, DW, France 24, El País, Europa Press, Euronews, Infobae, CNN International, Al Jazeera, The Guardian y South China Morning Post; la nacional usa Google Noticias México. Ambas se filtran filtrada por dominio (terrestre, marítimo, aéreo, espacial, ciberespacio, cognitivo) y con palabra clave opcional. El botón **Analizar** de cada resultado la pasa directo al análisis.

Los cuatro módulos se alimentan de la misma noticia: la cascada (M1) califica los cursos de acción (M3) y prepara un ejercicio de mesa (M2) que arranca con la noticia; la confiabilidad del texto (M4) ajusta la legitimidad y el peso de la comunicación.

## Fuentes abiertas

El botón **Consultar fuentes abiertas** busca, sin claves ni cuentas, información pública relacionada con la noticia:

| Fuente | Qué aporta |
| --- | --- |
| GDELT y Google Noticias | Cobertura en medios de los últimos 7 días (corroboración); si GDELT no responde se usa Google Noticias |
| Open-Meteo | Viento, lluvia y oleaje en el lugar detectado |
| NOAA SWPC | Clima espacial (afectación a GPS y satélites) |
| USGS | Sismos cercanos de magnitud 4.5 o mayor |
| NASA EONET | Eventos naturales activos en la región |
| Wikipedia | Contexto del lugar |

Las condiciones relevantes (oleaje alto, ráfagas fuertes, tormenta geomagnética, sismo cercano) se agregan automáticamente al análisis de los cuatro módulos. Solo se envían el lugar y palabras clave, no el texto completo.

## Imágenes satelitales y fuentes oficiales

- **Entorno geográfico satelital:** mapa interactivo del lugar con imagen de alta resolución (Esri) o la imagen del día anterior de NASA (MODIS), con los sismos y eventos naturales cercanos marcados. Incluye la imagen GOES más reciente de México y las perspectivas de ciclones tropicales del Atlántico y del Pacífico (NOAA/NHC).
- **Fuentes oficiales:** SEMAR (meteorología marítima y comunicados), CONAGUA (Servicio Meteorológico Nacional) y Protección Civil (CNPC, Atlas Nacional de Riesgos y SASMEX). Como no publican datos que una página web pueda leer, el sitio enlaza a su portal y a una búsqueda de sus avisos recientes sobre el lugar, y marca como prioritarias las que corresponden a la noticia.

## M5 · Panorama en vivo

Mapa de conciencia situacional en tiempo real, inspirado en tableros OSINT como Osiris, centrado en el lugar de la noticia:

| Capa | Fuente | Actualización |
| --- | --- | --- |
| Aeronaves (ADS-B) | adsb.lol, respaldos airplanes.live, adsb.fi y OpenSky | 30 s |
| Buques (AIS) | AISStream (clave gratuita del usuario) | continuo |
| Satélites GPS | CelesTrak + satellite.js | 10 s |
| Sismos 24 h | USGS | 5 min |
| Eventos naturales | NASA EONET | 10 min |
| Radar de lluvia | RainViewer | 10 min |
| Noticias | Google Noticias | 5 min |

Genera alertas (códigos de emergencia aérea 7500/7600/7700, sismos M5+, tormentas o incendios en la zona, buques detenidos, pocos satélites GPS visibles) que se pueden agregar al análisis de la noticia con un clic.

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
