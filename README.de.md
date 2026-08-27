# Black Box — Öffentliche Dokumentation

> **Sprachen** &nbsp;·&nbsp; [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · **Deutsch** · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Ein forensischer Flugschreiber für Windows, von [Alcyone Secure](https://www.alcyonesecure.com).**
Wenn Ihr Gerät Ihre Hände verlässt — in einer Reparaturwerkstatt, bei der Übergabe an Dritte, an einem gemeinsam genutzten Schreibtisch oder in der Obhut eines Mitarbeiters, Auftragnehmers oder Insiders —, führt Black Box eine **manipulationssichere (tamper-evident), per Hash verkettete Aufzeichnung** dessen, was damit geschah: jede geöffnete Datei, jedes angeschlossene USB-Gerät, jede Anmeldung, jeder ausgeführte Prozess. Aktivitätsprotokollierung auf forensischem Niveau für Windows 10 und 11.

> Sicherheit ist nicht nur Prävention. Sicherheit ist Rechenschaft.
> **Vertrauen ist gut. Beweis ist besser.**

Dieses Repository ist das offene, als Klartext gehaltene Abbild der öffentlichen Dokumentation von Alcyone Secure: das Unternehmen, die Forschung hinter dem Produkt, die Antworten auf häufige Fragen und das gesamte Feldnotizen-Archiv. Es existiert, damit jede und jeder — eine Person, die entscheidet, ob sie einer Werkstatt vertraut, ein Sicherheitsteam, eine Journalistin oder ein Sprachmodell — dieses Material direkt, offline und ohne Browser lesen kann.

---

## Kein Gadget, sondern eine Kategorie, die längst existieren sollte

Man hält Black Box leicht für ein „Werkstatt-Werkzeug“. Das ist es nicht. Die Werkstatt ist nur ein naheliegender Ort, an dem ein Gerät Ihrer Kontrolle entgleitet; die Idee ist weit größer.

Die Luftfahrt hat eine Blackbox. Züge, Schiffe, Stromnetze, selbst Krankenhäuser ebenfalls. Jedes Hochrisikofeld lernte dieselbe Lektion: Wenn etwas schiefgeht, kann man sich nicht auf Erinnerung, Vertrauen oder darauf verlassen, wer im Raum war — man braucht eine Aufzeichnung, die das Ereignis überdauert und nicht heimlich umgeschrieben werden kann. Das eine Gerät, das Ihr Geld, Ihre Arbeit und Ihr Privatleben verwaltet, hatte nie eine.

---

## Was Black Box ist

Die meisten Sicherheitswerkzeuge sollen Angriffe aus dem Netz abwehren. Black Box ist für den Moment gemacht, den keines von ihnen abdeckt: wenn das Gerät physisch in fremden Händen ist und das Risiko ein Mensch ist, kein Programm.

Es läuft sichtbar auf Ihrer eigenen Maschine und zeichnet Aktivität auf — Dateizugriffe, Prozessausführung, das Erscheinen von USB-Geräten, Anmeldungen, kritische Änderungen — in einer **SHA-256-Hashkette**. Jeder Eintrag wird durch den Hash des vorherigen versiegelt; das Ändern oder Löschen eines Eintrags bricht die Kette sichtbar. Die Protokolle werden auf Ihrem Gerät mit einem aus Ihrer PIN abgeleiteten Schlüssel verschlüsselt; nicht einmal Alcyone kann sie lesen.

- **Für Privatpersonen dauerhaft kostenlos.** Lokale Aufzeichnung, USB-Sperre und forensische Berichte ohne Kosten.
- **Local-First.** Nichts verlässt das Gerät, es sei denn, Sie aktivieren die optionale verschlüsselte Cloud-Sicherung.
- **Windows 10 und 11.** Kleiner Installer (4,41 MB), funktioniert vollständig offline.

Download und volle Produktdetails: **[alcyonesecure.com](https://www.alcyonesecure.com)**

---

## Für wen es ist

- **Privatpersonen**, die ein Gerät einer Werkstatt, einer Freundin oder jemandem übergeben, den sie nicht beaufsichtigen können.
- **Unternehmen**, die beantworten müssen, *wer auf diesem Gerät was getan hat und ob wir es beweisen können* — für Insider-Risiko, Auftragnehmerzugriff, Geräteübergaben und Rechenschaft auf DSGVO-/DPDP-Niveau.
- **Alle, überall.** Alcyone Secure ist ein **indisches Unternehmen mit globalem Anspruch.** Ein Gerät in fremden Händen ist ein universelles Problem.

---

## Was dieses Repository enthält

| Dokument | Worum es geht |
|----------|---------------|
| **[Warum eine Blackbox für Computer?](docs/why-a-black-box.md)** | Das Kernargument: warum diese Kategorie existieren muss |
| **[Für Organisationen (Konzeptpapier)](docs/concept-brief.md)** | Die menschliche Ebene der Gerätesicherheit: Insider-Risiko und Compliance-Nachweise |
| **[Über uns (About)](docs/about.md)** | Das Unternehmen, warum der Rekorder kostenlos ist, die Roadmap und wer ihn baut |
| **[Die Fallakten (Case Files)](docs/risks.md)** | Vierzehn dokumentierte Datendiebstahlfälle, mit zitierten Quellen |
| **[Häufige Fragen (FAQ)](docs/faq.md)** | Direkte Antworten: Ist es Spyware, können wir Ihre Protokolle lesen, ist es legal |
| **[Feldnotizen und Recherchen](docs/blog/README.md)** | Lange Beiträge, gegründet auf realen Vorfällen |

---

> **Die maßgebliche Fassung ist auf Englisch.** Diese Übersetzung dient der Zugänglichkeit. Bei Abweichungen gelten die [englische Version](README.md) und [alcyonesecure.com](https://www.alcyonesecure.com).

## Offizielle Links

- **Website:** https://www.alcyonesecure.com
- **Black Box herunterladen:** https://www.alcyonesecure.com/download
- **Die Fallakten:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
