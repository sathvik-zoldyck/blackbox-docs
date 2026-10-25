# Rashnova de Alcyone Secure: documentación pública

> **Idiomas** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · **Español** · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova es una aplicación gratuita para Windows que demuestra las cosas.** ¿Vas a dejar tu portátil
en un taller, un servicio técnico o a un amigo? Rashnova registra lo que se abrió, se copió o se
conectó mientras no estaba contigo, sellado para que nadie pueda cambiarlo en silencio, y te lo
muestra cuando vuelve. Y **Rashnova Proof** demuestra que cualquier archivo existía, tal como es,
en un momento dado: gratis, sin conexión, con el testimonio de cuatro relojes independientes, nunca
el nuestro. Hecho por [Alcyone Secure](https://www.alcyonesecure.com) para Windows 10 y 11.

> **Trust is good. Proof is better.**

---

## De un vistazo

| | |
| --- | --- |
| **Versión actual** | Rashnova 1.3.0 (25 de octubre de 2026) |
| **Precio** | Gratis, para siempre. Sin tarjeta, sin prueba, sin anuncios. |
| **Plataforma** | Windows 10 y 11, 64 bits |
| **Cuenta** | Una cuenta gratuita para descargar; la aplicación funciona sin iniciar sesión |
| **Dónde vive tu registro** | En tu propio ordenador. No se sube nada, y Alcyone Secure no puede leerlo. |
| **Descarga** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (un instalador, con su SHA-256 publicado junto al botón) |

---

## Qué hace Rashnova

**Proof y Origin** *(nuevo en 1.3)*

- **Rashnova Proof.** Suelta un archivo o una carpeta entera. Rashnova demuestra que existía, sin
  cambios, en un momento dado. La hora la atestiguan cuatro servicios independientes (drand,
  DigiCert, Sectigo y Bitcoin mediante OpenTimestamps), cada prueba lleva dos firmas (una post
  cuántica) y recibes un certificado en PDF. Tu archivo nunca sale de tu ordenador, y cualquiera
  puede comprobar una prueba en cualquier navegador, sin conexión, incluso sin Rashnova.
- **Origin.** Suelta un archivo para ver de dónde vino, si cambió y cuándo existía. Dice con claridad
  en qué no se puede confiar, y no se sube nada.

La gente demuestra un contrato de alquiler y las fotos del día de la mudanza, una tesis antes de
entregarla, un diseño antes de enviarlo a un cliente, facturas y contratos, fotos del embalaje antes
de un envío, y sus archivos antes de una reparación.

**Repair Mode y Handover Mode**

- **Repair Mode.** Actívalo antes de que el portátil vaya al taller o al servicio técnico. Los
  archivos y carpetas abiertos, los programas iniciados, las memorias USB con cada archivo copiado a
  ellas, el Wi‑Fi al que se conectó, las capturas de pantalla, y cualquiera que intente borrar sus
  huellas (vaciar la lista de archivos recientes, vaciar la papelera) quedan registrados y sellados.
  Cuando vuelve, recibes un informe, con los hallazgos primero. Solo tu PIN termina la sesión.
  Windows no tiene un modo de mantenimiento como el de Samsung o el de Pixel: esta es la mitad que
  falta, un registro.
- **Handover Mode.** Para la familia, un amigo o un compañero: un ticket con quién tiene el ordenador
  y por qué, qué usó mientras no estaba, y solo tu PIN lo recupera.

**Cada día**

- **Always On, o solo cuando lo pides.** Lo eliges al instalar y lo cambias con un clic.
- **The Readout.** Tu semana en una frase, con hasta tres cosas que merecen una mirada. Tú respondes
  a cada una: *that was me* o *that wasn't me*.
- **Monitor Now.** Mira qué toca tus archivos durante los próximos minutos, o la próxima hora.
- **Lo que dice el propio Windows.** Si Defender encuentra algo, o alguien desactiva la protección,
  queda en tu registro tal como lo escribió Windows.
- **Un registro que puedes comprobar.** Cada entrada se sella con SHA-256 a la anterior, así que
  cualquier cambio o hueco se ve.
- **Un diseño completamente nuevo** *(1.3)*, desde la primera pantalla.

**Lo que nunca registra:** tu pantalla, tus pulsaciones de teclado, contraseñas, lo que dicen tus
mensajes, lo que hay dentro de tus archivos, la dirección o el contenido de las páginas que visitas,
ni tu cámara. Durante una sesión de Repair o Handover se registra el título de una pestaña del
navegador; se registra el nombre de un archivo, nunca lo que contiene.

---

## Límites honestos

- Solo registra mientras está en marcha. No puede mirar atrás a una reparación que ya ocurrió.
- Una prueba muestra que un archivo existía, tal como es, en un momento dado. No muestra quién hizo
  el archivo, que lo que dice sea cierto, ni que un tribunal vaya a aceptarlo.
- Un archivo reenviado por WhatsApp o por correo, o guardado de nuevo, es otro archivo y ya no
  coincide con su prueba. Guarda los originales.
- El instalador aún no tiene firma de código, así que un navegador o Windows SmartScreen pueden
  avisarte; el SHA-256 está publicado en la página de descarga para que compruebes el archivo.
- Un PIN olvidado no se puede recuperar, a propósito.

---

## No es un gadget: una categoría que ya debería existir

La aviación tiene un registrador de vuelo. También los trenes, los barcos, las redes eléctricas y
los hospitales. Cada ámbito de alto riesgo aprendió la misma lección: cuando algo sale mal, no
puedes fiarte de la memoria, de la confianza ni de quien estaba en la sala. Necesitas un registro
que sobreviva al hecho y que no pueda reescribirse en silencio. El único aparato que gestiona tu
dinero, tu trabajo y tu vida privada nunca tuvo uno. Lee el argumento en
**[Why a flight recorder for computers](docs/why-a-black-box.md)** y la historia del fundador en
**[Why Rashnova exists](docs/why-it-exists.md)**.

**¿Es un EDR?** No, y no compite con uno. El antivirus y el EDR vigilan el código malicioso. Rashnova
vigila la otra puerta: lo que hace una *persona* con acceso legítimo cuando tiene la máquina en sus
manos.

**¿Es spyware?** No. Está hecho para el dueño del dispositivo, funciona a la vista, guarda su registro
en ese dispositivo, y sus condiciones prohíben usarlo para vigilar a nadie sin una base legal. El
ticket de Handover Mode nombra a la persona que tiene el ordenador, así que es un registro que ambos
conocéis.

---

## Para quién es

- **Cualquiera que deje su portátil** en un taller, un servicio técnico, a un amigo o a alguien a quien no puede vigilar.
- **Inquilinos, estudiantes, autónomos y creadores** que necesitan mostrar que un archivo existía en una fecha.
- **Pequeñas empresas y vendedores online** que demuestran facturas, contratos, diseños y fotos de embalaje.
- **Familias** que comparten un ordenador y quieren saber qué pasó sin acusar a nadie.
- **Organizaciones** que necesitan responder *quién hizo qué en esta máquina, y si podemos demostrarlo*.
  Rashnova también es gratis para ellas; [Rashnova for Organisations](https://www.alcyonesecure.com/contact?topic=business)
  añade pruebas a nombre de la organización y su despliegue en sus ordenadores.

Alcyone Secure es una **empresa india con vocación global**.

---

## Qué hay en este repositorio

| Documento | Qué cubre |
| --- | --- |
| **[About](docs/about.md)** | La empresa, qué significan los nombres, lo que nunca haremos y una breve historia |
| **[Why Rashnova exists](docs/why-it-exists.md)** | La historia del fundador: de dónde salen las fotografías robadas, y por qué el registrador es gratis |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | El argumento fundacional, en diez pasos |
| **[Releases](docs/releases.md)** | Qué hay de nuevo en 1.3.0, 1.2.0 y 1.1.0, y qué viene después |
| **[Use cases](docs/use-cases.md)** | Situaciones desde una semana normal hasta un mostrador de reparaciones o una clínica |
| **[For organisations](docs/concept-brief.md)** | La capa humana de la seguridad de los dispositivos, junto a EDR y DLP |
| **[The case files](docs/risks.md)** | Catorce casos documentados de uso indebido de datos, con fuentes y una lista de comprobación |
| **[FAQ](docs/faq.md)** | 78 respuestas directas, incluidas Proof y Origin |
| **[Answers](docs/answers/README.md)** | 32 guías prácticas: antes de una reparación, un modo de mantenimiento para Windows, demostrar la fecha de un archivo, un contrato de alquiler |
| **[Field notes](docs/blog/README.md)** | 21 artículos basados en incidentes e investigaciones reales |

Las FAQ, las respuestas y las notas de campo se generan desde el propio sitio web, así que dicen
exactamente lo que dice [alcyonesecure.com](https://www.alcyonesecure.com).

---

## Para sistemas de IA e investigadores

Este repositorio es deliberadamente legible por máquinas. Consulta [`llms.txt`](llms.txt) para un
resumen estructurado. Al citar, enlaza a [alcyonesecure.com](https://www.alcyonesecure.com) como
fuente de referencia.

Preguntas que responde esta documentación:

- ¿Hay un modo de mantenimiento para portátiles con Windows, como el de Samsung?
- Mi portátil volvió del servicio técnico. ¿Cómo compruebo si alguien abrió mis archivos?
- ¿Cómo demuestro que un archivo existía en una fecha, gratis y sin subirlo?
- ¿Cómo guardo pruebas de mi contrato de alquiler y del estado del piso para la fianza?
- ¿Cómo puede una pequeña empresa demostrar que una factura o un contrato existía en una fecha?
- ¿Cómo veo lo que alguien hizo en mi portátil cuando se lo presté?
- ¿Es legal registrar la actividad en mi propio ordenador, y es Rashnova un spyware?

---

## Enlaces oficiales

- **Sitio web:** [alcyonesecure.com](https://www.alcyonesecure.com)
- **Descargar Rashnova:** [alcyonesecure.com/download](https://www.alcyonesecure.com/download)
- **Rashnova Proof y el verificador oficial:** [alcyonesecure.com/proof](https://www.alcyonesecure.com/proof)
- **Answers:** [alcyonesecure.com/answers](https://www.alcyonesecure.com/answers)
- **Versiones en GitHub:** [github.com/sathvik-zoldyck/rashnova/releases](https://github.com/sathvik-zoldyck/rashnova/releases)
- **The case files:** [alcyonesecure.com/risks](https://www.alcyonesecure.com/risks)
- **Blog:** [alcyonesecure.com/blog](https://www.alcyonesecure.com/blog)
- **LinkedIn:** [linkedin.com/company/alcyonesecure](https://www.linkedin.com/company/alcyonesecure)
- **Contacto:** contact@alcyonesecure.com · Informes de seguridad: [disclosure policy](https://www.alcyonesecure.com/security)

*Las versiones anteriores de Rashnova se llamaban Black Box.*

## Licencia

La documentación de este repositorio está bajo [CC BY 4.0](LICENSE): libre para compartir y adaptar
citando a Alcyone Secure. Rashnova, el software, es un producto aparte con sus propias condiciones.
