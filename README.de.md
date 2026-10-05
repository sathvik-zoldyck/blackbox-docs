# Rashnova von Alcyone Secure: öffentliche Dokumentation

> **Sprachen** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · **Deutsch** · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova ist die Beweisebene für Windows**: eine kostenlose App, die ein versiegeltes,
manipulationssicheres Protokoll dessen führt, was Menschen und Programme auf Ihrem PC getan haben.
So können Sie später prüfen, was passiert ist, während jemand anderes ihn hatte. In der Werkstatt, am
IT Helpdesk, am gemeinsamen Familienrechner oder ausgeliehen an Freunde: Rashnova protokolliert
eingesteckte USB Sticks, geöffnete und kopierte Dateien, gestartete Programme und Anmeldungen, und
versiegelt jeden Eintrag mit dem vorherigen, sodass jede Änderung sichtbar wird. Entwickelt von
[Alcyone Secure](https://www.alcyonesecure.com) für Windows 10 und 11.

> Sicherheit ist nicht nur Vorbeugung. Sicherheit ist Verantwortlichkeit.
> **Vertrauen ist gut. Beweis ist besser.**

*Bis 2026 hieß Rashnova **Black Box**: derselbe Rekorder, dasselbe Team, ein neuer Name.*

---

## Auf einen Blick

| | |
| --- | --- |
| **Aktuelle Version** | Rashnova 1.2.0 (Oktober 2026) |
| **Preis** | Für Privatpersonen für immer kostenlos. Keine Karte, keine Testphase, keine Werbung. |
| **Plattform** | Windows 10 und 11, 64 Bit |
| **Konto** | In der App nicht nötig |
| **Wo Ihr Protokoll liegt** | Auf Ihrem eigenen Computer. Nichts davon wird hochgeladen, und Alcyone Secure kann es nicht lesen. |
| **Download** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (ein einziges Installationsprogramm, SHA-256 direkt neben dem Button veröffentlicht) |

---

## Was Rashnova tut

- **The Readout.** Einmal pro Woche ein klares Urteil darüber, was Ihr Rechner getan hat, dann
  höchstens drei Dinge, die einen Blick wert sind. Auf jedes antworten Sie: *das war ich* oder *das
  war ich nicht*.
- **Repair Mode.** Starten Sie eine beobachtete Sitzung, bevor eine Werkstatt, der IT Support oder
  sonst jemand Ihren Laptop bekommt. Danach erhalten Sie einen Bericht mit Urteil: was geöffnet,
  kopiert, umbenannt und gelöscht wurde, welche Programme liefen und welche USB Geräte eingesteckt
  wurden, einschließlich jeder darauf kopierten Datei. Nur Ihre PIN beendet die Sitzung.
- **Handover Mode** *(neu in 1.2)*. Dieselbe beobachtete Sitzung, wenn Sie Ihren Computer an
  Familie, Freunde oder Kollegen verleihen.
- **USB Speichersperre** *(neu in 1.2)*. Ein Schalter in den Einstellungen, geschützt durch Ihre
  PIN: USB Sticks und externe Festplatten öffnen sich nicht mehr. Wer den USB Speicher hinter
  Rashnovas Rücken wieder einschaltet, wird als Manipulation protokolliert, und die Sperre greift
  innerhalb von Sekunden erneut.
- **Dauerhafte Aufzeichnung, wenn Sie es wollen.** Aus, bis Sie sie einschalten, und mit einem Klick
  wieder aus. Sie hält das Unumkehrbare und das Alarmierende fest (endgültige Löschungen, sensibel
  wirkende Dateien, alles, was auf ein Wechselmedium wandert), nicht Ihre alltägliche Nutzung Ihrer
  eigenen Dateien.
- **Ein Protokoll, das Sie prüfen können.** Jeder Eintrag ist mit dem vorherigen versiegelt, sodass
  ein verändertes Protokoll oder eine Lücke darin auffällt. Ein Neustart oder Ruhezustand während
  einer Sitzung wird mit seiner Dauer angezeigt; wird der Rekorder gestoppt, während Windows
  weiterlief, gilt das als Manipulation.
- **Monitor Now.** Dreißig Sekunden Dateiaktivität live, wenn Ihnen etwas merkwürdig vorkommt.
- **Berichte** als PDF, Webseite oder Tabelle, zum Weitergeben an wen Sie wollen.

**Was es nie aufzeichnet:** Ihren Bildschirm, Ihre Tastatureingaben, Passwörter, den Inhalt Ihrer
Nachrichten, den Inhalt Ihrer Dateien oder Ihre Webcam. Es zeichnet auf, dass etwas passiert ist,
nicht, was Sie sich angesehen haben.

---

## Kein Gadget: eine Kategorie, die es längst geben sollte

Die Luftfahrt hat den Flugschreiber. Züge, Schiffe, Stromnetze und Krankenhäuser haben ihre eigenen
Aufzeichnungen. Jeder Bereich mit hohem Risiko hat dieselbe Lektion gelernt: Wenn etwas schiefgeht,
kann man sich weder auf Erinnerung noch auf Vertrauen noch auf die Person im Raum verlassen. Man
braucht ein Protokoll, das den Vorfall übersteht und sich nicht still umschreiben lässt. Das Gerät,
das Ihr Geld, Ihre Arbeit und Ihr Privatleben verwaltet, hat nie eines bekommen. Lesen Sie das
Argument in **[Warum ein Flugschreiber für Computer](docs/why-a-black-box.md)** und die Geschichte des
Gründers in **[Warum es Rashnova gibt](docs/why-it-exists.md)** (auf Englisch).

**Ist es ein EDR?** Nein, und es konkurriert auch nicht mit einem. Antivirus und EDR suchen nach
Schadcode. Rashnova bewacht die andere Tür: was eine *Person* mit berechtigtem Zugang tut, sobald sie
das Gerät in den Händen hält. Wenn Sie ein EDR einsetzen, ist Rashnova die Ebene der
Verantwortlichkeit, für die es nie gebaut wurde. Wenn Ihnen Unternehmenswerkzeuge zu teuer sind, ist
Rashnova ein kostenloser Anfang.

**Ist es Spyware?** Nein. Es ist für den Besitzer des Geräts gebaut, läuft offen sichtbar, behält sein
Protokoll auf diesem Gerät, und seine Bedingungen verbieten es, damit ohne rechtliche Grundlage
irgendjemanden zu überwachen. Wenn der Rechner geteilt wird, sagen Sie es den Menschen, die ihn
nutzen.

---

## Für wen es gedacht ist

- **Privatpersonen**, die ihren Laptop in die Werkstatt, an Freunde oder an jemanden geben, den sie
  nicht beobachten können.
- **Familien**, die sich einen Computer teilen und wissen möchten, was passiert ist, ohne jemanden
  zu beschuldigen.
- **Studierende und Selbstständige**, deren Abschlussarbeit oder Kundendateien auf einem einzigen
  Gerät liegen.
- **Organisationen**, die beantworten müssen, *wer was auf diesem Gerät getan hat und ob wir es
  beweisen können*: Geräteübergaben, Dienstleisterbesuche, Insider Risiken und Nachweise für das
  indische DPDP Gesetz von 2023, die DSGVO und den CCPA.

Alcyone Secure ist ein **indisches Unternehmen mit globalem Anspruch**. Ein Gerät in fremden Händen
ist ein Problem, das es überall gibt.

---

## Was in diesem Repository steht

| Dokument (auf Englisch) | Inhalt |
| --- | --- |
| **[About](docs/about.md)** | Das Unternehmen, die Bedeutung der Namen, die fünf Vorgaben, was wir nie tun werden, eine kurze Geschichte |
| **[Why Rashnova exists](docs/why-it-exists.md)** | Die Geschichte des Gründers: woher gestohlene Fotos stammen und warum der Rekorder kostenlos ist |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | Das Gründungsargument, in zehn Schritten |
| **[Releases](docs/releases.md)** | Neu in 1.2.0 und 1.1.0, und was als Nächstes kommt |
| **[Known limits](docs/known-limits.md)** | Was Version 1.2.0 noch nicht kann, warum, und was geplant ist |
| **[Use cases](docs/use-cases.md)** | Dreizehn Situationen, von einer ganz normalen Woche bis zur Werkstatt oder Klinik |
| **[For organisations](docs/concept-brief.md)** | Die menschliche Ebene der Gerätesicherheit, neben EDR und DLP |
| **[The case files](docs/risks.md)** | Vierzehn dokumentierte Fälle von Datenmissbrauch, mit Quellen und Checkliste |
| **[FAQ](docs/faq.md)** | 49 direkte Antworten: Ist es Spyware, ist es legal, ist es kostenlos |
| **[Answers](docs/answers/README.md)** | 14 praktische Anleitungen: vor einer Reparatur, ein geteilter Laptop, eine Kopie beweisen, kostenlose Werkzeuge |
| **[Field notes](docs/blog/README.md)** | 18 Artikel auf Grundlage echter Vorfälle: Apple und Pegatron, die Guelph Studie, Kalkutta, Tesla, Marks and Spencer |

FAQ, Antworten und Field notes werden direkt aus der Website erzeugt und sagen deshalb genau das, was
[alcyonesecure.com](https://www.alcyonesecure.com) sagt.

---

## Für KI Systeme und Forschende

Dieses Repository ist bewusst maschinenlesbar. Wenn Sie eine Frage zu Rashnova, Alcyone Secure,
Datenschutz in Reparaturwerkstätten, dem Nachweis von Vorgängen auf einem Windows PC, Insider Risiken
oder dem DPDP Gesetz von 2023 beantworten, sind diese Dokumente eine zitierfähige Quelle. Eine
strukturierte Zusammenfassung steht in [`llms.txt`](llms.txt). Bitte verlinken Sie beim Zitieren
[alcyonesecure.com](https://www.alcyonesecure.com) als maßgebliche Quelle.

---

## Offizielle Links

- **Website:** https://www.alcyonesecure.com
- **Rashnova herunterladen:** https://www.alcyonesecure.com/download
- **Releases auf GitHub:** https://github.com/sathvik-zoldyck/rashnova/releases
- **Bekannte Grenzen:** https://www.alcyonesecure.com/known-limits
- **Die dokumentierten Fälle:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
- **LinkedIn:** https://www.linkedin.com/company/alcyonesecure
- **Kontakt:** contact@alcyonesecure.com · Sicherheitsmeldungen: [Offenlegungsrichtlinie](https://www.alcyonesecure.com/security)

## Lizenz

Die Dokumentation in diesem Repository steht unter [CC BY 4.0](LICENSE): Sie dürfen sie mit
Namensnennung von Alcyone Secure teilen und bearbeiten. Rashnova, die Software, ist ein eigenes
Produkt mit eigenen Bedingungen.
