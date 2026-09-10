# Tower of HTML

**Tower of HTML** is a minimalist, offline-first educational platform for learning HTML fundamentals. The entire project is housed within a single, self-contained file (`index.html`) with zero external dependencies, frameworks, or server requirements.

## Features

* **100% Offline-First**: Runs locally in any web browser without requiring an internet connection.
* **Maximum Compatibility**: Built with legacy-safe JavaScript (ES3/ES5 standard) and basic HTML/CSS. Fully functional across legacy hardware, old browser engines, and modern mobile devices.
* **Zero Dependencies**: All core mechanics, styling, and instructional content are embedded into a single file.
* **Level-Code System**: Progress is tracked using short password hashes (e.g., `L1-START`), allowing users to jump directly to unlocked floors without needing local storage or cookies.

## Getting Started

1. Download the `index.html` file to your device.
2. Open the file by double-clicking it or opening it in any browser.
3. Complete the HTML exercise in the input field and click **CHECK CODE**.
4. Save the displayed Level Code to resume progress on another device or session.

## Architecture & Expansion

The application structure separates the core engine logic from the clear-text content blocks:

1. **Logic Engine**: Located within the `<script>` block, handling DOM updates, navigation, and validation checks.
2. **Content Data**: Stored as a simple array at the top of the script block for easy editing and extension.

