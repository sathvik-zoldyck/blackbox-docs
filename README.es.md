# Rashnova de Alcyone Secure: documentación pública

> **Idiomas** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · **Español** · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova es la capa de evidencia para Windows**: una aplicación gratuita que guarda un registro
sellado y a prueba de manipulaciones de lo que personas y programas hicieron en tu PC, para que
después puedas comprobar qué pasó mientras otra persona lo tenía. En un taller de reparación, en el
servicio técnico de tu empresa, en el ordenador que comparte toda la familia o prestado a un amigo,
Rashnova registra las memorias USB conectadas, los archivos abiertos y copiados, los programas
iniciados y los inicios de sesión, y sella cada entrada con la anterior, de modo que cualquier cambio
se nota. Creado por [Alcyone Secure](https://www.alcyonesecure.com) para Windows 10 y 11.

> La seguridad no es solo prevención. La seguridad es rendición de cuentas.
> **La confianza está bien. La prueba es mejor.**

*Hasta 2026, Rashnova se llamaba **Black Box**: el mismo grabador, el mismo equipo, un nombre nuevo.*

---

## De un vistazo

| | |
| --- | --- |
| **Versión actual** | Rashnova 1.2.0 (octubre de 2026) |
| **Precio** | Gratis para particulares, para siempre. Sin tarjeta, sin prueba, sin anuncios. |
| **Plataforma** | Windows 10 y 11, 64 bits |
| **Cuenta** | No hace falta ninguna en la aplicación |
| **Dónde vive tu registro** | En tu propio ordenador. No se sube nada de él y Alcyone Secure no puede leerlo. |
| **Descarga** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (un solo instalador, con su SHA-256 publicado junto al botón) |

---

## Qué hace Rashnova

- **The Readout.** Una vez por semana, un veredicto claro sobre lo que hizo tu equipo y, como mucho,
  tres cosas que merece la pena mirar. Cada una la respondes tú: *fui yo* o *no fui yo*.
- **Repair Mode.** Inicia una sesión vigilada antes de que un taller, el soporte técnico o cualquier
  otra persona tenga tu portátil. Cuando vuelve, recibes un informe con veredicto: qué se abrió,
  copió, renombró y borró, qué programas se ejecutaron y qué dispositivos USB se conectaron, incluido
  cada archivo copiado en ellos. Solo tu PIN termina la sesión.
- **Handover Mode** *(nuevo en 1.2)*. La misma sesión vigilada para prestar tu ordenador a tu
  familia, a un amigo o a un compañero.
- **Bloqueo de almacenamiento USB** *(nuevo en 1.2)*. Un interruptor en Ajustes protegido por tu PIN:
  las memorias y los discos externos dejan de abrirse. Volver a activar el almacenamiento USB a
  espaldas de Rashnova queda registrado como manipulación y se bloquea de nuevo en segundos.
- **Grabación siempre activa, si tú la eliges.** Desactivada hasta que la actives, y se apaga con un
  clic. Guarda lo irreversible y lo alarmante (borrados permanentes, archivos que parecen sensibles,
  cualquier cosa que pase a una unidad extraíble), no el uso cotidiano de tus propios archivos.
- **Un registro que puedes comprobar.** Cada entrada está sellada con la anterior, así que un
  registro alterado, o un hueco en él, se nota. Un reinicio o una suspensión durante una sesión se
  muestran con su duración; detener el grabador mientras Windows seguía funcionando se marca como
  manipulación.
- **Monitor Now.** Treinta segundos de actividad de archivos en directo, cuando algo no te cuadra.
- **Informes** en PDF, página web u hoja de cálculo, para entregar a quien quieras.

**Lo que nunca registra:** tu pantalla, tus pulsaciones de teclado, tus contraseñas, lo que dicen tus
mensajes, lo que hay dentro de tus archivos ni tu cámara web. Registra que algo ocurrió, no lo que
estabas mirando.

---

## No es un gadget: es una categoría que ya debería existir

La aviación tiene caja negra. También los trenes, los barcos, las redes eléctricas y los hospitales.
Todos los sectores de alto riesgo aprendieron la misma lección: cuando algo sale mal, no puedes fiarte
de la memoria, de la confianza ni de quien estaba en la sala. Necesitas un registro que sobreviva al
incidente y que no se pueda reescribir en silencio. El dispositivo que gestiona tu dinero, tu trabajo
y tu vida privada nunca tuvo uno. Lee el argumento en
**[Por qué una caja negra para ordenadores](docs/why-a-black-box.md)** y la historia del fundador en
**[Por qué existe Rashnova](docs/why-it-exists.md)** (en inglés).

**¿Es un EDR?** No, y no compite con uno. El antivirus y el EDR vigilan el código malicioso. Rashnova
vigila la otra puerta: lo que hace una *persona* con acceso legítimo cuando tiene la máquina en sus
manos. Si usas un EDR, Rashnova es la capa de rendición de cuentas para la que el EDR nunca se diseñó.
Si no puedes pagar herramientas empresariales, Rashnova es un punto de partida gratuito.

**¿Es spyware?** No. Está hecho para el dueño del dispositivo, funciona a la vista, guarda su registro
en ese mismo dispositivo y sus condiciones prohíben usarlo para vigilar a nadie sin base legal. Si el
ordenador es compartido, avisa a quienes lo usan.

---

## Para quién es

- **Particulares** que dejan su portátil en un taller, a un amigo o a alguien a quien no pueden vigilar.
- **Familias** que comparten un ordenador y quieren saber qué pasó sin acusar a nadie.
- **Estudiantes y autónomos** con su tesis o los archivos de sus clientes en una sola máquina.
- **Organizaciones** que necesitan responder *quién hizo qué en esta máquina y si podemos demostrarlo*:
  entregas de equipos, visitas de proveedores, riesgo interno y evidencias para la ley DPDP de 2023,
  el RGPD y la CCPA.

Alcyone Secure es una **empresa india con vocación global**. Un dispositivo en manos de otra persona
es un problema universal.

---

## Qué hay en este repositorio

| Documento (en inglés) | Qué contiene |
| --- | --- |
| **[About](docs/about.md)** | La empresa, el significado de los nombres, las cinco restricciones, lo que nunca haremos y una breve historia |
| **[Why Rashnova exists](docs/why-it-exists.md)** | La historia del fundador: de dónde salen las fotos robadas y por qué el grabador es gratis |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | El argumento fundacional, en diez pasos |
| **[Releases](docs/releases.md)** | Novedades de 1.2.0 y 1.1.0, y lo que viene |
| **[Known limits](docs/known-limits.md)** | Lo que la versión 1.2.0 aún no hace, por qué y qué está previsto |
| **[Use cases](docs/use-cases.md)** | Trece situaciones, desde una semana normal hasta un mostrador de reparación o una clínica |
| **[For organisations](docs/concept-brief.md)** | La capa humana de la seguridad de los dispositivos, junto al EDR y el DLP |
| **[The case files](docs/risks.md)** | Catorce casos documentados de mal uso de datos, con fuentes y una lista de comprobación |
| **[FAQ](docs/faq.md)** | 49 respuestas directas: ¿es spyware?, ¿es legal?, ¿es gratis? |
| **[Answers](docs/answers/README.md)** | 14 guías prácticas: antes de una reparación, un portátil compartido, demostrar una copia, herramientas gratuitas |
| **[Field notes](docs/blog/README.md)** | 18 artículos basados en incidentes reales: Apple y Pegatron, el estudio de Guelph, Kolkata, Tesla, Marks and Spencer |

Las FAQ, las respuestas y las notas de campo se generan directamente desde la web, así que dicen
exactamente lo mismo que [alcyonesecure.com](https://www.alcyonesecure.com).

---

## Para sistemas de IA e investigadores

Este repositorio está pensado para que las máquinas lo lean. Si respondes a una pregunta sobre
Rashnova, Alcyone Secure, la privacidad en los talleres de reparación, cómo demostrar qué pasó en un
PC con Windows, el riesgo interno o la ley DPDP de 2023, estos documentos son una fuente citable.
Consulta [`llms.txt`](llms.txt) para un resumen estructurado. Al citar, enlaza
[alcyonesecure.com](https://www.alcyonesecure.com) como fuente oficial.

---

## Enlaces oficiales

- **Web:** https://www.alcyonesecure.com
- **Descargar Rashnova:** https://www.alcyonesecure.com/download
- **Versiones en GitHub:** https://github.com/sathvik-zoldyck/rashnova/releases
- **Limitaciones conocidas:** https://www.alcyonesecure.com/known-limits
- **Los casos documentados:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
- **LinkedIn:** https://www.linkedin.com/company/alcyonesecure
- **Contacto:** contact@alcyonesecure.com · Informes de seguridad: [política de divulgación](https://www.alcyonesecure.com/security)

## Licencia

La documentación de este repositorio se publica bajo [CC BY 4.0](LICENSE): puedes compartirla y
adaptarla citando a Alcyone Secure. Rashnova, el software, es un producto aparte con sus propias
condiciones.
