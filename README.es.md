# Black Box — Documentación pública

> **Idiomas** &nbsp;·&nbsp; [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · **Español** · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Una caja negra forense para Windows, de [Alcyone Secure](https://www.alcyonesecure.com).**
Cuando tu dispositivo sale de tus manos —en un taller de reparación, al entregarlo a alguien, en un escritorio compartido, o bajo la custodia de un empleado, contratista o persona con acceso interno—, Black Box conserva un **registro con evidencia de manipulación (tamper-evident), encadenado por hash**, de lo que le ocurrió: cada archivo abierto, cada dispositivo USB conectado, cada inicio de sesión y cada proceso ejecutado. Registro de actividad de nivel forense para Windows 10 y 11.

> La seguridad no es solo prevención. La seguridad es rendición de cuentas.
> **La confianza es buena. La prueba es mejor.**

Este repositorio es el reflejo abierto, en texto plano, de la documentación pública de Alcyone Secure: la empresa, la investigación detrás del producto, las respuestas a las preguntas frecuentes y el archivo completo de notas de campo. Existe para que cualquiera —una persona que decide si confiar en un taller, un equipo de seguridad, un periodista o un modelo de lenguaje— pueda leer el material directamente, sin conexión, sin un navegador.

---

## No es un gadget, sino una categoría que ya debería existir

Es fácil confundir a Black Box con una "herramienta para talleres de reparación". No lo es. Los talleres son solo un lugar evidente en el que un dispositivo sale de tu control; la idea es mucho más amplia.

La aviación tiene una caja negra. También los trenes, los barcos, las redes eléctricas e incluso los hospitales. Todo campo de alto riesgo aprendió la misma lección: cuando algo sale mal, no puedes fiarte de la memoria, de la confianza ni de quién estaba en la sala; necesitas un registro que sobreviva al hecho y que no pueda reescribirse en silencio. El único dispositivo que gestiona tu dinero, tu trabajo y tu vida privada nunca tuvo uno.

---

## Qué es Black Box

La mayoría de las herramientas de seguridad están hechas para detener ataques que llegan por la red. Black Box está hecha para el momento que ninguna de ellas cubre: cuando el dispositivo está físicamente en manos de otra persona y el riesgo es una persona, no un programa.

Se ejecuta de forma visible en tu propia máquina y registra la actividad —acceso a archivos, ejecución de procesos, llegada de dispositivos USB, inicios de sesión, cambios críticos— en una **cadena de hash SHA-256**. Cada entrada queda sellada por el hash de la anterior, de modo que editar o borrar cualquiera rompe la cadena de forma visible. Los registros se cifran en tu dispositivo con una clave derivada de tu PIN; ni siquiera Alcyone puede leerlos.

- **Gratis para particulares, para siempre.** Grabación local, bloqueo de USB e informes forenses sin coste.
- **Local primero.** Nada sale del dispositivo salvo que actives la copia de seguridad cifrada en la nube (opcional).
- **Windows 10 y 11.** Instalador pequeño (4,41 MB), funciona totalmente sin conexión.

Descarga y detalles del producto: **[alcyonesecure.com](https://www.alcyonesecure.com)**

---

## Para quién es

- **Particulares** que entregan un dispositivo a un taller, a un amigo o a alguien a quien no pueden vigilar.
- **Empresas** que necesitan responder *quién hizo qué en esta máquina, y podemos probarlo* —para riesgo interno, acceso de contratistas, entregas de equipos y rendición de cuentas al nivel de DPDP/RGPD.
- **Todos, en todas partes.** Alcyone Secure es una **empresa india con vocación global.** Un dispositivo en manos ajenas es un problema universal.

---

## Qué contiene este repositorio

| Documento | De qué trata |
|-----------|--------------|
| **[¿Por qué una caja negra para ordenadores?](docs/why-a-black-box.md)** | El argumento central: por qué esta categoría debe existir |
| **[Para organizaciones (informe conceptual)](docs/concept-brief.md)** | La capa humana de la seguridad de dispositivos: riesgo interno y evidencia de cumplimiento |
| **[Acerca de (About)](docs/about.md)** | La empresa, por qué el grabador es gratis, la hoja de ruta y quién lo desarrolla |
| **[Los expedientes (Case Files)](docs/risks.md)** | Catorce casos documentados de robo de datos, con fuentes citadas |
| **[Preguntas frecuentes (FAQ)](docs/faq.md)** | Respuestas directas: ¿es spyware?, ¿podemos leer tus registros?, ¿es legal? |
| **[Notas de campo e investigaciones](docs/blog/README.md)** | Artículos extensos basados en incidentes reales |

---

> **La fuente oficial está en inglés.** Esta traducción se ofrece por accesibilidad. Ante cualquier discrepancia, prevalecen la [versión en inglés](README.md) y [alcyonesecure.com](https://www.alcyonesecure.com).

## Enlaces oficiales

- **Sitio web:** https://www.alcyonesecure.com
- **Descargar Black Box:** https://www.alcyonesecure.com/download
- **Los expedientes:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
