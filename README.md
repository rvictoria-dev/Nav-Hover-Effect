# Nav Hover Effect

### ₊⊹ About

This project consists of a pill-shaped navigation bar designed with a focus on fluid micro-interactions and minimalist design. Developed exclusively using pure HTML5 and CSS3, the project served as a practical study focused on advanced transitions, CSS selector logic, and interactive behavior.

https://github.com/user-attachments/assets/c5c73085-8b90-4a94-b365-eb2a77f272d3

---

### ★ Features

- A sliding block that follows the cursor from link to link

- Smooth transitions in the block’s position, its fade-in and fade-out effects, and the text color

- The text turns white on hover to maintain contrast with the burgundy block

- Pure HTML and CSS, no JavaScript

- Links of equal width using Flexbox, centered on the page

- Modern CSS: anchor positioning and the `:has()` selector

---

### ⚙️ Tech Stack

- **HTML**
- **CSS**

---

### 🖿 Project structure

```
nav-hover-effect/
├── Styles.css
├── index.html
└── README.md
```
---

### .ᐟ.ᐟ How It Works

- Anchor: The link under the cursor dynamically receives the anchor-name property: --pill, becoming the active reference at that moment.

- Pill: The nav::before pseudo-element (highlighted in burgundy) uses position-anchor: --pill and inset: anchor(...) to align itself and stretch to exactly the size of the anchored link.

- Motion: The `transition: inset 0.4s` property creates the visual effect of the block smoothly sliding from one link to another when the anchor changes.

- Visibility: Using the `nav:has(a:hover)::before` selector, the highlight only displays maximum opacity while the mouse is over the menu, fading out smoothly when the mouse leaves.

- Layers: Using `isolation: isolate` on the container and `z-index: -1` on the pseudo-element ensures that the burgundy block appears behind the text without disappearing beneath the main background.
