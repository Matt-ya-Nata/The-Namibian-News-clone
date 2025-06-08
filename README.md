#  The Namibian (Clone) – Holy Grail Layout with CSS Grid

This is a **responsive, modern HTML and CSS clone** of a typical news article layout, inspired by [The Namibian](https://www.namibian.com.na/) website. It is **not affiliated with the actual site**. This project demonstrates the **Holy Grail Layout** using **CSS Grid**, a powerful layout system in modern web design.

---

## 📸 Preview

![image](https://github.com/user-attachments/assets/2525a502-0f3d-47c7-8e65-21e274c04432)

*President Netumbo Nandi-Ndaitwah’s historic moment featured in a responsive layout.*

---

## 🧩 Key Features

- **Holy Grail Layout**: Header, footer, left/right fixed ads, and centered main content.
- **Responsive Design**: Collapsible ads on smaller screens using media queries.
- **Clean Typography**: Uses Google Fonts (`Poppins`) for professional styling.
- **Semantic HTML5**: `<header>`, `<article>`, `<footer>` and proper tag usage.
- **CSS Grid Focus**: Layout is built almost entirely with `grid-template-columns` and `grid-column`.

---

## 🧰 Project Stack

| Technology | Description                                  |
|------------|----------------------------------------------|
| HTML5      | Semantic markup for structuring the content  |
| CSS3       | Styling the layout and responsive behavior   |
| CSS Grid   | Core layout technique used for Holy Grail    |
| Media Queries | Responsive design implementation         |
| Google Fonts (Poppins) | Enhanced typography              |

---

## 🎯 Layout Overview

```text
+------------------------------+
|           HEADER            |
+------+----------------+-----+
| Left |     ARTICLE     |Right|
|  Ad  |   (Main Story)  | Ad  |
+------+----------------+-----+
|           FOOTER            |
+------------------------------+
```
## Implemented using:
```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  column-gap: 30px;
}
```

## 📱 Responsive Design Breakpoints
The layout adapts across multiple devices using the following breakpoints:
## ✅ Default: > 1200px (Desktop)
- Left and right ads are visible
- Article is centered
- Layout is 3-column
## ✅ max-width: 1200px (Laptop)
```css
@media screen and (max-width: 1200px) {
  .leftAd,
  .rightAd {
    display: none;
  }
  article {
    grid-column: span 3;
  }
}
```
- Left and right ads are hidden
- Article spans the full grid (centered layout)

## ✅ max-width: 980px (Tablet & Small Laptops)
```css
@media screen and (max-width: 980px) {
  .leftAd article .rightAd {
    grid-column: span 3;
  }
}
```
- Reaffirm article spans the full layout
- Improves readability on tablets
## 📂 File Structure
```text
namibian-holy-grail-clone/
├── index.html           # Main HTML layout
├── styles.css           # All styles including CSS Grid
├── README.md            # Project documentation
└── Images/
    ├── Namibian_logo png.png
    ├── radio logo.png
    ├── president.png
    ├── ad1.jpg
    └── AD2.png
```



