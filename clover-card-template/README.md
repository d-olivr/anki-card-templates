<div align="center">

# 🍀 Anki Clover — Card Template

<br>

<img src="https://img.shields.io/badge/HTML5-5e9e80?style=for-the-badge&logo=html5&logoColor=2f4f40" />
<img src="https://img.shields.io/badge/CSS3-5e9e80?style=for-the-badge&logo=css3&logoColor=2f4f40" />

</div>

<br>

A dark, green-toned Anki card template for general study use: a simple **front/back** layout with an optional example tucked behind a hint. It inherits the look of [Dark Leaf](https://github.com/d-olivr/anki-card-templates/blob/main/dark-leaf-card-template), but with a refreshed layout. Featuring a 'session' topbar plus decorated bubbles.

---

## 🟢 Preview
<div align="center">
   <img height="670" alt="screenshot 2" src="https://github.com/user-attachments/assets/7141271a-1abc-451c-845d-bf1443e152d9" /></td>
</div>


> Screenshots taken on Anki Desktop ⁨25.09.2 using [this](https://ankiweb.net/shared/info/1210908941) addon.

<br>

---

<br>

## ✅ Features

### 🟢 Session topbar

A pill at the top of the card showing `study session`, with the note's tags displayed right alongside it whenever the note has any, so it can give context without cluttering.

### 🟢 Decorated bubbles

Front and back share the same question bubble, with the `🍀` and `☘️` emojis placed in the corners as decoration. You can change the emojis by adjusting the front and back html code. You can even use kaomojis instead, which look super cute too (｡•̀ᴗ-)✧

### 🟢 Collapsible example

The `eg` field stays hidden by default behind Anki's native hint (`{{hint:eg}}`), rendered with MathJax support (`{{mathjax:hint:eg}}`). This section comes in handy for extra context, formulas, or notes without cluttering the answer itself. Learn more about the [hint feature](https://docs.ankiweb.net/templates/fields.html#hint-fields)
### 🟢 Code rendering

Keeps the Dark Leaf styling: inline `code` becomes a dark pill with green text, and `<pre><code>` blocks turn into a block styled like VSCode. Using `<b>` inside `code`/`pre` highlights a specific token in the accent color.

### 🟢 Math support

CSS is already set up for MathJax (`mjx-container`) and KaTeX, with both inline and block (`display="true"`) formulas respecting the card's width and left alignment.

### 🟢 Cloze support

Cloze deletions are styled through the `.cloze` class, rendered in the accent color with extra bold weight so the hidden part stands out clearly from the rest of the card text.

### 🟢 Responsive layout

Dedicated `.mobile` rules shrink paddings, font sizes, and the background grid to better fit the Anki mobile screen, with no extra configuration needed.

<br>

---

<br>

## 🗂️ Field structure

| Field | Used in template | Description |
|---|---|---|
| `front` | `{{edit:front}}` (Front and Back) | Question / prompt, shown on both sides of the card |
| `back` | `{{edit:back}}` (Back) | Answer, shown in the answer bubble after flipping |
| `eg` | `{{mathjax:hint:eg}}` (Back) | Optional example or extra note, hidden behind a hint |
| `Tags` | `{{Tags}}` (Front and Back) | Displayed next to `study session` in the topbar whenever the note has tags |

<br>

---

<br>

## 📗 Installation

1. Make sure to download the [Coolvetica Font](https://www.dafont.com/coolvetica.font).
2. Rename the font file to `_Coolvetica Rg.otf` (the exact name used in `@font-face`) and drop it into your [Anki media folder](https://docs.ankiweb.net/files.html#media):
   - **Windows:** `%APPDATA%\Anki2\<profile>\collection.media\`
   - **macOS:** `~/Library/Application Support/Anki2/<profile>/collection.media/`
   - **Linux:** `~/.local/share/Anki2/<profile>/collection.media/`
3. In Anki, click `Add`, then `Manage` next to Type, then `Add` and select `Basic` to create a new note type.
4. Select the new note type and click `Cards...`
5. Paste `front.html` into "Front Template", `back.html` into "Back Template", and `style.css` into "Styling", then click `Save`.
6. Back in `Manage Note Types`, select the note type and click `Fields...` to rename/add fields so they match `front`, `back` and `eg`, as described in the table above.
7. When creating new cards, select this template's note type and fill in the fields as described above.
8. Done :)

> **NOTE:** The font filename must start with `_` so Anki doesn't strip it during sync or delete it when [checking media](https://docs.ankiweb.net/media.html#checking-media).
