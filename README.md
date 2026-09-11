# Tower of HTML

> **Make HTML education universally accessible — regardless of hardware, internet connectivity, or device age.**

**Tower of HTML** is a minimalist, offline-first educational platform designed to teach HTML fundamentals from scratch. The entire application is housed within a single, self-contained `.html` file with zero external dependencies, frameworks, build steps, or server requirements.

## 🌐 Live Version

You can try out the project directly in your browser:
👉 [Live Version on GitHub Pages](https://m-tarantino.github.io/Tower-of-HTML/)

---

## 📋 Table of Contents

- [Design Philosophy & Core Mission](#design-philosophy--core-mission)
- [Key Features](#key-features)
- [Universal Accessibility & Hardware Compatibility](#universal-accessibility--hardware-compatibility)
- [Getting Started](#getting-started)
- [Architecture & Mechanics](#architecture--mechanics)
- [Learning Path (51 Floors)](#learning-path-51-floors)
- [Level-Code Progression System](#level-code-progression-system)
- [Customization & Extension Guidelines](#customization--extension-guidelines)
- [Translations](#translations)
- [Language Translation Progress](#language-translation-progress)
- [Technical Specifications](#technical-specifications)
- [License & Author](#license--author)

---

## 🎯 Design Philosophy & Core Mission

### The Problem We Solve
Most modern web development learning platforms introduce significant barriers:
1. **Dependency on Internet Connectivity**: Online IDEs and LMS platforms fail in low-bandwidth or offline environments.
2. **Modern Hardware Requirements**: Modern tools require modern operating systems, high RAM, and heavy browser engines, locking out users on older hardware.
3. **Complexity Overhead**: Beginners are often overwhelmed by build tools, frameworks, and package managers before writing a single line of HTML.
4. **Vendor Lock-in**: User progress depends on third-party platform availability and mandatory account creation.

### Our Solution
Tower of HTML operates on four core commitments:
* **Accessibility Before Features**: Prioritizes raw compatibility and clear readability over UI frameworks.
* **Education Over Entertainment**: Structured, floor-by-floor progression where mastery is earned through strict, fair validation.
* **Ownership Over Platforms**: Users can own, download, modify, and run the project indefinitely without asking permission.
* **Clarity Over Cleverness**: Written in clear, readable code without obfuscation or transpilation so learners can inspect and learn directly from the source code itself.

---

## ✨ Key Features

* **100% Offline-First**: Runs locally in any web browser without requiring network access.
* **Single-File Architecture**: Everything (CSS, JS, Content) resides inside one portable `index.html` file (~50KB).
* **Legacy Engine Support**: Built using legacy-safe JavaScript (ES3/ES5 standard) to ensure functional execution on vintage hardware.
* **Zero Dependencies**: Free of external libraries, package managers, fonts, or CDN links.
* **Level-Code System**: Simple password hash mechanism allows users to resume progress across any browser or device without local storage.
* **Terminal Themes**: Customizable visual modes (Matrix, Amber, DOS Blue, Light, Cyber) accessible directly in the interface.

---

## 🌐 Universal Accessibility & Hardware Compatibility

Because Tower of HTML is written in legacy-safe JavaScript without modern web dependencies, it runs reliably across a wide spectrum of devices and operating systems:

| Device / Platform | Operational Status | Notes |
| :--- | :---: | :--- |
| **1995 Pentium PC** | ✅ Supported | Windows 95/98, Internet Explorer 6+ |
| **Chromebooks** | ✅ Supported | All Chrome browser versions |
| **Legacy Mobile (iPhone 4S / Android 4.0)** | ✅ Supported | Native mobile browsers (Safari 5+, Android WebKit) |
| **Modern Laptops & Desktops** | ✅ Supported | Chrome, Firefox, Safari, Edge, Opera |
| **Raspberry Pi** | ✅ Supported | Lightweight browser engines |
| **Low-Resource Educational Labs** | ✅ Supported | No administrative privileges or installation required |

This design allows educators in low-resource environments to download the project once and distribute it to students via USB or local file sharing.

---

## 🚀 Getting Started

1. Download or save the `index.html` file to your device.
2. Double-click `index.html` (or open it with any web browser).
3. Read the prompt for the current floor, type your HTML snippet into the input field, and click **CHECK CODE**.
4. Upon completing a floor, write down or copy the generated **Level Code** to resume your progress in future sessions or on different devices.

---

## 🏗️ Architecture & Mechanics

The single `index.html` file strictly separates the execution logic from instructional content while maintaining a dependency-free environment:


index.html
├── <head>
│   └── <style> : Terminal styling, responsive layouts, visual themes
└── <body>
├── UI Container : Game screen, input terminal, output view
└── <script>
├── levels[] Array : Plain-text instructional data & validation rules
└── Engine Logic   : DOM updates, level-code verification, progression state

### Design Commitments
- **Inline CSS**: Embedded within a single `<style>` block.
- **Inline JavaScript**: Embedded within a single `<script>` block.
- **ES3/ES5 Standard**: Uses standard loop constructs and ES3/ES5 syntax (`var`, `for` loops) instead of modern ES6+ features requiring transpilation.

---

## 📚 Learning Path (51 Floors)

The curriculum consists of 51 structured floors spanning six distinct phases:


Skill Progression:
Beginner (Floors 0–8)    → Tags, closing tags, and page structure
Intermediate (Floors 9–28)  → Formatting, links, buttons, and media
Advanced (Floors 29–48)  → Divisions, lists, forms, tables, and attributes
Expert (Floors 49–51)    → Document declarations, character sets, and final integration

### Phase 1: Foundation (Floors 0–8)
| Floor | Code | Title | Task / Concept |
| :---: | :--- | :--- | :--- |
| **0** | `START` | Overview & Instructions | Game introduction & controls |
| **1** | `L1-ROOT` | The Root Element | `<html>` tag creation |
| **2** | `L2-HEAD` | The Head Section | `<head>` metadata container |
| **3** | `L3-TITLE` | Page Title | `<title>` tab naming |
| **4** | `L4-BODY` | The Body Section | `<body>` content area |
| **5** | `L5-PARA` | Paragraphs | `<p>` text structure |
| **6** | `L6-CLOSE-P` | Closing Paragraph Tag | `</p>` tag closure |
| **7** | `L7-CLOSE-BODY` | Closing Body Tag | `</body>` tag closure |
| **8** | `L8-CLOSE-HTML` | Closing HTML Tag | `</html>` tag closure |

### Phase 2: Content & Text (Floors 9–18)
| Floor | Code | Title | Task / Concept |
| :---: | :--- | :--- | :--- |
| **9** | `L9-H1` | Main Heading (H1) | `<h1>` heading level 1 |
| **10** | `L10-H2` | Subheading (H2) | `<h2>` heading level 2 |
| **11** | `L11-CLOSE-H1` | Close Heading Tag | `</h1>` closing tag |
| **12** | `L12-BOLD` | Bold Text | `<b>` presentation bold |
| **13** | `L13-CLOSE-BOLD` | Close Bold Tag | `</b>` tag closure |
| **14** | `L14-ITALIC` | Italic Text | `<i>` presentation italic |
| **15** | `L15-CLOSE-ITALIC` | Close Italic Tag | `</i>` tag closure |
| **16** | `L16-STRONG` | Strong Emphasis | `<strong>` semantic emphasis |
| **17** | `L17-CLOSE-STRONG` | Close Strong Tag | `</strong>` tag closure |
| **18** | `L18-EM` | Emphasis | `<em>` semantic stress |

### Phase 3: Links & Media (Floors 19–28)
| Floor | Code | Title | Task / Concept |
| :---: | :--- | :--- | :--- |
| **19** | `L19-ANCHOR` | Link Tag | `<a>` anchor element |
| **20** | `L20-HREF` | Link Destination | `<a href="...">` attribute usage |
| **21** | `L21-CLOSE-ANCHOR` | Close Link Tag | `</a>` tag closure |
| **22** | `L22-IMG` | Image Element | `<img>` image container |
| **23** | `L23-SRC` | Image Source | `<img src="...">` attribute usage |
| **24** | `L24-ALT` | Alt Text | Accessibility attribute (`alt="..."`) |
| **25** | `L25-BR` | Line Break | `<br>` self-closing break |
| **26** | `L26-HR` | Horizontal Rule | `<hr>` divider line |
| **27** | `L27-BUTTON` | Button Element | `<button>` interactive element |
| **28** | `L28-CLOSE-BUTTON` | Close Button Tag | `</button>` tag closure |

### Phase 4: Organization (Floors 29–38)
| Floor | Code | Title | Task / Concept |
| :---: | :--- | :--- | :--- |
| **29** | `L29-DIV` | Division Container | `<div>` block container |
| **30** | `L30-CLOSE-DIV` | Close DIV Tag | `</div>` tag closure |
| **31** | `L31-SPAN` | Span Element | `<span>` inline container |
| **32** | `L32-CLOSE-SPAN` | Close Span Tag | `</span>` tag closure |
| **33** | `L33-UL` | Unordered List | `<ul>` bulleted list container |
| **34** | `L34-LI` | List Item | `<li>` element |
| **35** | `L35-CLOSE-LI` | Close List Item | `</li>` tag closure |
| **36** | `L36-OL` | Ordered List | `<ol>` numbered list container |
| **37** | `L37-CLOSE-UL` | Close Unordered List | `</ul>` tag closure |
| **38** | `L38-CLOSE-OL` | Close Ordered List | `</ol>` tag closure |

### Phase 5: Intermediate & Advanced (Floors 39–48)
| Floor | Code | Title | Task / Concept |
| :---: | :--- | :--- | :--- |
| **39** | `L39-FORM` | Form Container | `<form>` input wrapper |
| **40** | `L40-CLOSE-FORM` | Close Form Tag | `</form>` tag closure |
| **41** | `L41-INPUT` | Input Field | `<input>` self-closing field |
| **42** | `L42-TABLE` | Data Table | `<table>` container |
| **43** | `L43-TR` | Table Row | `<tr>` row element |
| **44** | `L44-TD` | Table Cell | `<td>` data cell element |
| **45** | `L45-CLOSE-TABLE` | Close Table Tag | `</table>` tag closure |
| **46** | `L46-COMMENT` | HTML Comments | `<!-- comment -->` syntax |
| **47** | `L47-CLASS` | Class Attribute | `class="..."` styling target |
| **48** | `L48-ID` | ID Attribute | `id="..."` unique target |

### Phase 6: Final Challenge (Floors 49–51)
| Floor | Code | Title | Task / Concept |
| :---: | :--- | :--- | :--- |
| **49** | `L49-DOCTYPE` | Document Type | `<!DOCTYPE html>` declaration |
| **50** | `L50-META-CHARSET` | Character Encoding | `<meta charset="UTF-8">` metadata |
| **51** | `L51-COMPLETE` | **FINAL BOSS** | Build a complete, valid webpage |

---

## 🔑 Level-Code Progression System

Rather than relying on browser storage APIs (`localStorage`, `indexedDB`, or cookies), progress is saved via short, human-readable **Level Codes**. 

### How It Works
1. Upon completing a floor, the application displays a unique code (e.g., `L5-PARA`).
2. Users can copy, save, or write down the code.
3. In subsequent sessions, entering the code into the **JUMP TO FLOOR** field instantly loads that floor's state.

### Benefits
- **Cross-Browser & Cross-Device**: Move seamlessly between an old mobile phone and a desktop computer.
- **Zero Privacy Footprint**: Operates without tracking users, storing cookies, or making web requests.
- **No API Dependencies**: Functions on browsers created before local storage specifications existed.

---

## 🛠️ Customization & Extension Guidelines

Because the entire application logic is stored in a clean JavaScript array, adding or modifying floors requires editing the `levels` array within `index.html`.

### Adding a New Floor

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
```
Validation Design Guidelines
When adding validation rules, maintain the project's universal compatibility rules:
 * Use Standard String Operations: Rely on methods like .indexOf(), .toLowerCase(), and basic regular expressions.
 * Handle Whitespace Flexibly: Avoid strict string comparisons that fail due to extra trailing spaces or line breaks.
 * Preserve Compatibility: Do not introduce ES6 methods (such as .includes()) unless polyfilled natively within the file.
📂 Translations
All available language-specific subfolders can be found within the Translation directory. Each folder contains:
 * A dedicated README written entirely in the native language.
 * A complete Complete Guide written entirely in the native language.
🌍 Language Translation Progress
> Disclaimer: Language translations in this project are generated using Artificial Intelligence (AI). While AI models provide high-quality processing, minor contextual errors may exist.
> 
We aim to support major world languages spoken by over 1 million people.
Core Languages
 * [x] English
 * [x] German (Deutsch)
 * [x] Chinese - Mandarin (普通话)
 * [x] Hindi (हिन्दी)
 * [x] Spanish (Español)
 * [x] Arabic - Modern Standard (العربية الفصحى)
 * [o] French (Français)
 * [o] Bengali (বাংলা)
 * [o] Portuguese (Português)
 * [o] Russian (Русский)
 * [o] Urdu (اردو)
 * [o] Indonesian (Bahasa Indonesia)
 * [o] Swahili (Kiswahili)
 * [o] Hausa (Harshen Hausa)
 * [o] Yoruba (Èdè Yorùbá)
 * [o] Zulu (isiZulu)
 * [o] Twi (Akan)
 * [o] Japanese (日本語)
 * [o] Punjabi (ਪੰਜਾਬੀ / پنجابی)
 * [o] Vietnamese (Tiếng Việt)
 * [o] Turkish (Türkçe)
 * [o] Korean (한국어)
(Legend: [x] Completed | [o] In Progress | [ ] Planned)
📐 Technical Specifications
 * File Format: Single .html file (~50KB)
 * Standards: HTML5, CSS3, ES3/ES5 JavaScript
 * Dependencies: 0 external libraries, 0 fonts, 0 frameworks
 * Network Requirement: 0 KB/s (100% offline functional)
 * Storage Requirements: None
 * Minimum Browser Requirements: Internet Explorer 6+, Firefox 1.0+, Safari 1.0+, Chrome 1.0+, or any legacy WebKit/Gecko browser.
📄 License & Author
Author
M-Tarantino (@M-Tarantino)
License
This project is licensed under the MIT License. You are free to use, modify, distribute, host, and teach with this software for both non-commercial and commercial purposes, provided original attribution is retained.
Tower of HTML — Accessible. Durable. Universal.

