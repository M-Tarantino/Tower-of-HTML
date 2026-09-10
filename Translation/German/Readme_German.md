# Tower of HTML

> **Mache HTML-Bildung universell zugänglich — unabhängig von Hardware, Internetverbindung oder dem Alter des Geräts.**

**Tower of HTML** ist eine minimalistische, Offline-First-Bildungsplattform, die entwickelt wurde, um HTML-Grundlagen von Grund auf zu vermitteln. Die gesamte Anwendung befindet sich in einer einzigen, in sich geschlossenen `.html`-Datei ohne externe Abhängigkeiten, Frameworks, Build-Schritte oder Server-Anforderungen.

---

## 📋 Inhaltsverzeichnis

- [Design-Philosophie & Kernmission](#design-philosophie--kernmission)
- [Hauptmerkmale](#hauptmerkmale)
- [Universelle Barrierefreiheit & Hardware-Kompatibilität](#universelle-barrierefreiheit--hardware-kompatibilität)
- [Erste Schritte](#erste-schritte)
- [Architektur & Mechanik](#architektur--mechanik)
- [Lernpfad (51 Etagen)](#lernpfad-51-etagen)
- [Level-Code-Progressionssystem](#level-code-progressionssystem)
- [Anpassungs- & Erweiterungsrichtlinien](#anpassungs--erweiterungsrichtlinien)
- [Sprachübersetzungsfortschritt](#sprachübersetzungsfortschritt)
- [Technische Spezifikationen](#technische-spezifikationen)
- [Lizenz & Autor](#lizenz--autor)

---

## 🎯 Design-Philosophie & Kernmission

### Das Problem, das wir lösen
Die meisten modernen Webentwicklungs-Lernplattformen stellen erhebliche Hürden dar:
1. **Abhängigkeit von Internetverbindung**: Online-IDEs und LMS-Plattformen versagen in Umgebungen mit geringer Bandbreite oder ohne Internetverbindung.
2. **Anforderungen an moderne Hardware**: Moderne Tools erfordern moderne Betriebssysteme, viel Arbeitsspeicher und schwere Browser-Engines, wodurch Nutzer mit älterer Hardware ausgeschlossen werden.
3. **Komplexitätsoverhead**: Anfänger sind oft mit Build-Tools, Frameworks und Paketmanagern überfordert, bevor sie auch nur eine einzige Zeile HTML schreiben.
4. **Vendor-Lock-in**: Der Fortschritt der Nutzer hängt von der Verfügbarkeit von Drittanbieterplattformen und der obligatorischen Erstellung von Konten ab.

### Unsere Lösung
Tower of HTML basiert auf vier Kernverpflichtungen:
* **Barrierefreiheit vor Features**: Priorisiert rohe Kompatibilität und klare Lesbarkeit gegenüber UI-Frameworks.
* **Bildung vor Unterhaltung**: Strukturierte, etagenweise Progression, bei der die Beherrschung durch strenge, faire Validierung erarbeitet wird.
* **Eigentum vor Plattformen**: Nutzer können das Projekt unbegrenzt besitzen, herunterladen, modifizieren und ausführen, ohne um Erlaubnis zu bitten.
* **Klarheit vor Raffinesse**: Geschrieben in klarem, lesbarem Code ohne Verschleierung oder Transpilierung, damit Lernende direkt aus dem Quellcode inspizieren und lernen können.

---

## ✨ Hauptmerkmale

* **100 % Offline-First**: Läuft lokal in jedem Webbrowser, ohne Netzwerkzugriff zu erfordern.
* **Einzeldatei-Architektur**: Alles (CSS, JS, Inhalt) befindet sich in einer einzigen, portablen `index.html`-Datei (~50 KB).
* **Unterstützung für Legacy-Engines**: Entwickelt mit legacy-sicherem JavaScript (ES3/ES5-Standard), um eine funktionale Ausführung auf älterer Hardware sicherzustellen.
* **Keine Abhängigkeiten**: Frei von externen Bibliotheken, Paketmanagern, Schriftarten oder CDN-Links.
* **Level-Code-System**: Ein einfacher Passwort-Hash-Mechanismus ermöglicht es Nutzern, den Fortschritt in jedem Browser oder auf jedem Gerät ohne lokalen Speicher fortzusetzen.
* **Terminal-Themes**: Anpassbare visuelle Modi (Matrix, Amber, DOS Blue, Light, Cyber), die direkt in der Benutzeroberfläche zugänglich sind.

---

## 🌐 Universelle Barrierefreiheit & Hardware-Kompatibilität

Da Tower of HTML in legacy-sicherem JavaScript ohne moderne Web-Abhängigkeiten geschrieben ist, läuft es zuverlässig auf einem breiten Spektrum von Geräten und Betriebssystemen:

| Gerät / Plattform | Betriebsstatus | Hinweise |
| :--- | :---: | :--- |
| **1995 Pentium PC** | ✅ Unterstützt | Windows 95/98, Internet Explorer 6+ |
| **Chromebooks** | ✅ Unterstützt | Alle Chrome-Browser-Versionen |
| **Legacy Mobile (iPhone 4S / Android 4.0)** | ✅ Unterstützt | Native mobile Browser (Safari 5+, Android WebKit) |
| **Moderne Laptops & Desktops** | ✅ Unterstützt | Chrome, Firefox, Safari, Edge, Opera |
| **Raspberry Pi** | ✅ Unterstützt | Leichte Browser-Engines |
| **Ressourcenarme Bildungslabore** | ✅ Unterstützt | Keine Administratorrechte oder Installation erforderlich |

Dieses Design ermöglicht es Pädagogen in ressourcenarmen Umgebungen, das Projekt einmal herunterzuladen und über USB oder lokale Dateifreigabe an Schüler zu verteilen.

---

## 🚀 Erste Schritte

1. Laden Sie die `index.html`-Datei herunter oder speichern Sie sie auf Ihrem Gerät.
2. Doppelklicken Sie auf `index.html` (oder öffnen Sie sie mit einem beliebigen Webbrowser).
3. Lesen Sie die Anweisung für die aktuelle Etage, geben Sie Ihr HTML-Snippet in das Eingabefeld ein und klicken Sie auf **CHECK CODE**.
4. Schreiben Sie nach Abschluss einer Etage den generierten **Level Code** auf oder kopieren Sie ihn, um Ihren Fortschritt in zukünftigen Sitzungen oder auf anderen Geräten fortzusetzen.

---

## 🏗️ Architektur & Mechanik

Die einzelne `index.html`-Datei trennt die Ausführungslogik strikt vom Lehrmaterial und behält dabei eine abhängigkeitsfreie Umgebung bei:


index.html
├── <head>
│   └── <style> : Terminal-Styling, responsive Layouts, visuelle Themes
└── <body>
├── UI-Container : Spielbildschirm, Eingabeterminal, Ausgabeansicht
└── <script>
├── levels[] Array : Reine Text-Lehrdaten & Validierungsregeln
└── Engine-Logik   : DOM-Updates, Level-Code-Verifizierung, Fortschrittsstatus

### Design-Verpflichtungen
- **Inline-CSS**: Eingebettet in einen einzigen `<style>`-Block.
- **Inline-JavaScript**: Eingebettet in einen einzigen `<script>`-Block.
- **ES3/ES5-Standard**: Verwendet Standard-Schleifenkonstrukte und ES3/ES5-Syntax (`var`, `for`-Schleifen) anstelle moderner ES6+-Funktionen, die eine Transpilierung erfordern.

---

## 📚 Lernpfad (51 Etagen)

Der Lehrplan besteht aus 51 strukturierten Etagen, die sich über sechs verschiedene Phasen erstrecken:


Fähigkeitsprogression:
Anfänger (Etagen 0–8)          → Tags, schließende Tags und Seitenstruktur
Mittelstufe (Etagen 9–28)      → Formatierung, Links, Buttons und Medien
Fortgeschritten (Etagen 29–48) → Bereiche, Listen, Formulare, Tabellen und Attribute
Profi (Etagen 49–51)          → Dokumentdeklarationen, Zeichensätze und finale Integration

### Phase 1: Grundlagen (Etagen 0–8)
| Etage | Code | Titel | Aufgabe / Konzept |
| :---: | :--- | :--- | :--- |
| **0** | `START` | Übersicht & Anweisungen | Spieleinführung & Steuerung |
| **1** | `L1-ROOT` | Das Stammelement | `<html>`-Tag-Erstellung |
| **2** | `L2-HEAD` | Der Kopfbereich | `<head>`-Metadatencontainer |
| **3** | `L3-TITLE` | Seitentitel | `<title>`-Tab-Benennung |
| **4** | `L4-BODY` | Der Hauptteil | `<body>`-Inhaltsbereich |
| **5** | `L5-PARA` | Absätze | `<p>`-Textstruktur |
| **6** | `L6-CLOSE-P` | Schließendes Absatz-Tag | `</p>`-Tag-Schließung |
| **7** | `L7-CLOSE-BODY` | Schließendes Body-Tag | `</body>`-Tag-Schließung |
| **8** | `L8-CLOSE-HTML` | Schließendes HTML-Tag | `</html>`-Tag-Schließung |

### Phase 2: Inhalt & Text (Etagen 9–18)
| Etage | Code | Titel | Aufgabe / Konzept |
| :---: | :--- | :--- | :--- |
| **9** | `L9-H1` | Hauptüberschrift (H1) | `<h1>`-Überschriftenebene 1 |
| **10** | `L10-H2` | Unterüberschrift (H2) | `<h2>`-Überschriftenebene 2 |
| **11** | `L11-CLOSE-H1` | Schließendes Überschriften-Tag | `</h1>`-Schließtag |
| **12** | `L12-BOLD` | Fettgedruckter Text | `<b>`-Präsentationsfett |
| **13** | `L13-CLOSE-BOLD` | Schließendes Fett-Tag | `</b>`-Tag-Schließung |
| **14** | `L14-ITALIC` | Kursiver Text | `<i>`-Präsentationskursiv |
| **15** | `L15-CLOSE-ITALIC` | Schließendes Kursiv-Tag | `</i>`-Tag-Schließung |
| **16** | `L16-STRONG` | Starke Hervorhebung | `<strong>`-semantische Hervorhebung |
| **17** | `L17-CLOSE-STRONG` | Schließendes Stark-Tag | `</strong>`-Tag-Schließung |
| **18** | `L18-EM` | Hervorhebung | `<em>`-semantische Betonung |

### Phase 3: Links & Medien (Etagen 19–28)
| Etage | Code | Titel | Aufgabe / Konzept |
| :---: | :--- | :--- | :--- |
| **19** | `L19-ANCHOR` | Link-Tag | `<a>`-Anker-Element |
| **20** | `L20-HREF` | Link-Ziel | `<a href="...">`-Attributnutzung |
| **21** | `L21-CLOSE-ANCHOR` | Schließendes Link-Tag | `</a>`-Tag-Schließung |
| **22** | `L22-IMG` | Bildelement | `<img>`-Bildcontainer |
| **23** | `L23-SRC` | Bildquelle | `<img src="...">`-Attributnutzung |
| **24** | `L24-ALT` | Alt-Text | Barrierefreiheitsattribut (`alt="..."`) |
| **25** | `L25-BR` | Zeilenumbruch | Selbstschließender Umbruch `<br>` |
| **26** | `L26-HR` | Horizontale Linie | `<hr>`-Trennlinie |
| **27** | `L27-BUTTON` | Button-Element | Interaktives Element `<button>` |
| **28** | `L28-CLOSE-BUTTON` | Schließendes Button-Tag | `</button>`-Tag-Schließung |

### Phase 4: Organisation (Etagen 29–38)
| Etage | Code | Titel | Aufgabe / Konzept |
| :---: | :--- | :--- | :--- |
| **29** | `L29-DIV` | Divisions-Container | `<div>`-Blockcontainer |
| **30** | `L30-CLOSE-DIV` | Schließendes DIV-Tag | `</div>`-Tag-Schließung |
| **31** | `L31-SPAN` | Span-Element | `<span>`-Inline-Container |
| **32** | `L32-CLOSE-SPAN` | Schließendes Span-Tag | `</span>`-Tag-Schließung |
| **33** | `L33-UL` | Ungeordnete Liste | `<ul>`-Aufzählungslisten-Container |
| **34** | `L34-LI` | Listenelement | `<li>`-Element |
| **35** | `L35-CLOSE-LI` | Schließendes Listenelement | `</li>`-Tag-Schließung |
| **36** | `L36-OL` | Geordnete Liste | `<ol>`-Nummerierungslisten-Container |
| **37** | `L37-CLOSE-UL` | Schließende ungeordnete Liste | `</ul>`-Tag-Schließung |
| **38** | `L38-CLOSE-OL` | Schließende geordnete Liste | `</ol>`-Tag-Schließung |

### Phase 5: Fortgeschritten & Experte (Etagen 39–48)
| Etage | Code | Titel | Aufgabe / Konzept |
| :---: | :--- | :--- | :--- |
| **39** | `L39-FORM` | Formular-Container | `<form>`-Eingabe-Wrapper |
| **40** | `L40-CLOSE-FORM` | Schließendes Formular-Tag | `</form>`-Tag-Schließung |
| **41** | `L41-INPUT` | Eingabefeld | Selbstschließendes Feld `<input>` |
| **42** | `L42-TABLE` | Datentabelle | `<table>`-Container |
| **43** | `L43-TR` | Tabellenzeile | `<tr>`-Zeilenelement |
| **44** | `L44-TD` | Tabellenzelle | `<td>`-Datenzellenelement |
| **45** | `L45-CLOSE-TABLE` | Schließendes Tabellen-Tag | `</table>`-Tag-Schließung |
| **46** | `L46-COMMENT` | HTML-Kommentare | `<!-- comment -->`-Syntax |
| **47** | `L47-CLASS` | Class-Attribut | `class="..."`-Styling-Ziel |
| **48** | `L48-ID` | ID-Attribut | `id="..."`-Eindeutiges Ziel |

### Phase 6: Finale Herausforderung (Etagen 49–51)
| Etage | Code | Titel | Aufgabe / Konzept |
| :---: | :--- | :--- | :--- |
| **49** | `L49-DOCTYPE` | Dokumenttyp | `<!DOCTYPE html>`-Deklaration |
| **50** | `L50-META-CHARSET` | Zeichenkodierung | `<meta charset="UTF-8">`-Metadaten |
| **51** | `L51-COMPLETE` | **FINALER BOSS** | Erstelle eine vollständige, gültige Webseite |

---

## 🔑 Level-Code-Progressionssystem

Anstatt sich auf Browser-Speicher-APIs (`localStorage`, `indexedDB` oder Cookies) zu verlassen, wird der Fortschritt über kurze, menschenlesbare **Level-Codes** gespeichert.

### Wie es funktioniert
1. Nach Abschluss einer Etage zeigt die Anwendung einen eindeutigen Code an (z. B. `L5-PARA`).
2. Nutzer können den Code kopieren, speichern oder aufschreiben.
3. In späteren Sitzungen lädt die Eingabe des Codes in das Feld **JUMP TO FLOOR** sofort den Zustand dieser Etage.

### Vorteile
- **Browser- und geräteübergreifend**: Nahtloser Wechsel zwischen einem alten Mobiltelefon und einem Desktop-Computer.
- **Kein Datenschutz-Footprint**: Funktioniert ohne Verfolgung von Nutzern, Speicherung von Cookies oder Durchführung von Web-Anfragen.
- **Keine API-Abhängigkeiten**: Funktioniert auf Browsern, die vor der Existenz von Local-Storage-Spezifikationen erstellt wurden.

---

## 🛠️ Anpassungs- & Erweiterungsrichtlinien

Da die gesamte Anwendungslogik in einem sauberen JavaScript-Array gespeichert ist, erfordert das Hinzufügen oder Modifizieren von Etagen die Bearbeitung des `levels`-Arrays innerhalb von `index.html`.

### Hinzufügen einer neuen Etage

```javascript
{
    id: "L52-HEADER",
    title: "Floor 52: Header Semantic Element",
    info: "The <header> tag represents introductory content or navigation links.",
    hint: "Type <header> to open the header section.",
    desc: "Create an opening header tag.",
    check: function(input) {
        var clean = input.toLowerCase().replace(/\s+/g, '');
        return clean.indexOf("<header>") !== -1;
    }
}

Validierungs-Designrichtlinien
Halten Sie beim Hinzufügen von Validierungsregeln die universellen Kompatibilitätsregeln des Projekts ein:
 * Standard-String-Operationen verwenden: Verlassen Sie sich auf Methoden wie .indexOf(), .toLowerCase() und grundlegende reguläre Ausdrücke.
 * Leerzeichen flexibel behandeln: Vermeiden Sie strenge String-Vergleiche, die aufgrund zusätzlicher Leerzeichen am Ende oder Zeilenumbrüchen fehlschlagen.
 * Kompatibilität bewahren: Führen Sie keine ES6-Methoden (wie .includes()) ein, es sei denn, sie werden nativ innerhalb der Datei als Polyfill bereitgestellt.
🌍 Sprachübersetzungsfortschritt
> Haftungsausschluss: Sprachübersetzungen in diesem Projekt werden mithilfe von Künstlicher Intelligenz (KI) erstellt. Während KI-Modelle eine hochwertige Verarbeitung ermöglichen, können geringfügige kontextbezogene Fehler vorhanden sein.
> 
Wir streben an, wichtige Weltsprachen zu unterstützen, die von über 1 Million Menschen gesprochen werden.
Kernsprachen
 * [x] Englisch (English)
 * [x] Deutsch (Deutsch)
 * [x] Chinesisch - Mandarin (普通话)
 * [x] Hindi (हिन्दी)
 * [x] Spanisch (Español)
 * [x] Arabisch - Modern Standard (العربية الفصحى)
 * [o] Französisch (Français)
 * [o] Bengali (বাংলা)
 * [o] Portugiesisch (Português)
 * [o] Russisch (Русский)
 * [o] Urdu (اردو)
 * [o] Indonesisch (Bahasa Indonesia)
 * [o] Suaheli (Kiswahili)
 * [o] Hausa (Harshen Hausa)
 * [o] Yoruba (Èdè Yorùbá)
 * [o] Zulu (isiZulu)
 * [o] Twi (Akan)
 * [o] Japanisch (日本語)
 * [o] Pandschabi (ਪੰਜਾਬੀ / پنجابی)
 * [o] Vietnamesisch (Tiếng Việt)
 * [o] Türkisch (Türkçe)
 * [o] Koreanisch (한국어)
(Legende: [x] Abgeschlossen | [o] In Bearbeitung | [ ] Geplant)
📐 Technische Spezifikationen
 * Dateiformat: Einzelne .html-Datei (~50 KB)
 * Standards: HTML5, CSS3, ES3/ES5 JavaScript
 * Abhängigkeiten: 0 externe Bibliotheken, 0 Schriftarten, 0 Frameworks
 * Netzwerkanforderung: 0 KB/s (100 % offline funktionsfähig)
 * Speicheranforderungen: Keine
 * Minimale Browser-Anforderungen: Internet Explorer 6+, Firefox 1.0+, Safari 1.0+, Chrome 1.0+ oder ein beliebiger Legacy-WebKit/Gecko-Browser.
📄 Lizenz & Autor
Autor
M-Tarantino (@M-Tarantino)
Lizenz
Dieses Projekt ist unter der MIT-Lizenz lizenziert. Es steht Ihnen frei, diese Software für nicht-kommerzielle und kommerzielle Zwecke zu verwenden, zu modifizieren, zu verteilen, zu hosten und damit zu unterrichten, vorausgesetzt, die ursprüngliche Namensnennung wird beibehalten.
Tower of HTML — Zugänglich. Langlebig. Universell.

