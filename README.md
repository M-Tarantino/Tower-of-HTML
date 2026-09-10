# Tower of HTML

**Tower of HTML** is a minimalist, offline-first educational platform for learning HTML fundamentals. The entire project is housed within a single, self-contained file (`index.html`) with zero external dependencies, frameworks, or server requirements.

## Features

* **100% Offline-First**: Runs locally in any web browser without requiring an internet connection.
* **Maximum Compatibility**: Built with legacy-safe JavaScript (ES3/ES5 standard) and basic HTML/CSS. Fully functional across legacy hardware, old browser engines, and modern mobile devices.
* **Zero Dependencies**: All core mechanics, styling, and instructional content are embedded into a single file.
* **Level-Code System**: Progress is tracked using short password hashes (e.g., `L1-ROOT`), allowing users to jump directly to unlocked floors without needing local storage or cookies.

## Getting Started

1. Download the `index.html` file to your device.
2. Open the file by double-clicking it or opening it in any browser.
3. Complete the HTML exercise in the input field and click **CHECK CODE**.
4. Save the displayed Level Code to resume progress on another device or session.

## Architecture & Expansion

The application structure separates the core engine logic from the clear-text content blocks:

1. **Logic Engine**: Located within the `<script>` block, handling DOM updates, navigation, and validation checks.
2. **Content Data**: Stored as a simple array at the top of the script block for easy editing and extension.

## Learning Path (51 Floors)

### Phase 1: Foundation (Floors 0-8)
- Floor 0: Overview & Instructions
- Floors 1-5: Basic tags (`<html>`, `<head>`, `<title>`, `<body>`, `<p>`)
- Floors 6-8: Closing tags (`</p>`, `</body>`, `</html>`)

### Phase 2: Content & Text (Floors 9-18)
- Floors 9-10: Headings (`<h1>`, `<h2>`)
- Floor 11: Close heading tag (`</h1>`)
- Floors 12-13: Bold text (`<b>`, `</b>`)
- Floors 14-15: Italic text (`<i>`, `</i>`)
- Floors 16-17: Strong emphasis (`<strong>`, `</strong>`)
- Floor 18: Emphasis tag (`<em>`)

### Phase 3: Links & Media (Floors 19-28)
- Floors 19-21: Links (`<a>`, `href` attribute, `</a>`)
- Floors 22-24: Images (`<img>`, `src`, `alt`)
- Floor 25: Line break (`<br>`)
- Floor 26: Horizontal rule (`<hr>`)
- Floors 27-28: Buttons (`<button>`, `</button>`)

### Phase 4: Organization (Floors 29-38)
- Floors 29-30: Divisions (`<div>`, `</div>`)
- Floors 31-32: Span elements (`<span>`, `</span>`)
- Floors 33-35: Unordered lists (`<ul>`, `<li>`, closing tags)
- Floors 36-38: Ordered lists (`<ol>`, closing tags)

### Phase 5: Intermediate & Advanced (Floors 39-48)
- Floors 39-40: Forms (`<form>`, `</form>`)
- Floor 41: Input fields (`<input>`)
- Floors 42-45: Tables (`<table>`, `<tr>`, `<td>`, `</table>`)
- Floor 46: HTML comments (`<!-- -->`)
- Floor 47: Class attribute
- Floor 48: ID attribute

### Phase 6: Final Challenge (Floors 49-51)
- Floor 49: DOCTYPE declaration
- Floor 50: Meta charset
- Floor 51: **FINAL BOSS** - Build a complete webpage

## Level Codes

Users can jump directly to any unlocked floor using the **JUMP TO FLOOR** input:

```
START    → Floor 0 (Instructions)
L1-ROOT  → Floor 1 (Root HTML element)
L2-HEAD  → Floor 2 (Head section)
L3-TITLE → Floor 3 (Page title)
... and so on
L51-COMPLETE → Floor 51 (Final boss)
```

## Customization & Expansion

To add new floors, simply add objects to the `levels` array in the HTML file:

```javascript
{
    id: "L99-EXAMPLE",
    title: "Floor 99: Example Tag",
    info: "Explanation of the concept...",
    hint: "Hint for the user...",
    desc: "Description of the task...",
    check: function(input) {
        return input.toLowerCase().indexOf("<example>") !== -1;
    }
}
```

### Validation Functions

- **Simple string match**: `return input.toLowerCase().indexOf("<tag>") !== -1;`
- **Multiple conditions**: `return lower.indexOf("<tag") !== -1 && lower.indexOf("attribute") !== -1;`
- **Complex patterns**: Build custom logic for validation

## Technical Details

- **Language**: Pure HTML5 + CSS + ES3/ES5 JavaScript
- **File Size**: ~50KB (single .html file)
- **Browser Support**: All modern browsers + legacy engines (IE6+)
- **Dependencies**: None
- **Storage**: No local storage required (uses level codes)

## License

MIT License - You are free to use, modify, and distribute this project.

See `github.com/M-Tarantino` for more information.

## Author

**M-Tarantino** (@M-Tarantino)

---

**Enjoy climbing the Tower of HTML!** 🏆
