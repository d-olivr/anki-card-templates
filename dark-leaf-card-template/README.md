<h1> 🍃 Anki Dark Leaf + Toggle Template  </h1>

[![][html-img]][html-url] [![][css-img]][css-url]

[html-img]: https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white
[html-url]: ./front.html
[css-img]: https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white
[css-url]: ./style.css

A custom Anki card template with a clean dark and green palette, a collapsible **e.g.** section for examples, and custom theme for inline and code blocks.

---

## 🟢 Preview
<img width="1200" alt="preview" src="https://github.com/user-attachments/assets/19fae4f2-de08-45f9-9e8a-ed7957ca6790" />

<!--- to be added later! --->

> Screenshots taken on Anki Desktop 25.09.2 using the [Onigiri](https://ankiweb.net/shared/info/1210908941) addon.
 
<br>

---

<br>

## ✅ Features

### Three-section layout

| Section | Field name | Description |
|---------|------------|-------------|
| **Front** | `Front` | The question / prompt shown before flipping |
| **Back** | `Back` | The answer revealed after flipping |
| **e.g.** | `Example` | Extra example or context, hidden by default behind a toggle |

### 🟢 Collapsible *e.g.* section

The **e.g.** block sits below the answer and starts collapsed. Clicking the label expands it, being useful for examples, mnemonics, usage sentences, or anything you don't want cluttering the answer at a first glance.


### 🟢 Code Rendering

### Inline code

Wrap any snippet in backticks (or `<code>` tags) and it gets a subtle dark pill with a green color, distinct from regular text but not distracting. It renders as a rounded badge with slightly dark background and green text.

### Code Block

Wrap multi-line snippets in `<pre><code>` for a VS Code styled block: dark `#1e1e1e` background, left-aligned and horizontally scrollable.

You can use `<b>` inside `<pre>` or `<code>` to highlight a specific token in the accent color.

<br>

---

<br>

## 📗 Installation


1. Make sure to have [Coolvetica](https://www.dafont.com/coolvetica.font) downloaded.
2. Rename the font file to `_Coolvetica-Regular.ttf` and paste it in your [Anki media folder](https://docs.ankiweb.net/files.html#media):
   - **Windows:** `%APPDATA%\Anki2\<profile>\collection.media\`
   - **macOS:** `~/Library/Application Support/Anki2/<profile>/collection.media/`
   - **Linux:** `~/.local/share/Anki2/<profile>/collection.media/`
3. In Anki, click `Add`, then `Manage` next to Type, then `Add` and select `Basic` to create a new note type.
4. Select the new note type and click `Cards...`
5. Rename the card to `toggle`, then paste `front.html` into "Front Template", `back.html` into "Back Template", and `main.css` into "Styling", then click `Save`.
6. Back in `Manage Note Types`, select the note type and click `Fields...` to rename/add fields so they match `Front`, `Back`, and `Example` as described above.
7. Add your new cards by selecting the `toggle` card type.
8. Done :)

> NOTE: The font filename must start with `_` so Anki doesn't strip it during sync or delete it when [checking media](https://docs.ankiweb.net/media.html#checking-media).

