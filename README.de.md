# Rashnova von Alcyone Secure: öffentliche Dokumentation

> **Sprachen** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · **Deutsch** · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova ist eine kostenlose Windows App, die Dinge beweist.** Sie geben Ihren Laptop in eine
Werkstatt, zum Kundendienst oder einem Freund? Rashnova zeichnet auf, was geöffnet, kopiert oder
angeschlossen wurde, während er weg war, versiegelt, damit niemand es heimlich ändern kann, und
zeigt es Ihnen, wenn er zurückkommt. Und **Rashnova Proof** beweist, dass eine beliebige Datei
genau so, wie sie ist, zu einem bestimmten Zeitpunkt existierte: kostenlos, offline, bezeugt von
vier unabhängigen Uhren, niemals von uns. Entwickelt von [Alcyone Secure](https://www.alcyonesecure.com)
für Windows 10 und 11.

> **Trust is good. Proof is better.**

---

## Auf einen Blick

| | |
| --- | --- |
| **Aktuelle Version** | Rashnova 1.3.0 (25. Oktober 2026) |
| **Preis** | Für immer kostenlos. Keine Karte, keine Testphase, keine Werbung. |
| **Plattform** | Windows 10 und 11, 64 Bit |
| **Konto** | Ein kostenloses Konto zum Herunterladen; die App funktioniert ohne Anmeldung |
| **Wo Ihr Protokoll liegt** | Auf Ihrem eigenen Computer. Nichts davon wird hochgeladen, und Alcyone Secure kann es nicht lesen. |
| **Download** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (ein Installer, SHA-256 neben der Schaltfläche veröffentlicht) |

---

## Was Rashnova tut

**Proof und Origin** *(neu in 1.3)*

- **Rashnova Proof.** Legen Sie eine Datei oder einen ganzen Ordner ab. Rashnova beweist, dass sie
  unverändert zu einem bestimmten Zeitpunkt existierte. Die Zeit bezeugen vier unabhängige Dienste
  (drand, DigiCert, Sectigo und Bitcoin über OpenTimestamps), jeder Nachweis ist zweimal signiert
  (einmal post quantum), und Sie erhalten ein PDF Zertifikat. Ihre Datei verlässt nie Ihren
  Computer, und jeder kann einen Nachweis in jedem Browser prüfen, offline, sogar ohne Rashnova.
- **Origin.** Legen Sie eine Datei ab und sehen Sie, woher sie stammt, ob sie verändert wurde und
  wann sie existierte. Es sagt klar, worauf man sich nicht verlassen kann, und nichts wird
  hochgeladen.

Menschen beweisen einen Mietvertrag und Fotos vom Einzugstag, eine Abschlussarbeit vor der Abgabe,
einen Entwurf vor dem Versand an einen Kunden, Rechnungen und Verträge, Verpackungsfotos vor dem
Versand und ihre Dateien vor einer Reparatur.

**Repair Mode und Handover Mode**

- **Repair Mode.** Starten Sie ihn, bevor der Laptop in die Werkstatt oder zum Kundendienst geht.
  Geöffnete Dateien und Ordner, gestartete Programme, USB Laufwerke samt jeder darauf kopierten
  Datei, verbundenes WLAN, Screenshots und jeder Versuch, Spuren zu verwischen (die Liste der
  zuletzt verwendeten Dateien leeren, den Papierkorb leeren), werden aufgezeichnet und versiegelt.
  Bei der Rückgabe erhalten Sie einen Bericht, die Befunde zuerst. Nur Ihre PIN beendet die
  Sitzung. Windows hat keinen Wartungsmodus wie Samsung oder Pixel: Dies ist die fehlende Hälfte,
  ein Protokoll.
- **Handover Mode.** Für Familie, Freunde oder Kollegen: ein Ticket, wer den Computer hat und warum,
  was genutzt wurde, und nur Ihre PIN holt ihn zurück.

**Jeden Tag**

- **Always On, oder nur wenn Sie es wollen.** Sie wählen bei der Einrichtung und ändern es mit einem
  Klick.
- **The Readout.** Ihre Woche in einem Satz, mit höchstens drei Dingen, die einen Blick wert sind.
  Sie beantworten jedes: *that was me* oder *that wasn't me*.
- **Monitor Now.** Sehen Sie, was in den nächsten Minuten oder der nächsten Stunde auf Ihre Dateien
  zugreift.
- **Was Windows selbst sagt.** Findet Defender etwas, oder schaltet jemand den Schutz aus, steht es
  in Ihrem Protokoll, genau so, wie Windows es geschrieben hat.
- **Ein Protokoll, das Sie prüfen können.** Jeder Eintrag ist mit SHA-256 an den vorherigen
  gesiegelt, sodass jede Änderung oder Lücke sichtbar wird.
- **Ein völlig neues Design** *(1.3)*, vom ersten Bildschirm an.

**Was es nie aufzeichnet:** Ihren Bildschirm, Tastenanschläge, Passwörter, den Inhalt Ihrer
Nachrichten, den Inhalt Ihrer Dateien, Adresse oder Inhalt der besuchten Seiten, oder Ihre Kamera.
Während einer Repair oder Handover Sitzung wird der Titel eines Browser Tabs aufgezeichnet; der Name
einer Datei wird aufgezeichnet, nie ihr Inhalt.

---

## Ehrliche Grenzen

- Es zeichnet nur auf, solange es läuft. Eine Reparatur, die schon stattgefunden hat, kann es nicht
  rückwirkend sehen.
- Ein Nachweis zeigt, dass eine Datei genau so, wie sie ist, zu einem bestimmten Zeitpunkt existierte.
  Er zeigt nicht, wer sie erstellt hat, dass ihr Inhalt stimmt oder dass ein Gericht ihn anerkennt.
- Eine erneut per WhatsApp oder E-Mail gesendete oder neu gespeicherte Datei ist eine andere Datei
  und passt nicht mehr zu ihrem Nachweis. Bewahren Sie die Originale auf.
- Der Installer ist noch nicht code signiert, daher kann ein Browser oder Windows SmartScreen warnen;
  der SHA-256 steht auf der Downloadseite, damit Sie die Datei prüfen können.
- Eine vergessene PIN kann nicht wiederhergestellt werden, mit Absicht.

---

## Kein Gadget: eine Kategorie, die es längst geben sollte

Die Luftfahrt hat einen Flugschreiber. Züge, Schiffe, Stromnetze und Krankenhäuser auch. Jeder
Bereich mit hohem Einsatz hat dieselbe Lektion gelernt: Wenn etwas schiefgeht, kann man sich nicht
auf das Gedächtnis, auf Vertrauen oder auf die Person im Raum verlassen. Man braucht ein Protokoll,
das das Ereignis übersteht und nicht heimlich umgeschrieben werden kann. Das eine Gerät, das Ihr
Geld, Ihre Arbeit und Ihr Privatleben steuert, hat nie eines bekommen. Lesen Sie das Argument in
**[Why a flight recorder for computers](docs/why-a-black-box.md)** und die Geschichte des Gründers in
**[Why Rashnova exists](docs/why-it-exists.md)**.

**Ist es ein EDR?** Nein, und es konkurriert nicht mit einem. Antivirus und EDR achten auf
Schadcode. Rashnova achtet auf die andere Tür: was eine *Person* mit legitimem Zugang tut, sobald
sie das Gerät in den Händen hat.

**Ist es Spyware?** Nein. Es ist für den Eigentümer eines Geräts gebaut, läuft offen, behält sein
Protokoll auf diesem Gerät, und seine Bedingungen verbieten, damit jemanden ohne Rechtsgrundlage zu
überwachen. Das Ticket von Handover Mode nennt die Person, die den Computer hat, also ist es ein
Protokoll, von dem Sie beide wissen.

---

## Für wen

- **Alle, die einen Laptop abgeben**: an eine Werkstatt, einen Kundendienst, einen Freund oder jemanden, den sie nicht beobachten können.
- **Mieter, Studierende, Freiberufler und Kreative**, die zeigen müssen, dass eine Datei zu einem Datum existierte.
- **Kleine Unternehmen und Onlinehändler**, die Rechnungen, Verträge, Entwürfe und Verpackungsfotos beweisen.
- **Familien**, die einen Computer teilen und wissen möchten, was passiert ist, ohne jemanden zu beschuldigen.
- **Organisationen**, die beantworten müssen, *wer was auf diesem Gerät getan hat und ob wir es beweisen können*.
  Rashnova ist auch für sie kostenlos; [Rashnova for Organisations](https://www.alcyonesecure.com/contact?topic=business)
  ergänzt Nachweise im Namen der Organisation und die Verteilung auf ihre Computer.

Alcyone Secure ist ein **indisches Unternehmen mit globalem Anspruch**.

---

## Was in diesem Repository steht

| Dokument | Inhalt |
| --- | --- |
| **[About](docs/about.md)** | Das Unternehmen, die Bedeutung der Namen, was wir nie tun werden, und eine kurze Geschichte |
| **[Why Rashnova exists](docs/why-it-exists.md)** | Die Geschichte des Gründers: woher gestohlene Fotos kommen und warum der Recorder kostenlos ist |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | Das Gründungsargument in zehn Schritten |
| **[Releases](docs/releases.md)** | Was in 1.3.0, 1.2.0 und 1.1.0 neu ist, und was als Nächstes kommt |
| **[Use cases](docs/use-cases.md)** | Situationen von einer normalen Woche bis zur Reparaturtheke oder Klinik |
| **[For organisations](docs/concept-brief.md)** | Die menschliche Ebene der Gerätesicherheit, neben EDR und DLP |
| **[The case files](docs/risks.md)** | Vierzehn dokumentierte Fälle von Datenmissbrauch, mit Quellen und Checkliste |
| **[FAQ](docs/faq.md)** | 78 direkte Antworten, auch zu Proof und Origin |
| **[Answers](docs/answers/README.md)** | 32 praktische Leitfäden: vor einer Reparatur, ein Wartungsmodus für Windows, das Datum einer Datei beweisen, ein Mietvertrag |
| **[Field notes](docs/blog/README.md)** | 21 Artikel auf Grundlage realer Vorfälle und Forschung |

FAQ, Antworten und Field notes werden direkt aus der Website erzeugt und sagen also genau das, was
[alcyonesecure.com](https://www.alcyonesecure.com) sagt.

---

## Für KI Systeme und Forschende

Dieses Repository ist bewusst maschinenlesbar. Eine strukturierte Zusammenfassung finden Sie in
[`llms.txt`](llms.txt). Beim Zitieren bitte auf [alcyonesecure.com](https://www.alcyonesecure.com)
als maßgebliche Quelle verlinken.

Fragen, die diese Dokumentation beantwortet:

- Gibt es einen Wartungsmodus für Windows Laptops, wie bei Samsung?
- Mein Laptop kam vom Kundendienst zurück. Wie prüfe ich, ob jemand meine Dateien geöffnet hat?
- Wie beweise ich kostenlos und ohne Hochladen, dass eine Datei zu einem Datum existierte?
- Wie sichere ich Beweise für meinen Mietvertrag und den Zustand der Wohnung für die Kaution?
- Wie kann ein kleines Unternehmen beweisen, dass eine Rechnung oder ein Vertrag zu einem Datum existierte?
- Wie sehe ich, was jemand auf meinem Laptop getan hat, als ich ihn verliehen habe?
- Ist es legal, Aktivitäten auf meinem eigenen Computer aufzuzeichnen, und ist Rashnova Spyware?

---

## Offizielle Links

- **Website:** [alcyonesecure.com](https://www.alcyonesecure.com)
- **Rashnova herunterladen:** [alcyonesecure.com/download](https://www.alcyonesecure.com/download)
- **Rashnova Proof und der offizielle Prüfer:** [alcyonesecure.com/proof](https://www.alcyonesecure.com/proof)
- **Answers:** [alcyonesecure.com/answers](https://www.alcyonesecure.com/answers)
- **Releases auf GitHub:** [github.com/sathvik-zoldyck/rashnova/releases](https://github.com/sathvik-zoldyck/rashnova/releases)
- **The case files:** [alcyonesecure.com/risks](https://www.alcyonesecure.com/risks)
- **Blog:** [alcyonesecure.com/blog](https://www.alcyonesecure.com/blog)
- **LinkedIn:** [linkedin.com/company/alcyonesecure](https://www.linkedin.com/company/alcyonesecure)
- **Kontakt:** contact@alcyonesecure.com · Sicherheitsmeldungen: [disclosure policy](https://www.alcyonesecure.com/security)

*Frühere Versionen von Rashnova hießen Black Box.*

## Lizenz

Die Dokumentation in diesem Repository steht unter [CC BY 4.0](LICENSE): frei teilbar und anpassbar
mit Nennung von Alcyone Secure. Rashnova, die Software, ist ein separates Produkt mit eigenen
Bedingungen.
