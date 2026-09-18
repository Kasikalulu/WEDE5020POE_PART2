# WEDE5020POE_PART2
# MABLFA Website — WEDE5020 Portfolio of Evidence

**Student Name:** Christophe Cishugi  
**Student Number:** ST10538383  
**Module:** WEDE5020 — Web Development (Introduction)  
**Project:** Mabopane Local Football Association (MABLFA) Website

---

## 1. Introduction

This document is the README for the Mabopane Local Football Association website. It tracks all changes made between **Part 1** (HTML foundation) and **Part 2** (CSS styling and responsive design). Each change is listed with a short explanation and referenced to the module material (The IIE, 2026).

---

## 2. Changes From Part 1 to Part 2

### 2.1 External Stylesheet Created

In Part 1, all pages were plain HTML with no styling and In Part 2 I created an external stylesheet called `styles.css` and linked to every HTML page using the `<link>` tag inside the `<head>` section (The IIE, 2026, Week 5, Slide 6).

**Change made:**
- Created `styles.css` in a `css/` folder
- Linked it to all 5 pages using `<link href="css/styles.css" rel="stylesheet" type="text/css"/>`

**Reference:** The IIE (2026) states that the `<link>` tag connects a page to an external CSS file and should appear inside the `<head>` tag (The IIE, 2026, Week 5, Slide 6).

---

### 2.2 CSS Reset Added

In Part 1, browsers applied their own default margins and padding, causing spacing inconsistencies. In Part 2, a universal selector (`*`) was added to reset these defaults (The IIE, 2026, Week 6, Slide 3).

**Change made:**

    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

**Why it matters:** This makes every browser start from the same baseline, ensuring consistent styling (The IIE, 2026, WEDE5020POE.pdf, Part 2, Section 2.2).

---

### 2.3 Colour Scheme Introduced

In Part 1, the website used browser default colours (black text on white). In Part 2, a dark theme was applied using a near-black background, white text, and antique gold as the accent colour.

| **Element** | **Colour** | **Hex Code** |
| :--- | :--- | :--- |
| Body background | Near-black | `#0d0d0d` |
| Wrapper | Dark grey | `#111111` |
| Header/Footer | Deep black | `#0a0a0a` |
| Gold accent | Antique gold | `#c9a961` |
| Main text | White | `#ffffff` |
| Muted text | Light grey | `#cccccc` |

**Reference:** Colour was applied using `color` and `background-color` (The IIE, 2026, Week 6, Slide 27).

---

### 2.4 Typography Styled

In Part 1, all text used browser defaults. In Part 2, three font families were introduced using `font-family` (The IIE, 2026, Week 6, Slide 27):

1. **Arial, Helvetica, sans-serif** — for body text
2. **Georgia, Times New Roman, serif** — for headings
3. **Cursive** — for the "Mabopane" script name and decorative headings

Additional typography properties added:
- `font-size` — for hierarchy
- `font-weight` — bold for emphasis
- `line-height` — for readability
- `letter-spacing` — for headings and labels
- `text-align` — for centring content

**Reference:** Typography controls the visual hierarchy of a webpage (The IIE, 2026, Week 6, Slide 27).

---

### 2.5 Header Redesigned and Made Consistent

In Part 1, the header was plain text with no logo or structure. In Part 2, the header was rebuilt with a consistent layout across all 5 pages.

**Changes made:**
1. Added a centered logo using `display: block` and `margin: 0 auto` (The IIE, 2026, Week 6, Slides 16-17)
2. Added a cursive script site name "Mabopane"
3. Added a decorative "L F A" divider with gold lines using `<span>` (The IIE, 2026, Week 5, Slide 13)
4. Added a sign-in placeholder link positioned absolutely to the top right (The IIE, 2026, Week 6, Slide 19)

**Reference:** Positioning elements with `position: relative` on the parent and `position: absolute` on the child is covered in Week 6, Slide 19 (The IIE, 2026).

---

### 2.6 Navigation Made Horizontal

In Part 1, navigation links stacked vertically with bullet points. In Part 2, the navigation is horizontal and styled.

**Changes made:**
1. Removed bullet points with `list-style: none` (The IIE, 2026, Week 6, Slide 16)
2. Made items horizontal with `display: inline-block` (The IIE, 2026, Week 6, Slide 16)
3. Added hover effects that change colour and add a gold underline
4. Added `class="currentPage"` to highlight the current page in gold

**Reference:** Horizontal navigation is achieved by changing `<li>` items from block to inline-block (The IIE, 2026, Week 6, Slide 16).

---

### 2.7 Homepage Feature Cards Added

In Part 1, the homepage had no cards. In Part 2, four cards were added to the homepage: Fixtures & Results, League Table, Clubs & Players, and Gallery.

**Changes made:**
1. Applied `float: left` to place 4 cards in one row (The IIE, 2026, Week 6, Slide 20)
2. Each card is `width: 23%` with `margin-right: 2%` (The IIE, 2026, Week 7, Slide 14)
3. Added `background-image` to each card via inline style (The IIE, 2026, Week 5, Slide 10; Week 6, Slide 26)
4. Added a semi-transparent overlay with `rgba(0, 0, 0, 0.6)` so text remains readable (The IIE, 2026, Week 6, Slide 26)

**Reference:** Float layout is explained in Week 6, Slide 20, and using percentages for widths is explained in Week 7, Slide 14 (The IIE, 2026).

---

### 2.8 History Section and About Strip Added

In Part 1, there were no such sections. In Part 2, two new sections were added to the homepage.

**Changes made:**
1. **History section** — uses a `linear-gradient` overlay on top of a background image so text stays readable (The IIE, 2026, Week 6, Slide 26)
2. **About strip** — same technique, with a clickable "ABOUT US →" link styled as a pill using `border-radius` (The IIE, 2026, Week 6, Slide 25)

**Reference:** Applying a `linear-gradient` as a background is covered in Week 6, Slide 26 (The IIE, 2026).

---

### 2.9 Gallery Page Styled as a Grid

In Part 1, the gallery was just 3 unstyled images stacked. In Part 2, it was rebuilt as a 3-column grid with gold-outlined images and captions.

**Changes made:**
1. Used `float: left` with `width: 31%` so 3 images fit per row (The IIE, 2026, Week 6, Slide 20; Week 7, Slide 14)
2. Added `border: 2px solid #c9a961` around each image (The IIE, 2026, Week 6, Slide 24)
3. Added `border-radius` for rounded corners (The IIE, 2026, Week 6, Slide 25)
4. Added a caption below each image using `<p class="gallery-caption">`
5. Added `box-shadow` for depth (The IIE, 2026, WEDE5020POE.pdf, Part 2, Section 2.5)

**Reference:** Float-based grids are covered in Week 6, Slide 20, and percentage widths in Week 7, Slide 14 (The IIE, 2026).

---

### 2.10 League Table and Fixtures Page Split Into Two Columns

In Part 1, the league table page was just a heading and a link. In Part 2, it was rebuilt with two side-by-side columns.

**Changes made:**
1. Left column (48% width) — displays upcoming fixtures
2. Right column (48% width) — displays the league table
3. Both columns use `float: left` with a `4%` gap between them (The IIE, 2026, Week 6, Slide 20; Week 7, Slide 14)
4. The parent container uses `overflow: hidden` to contain the floated columns (The IIE, 2026, Week 6, Slide 22)
5. A `.clearFix` div is used to close the float (The IIE, 2026, Week 6, Slide 21)

**Reference:** Float layout and clearing are covered in Week 6, Slides 20-21 (The IIE, 2026).

---

### 2.11 Link Pseudo-Classes Added

In Part 1, links were unstyled. In Part 2, all five link states were styled (The IIE, 2026, Week 6, Slides 28-29):

| **Pseudo-Class** | **Purpose** |
| :--- | :--- |
| `a:link` | Default link colour (gold) |
| `a:visited` | Darker gold once visited |
| `a:hover` | White when hovered |
| `a:active` | Gold when clicked |
| `a:focus` | Dashed gold outline for keyboard users |

**Reference:** The order of link pseudo-classes matters — link, visited, hover, active, focus — otherwise they do not work (The IIE, 2026, Week 6, Slide 28).

---

### 2.12 Responsive Design Added (Tablet & Mobile)

In Part 1, the pages were not responsive. In Part 2, two media queries were added using the mobile-first approach (The IIE, 2026, Week 7, Slides 12-13).

**Tablet breakpoint — `@media only screen and (max-width: 960px)`:**
- Cards reduce from 4 per row to 2 per row
- Gallery reduces from 3 per row to 2 per row
- Font sizes reduce
- Sign-in link drops below navigation

**Mobile breakpoint — `@media only screen and (max-width: 480px)`:**
- All layouts stack vertically (single column)
- Navigation stacks vertically with dividers
- Cards become full-width
- Gallery items become full-width
- Font sizes reduce further for readability

**Reference:** Media queries test for browser width before applying new CSS rules (The IIE, 2026, Week 7, Slide 12). The mobile-first concept is covered in Week 7, Slide 19.

---

### 2.13 Responsive Images Applied

In Part 1, images had no responsiveness. In Part 2, all images use `max-width: 100%` and `height: auto` so they scale with the browser (The IIE, 2026, Week 7, Slide 8).

**Change made:**

    img {
        max-width: 100%;
        height: auto;
    }

**Reference:** Responsive images are achieved using `max-width: 100%` so images never overflow their container (The IIE, 2026, Week 7, Slide 8).

---

### 2.14 Code Comments Added

In Part 1, code had no comments. In Part 2, every CSS rule and every HTML section has an explanatory comment referencing the module slides.

**Reference:** WEDE5020POE.pdf rubric awards marks for "comments that fully explain the code that is developed or written" (The IIE, 2026, WEDE5020POE.pdf, Part 1 Rubric, Section 5.6).

---

### 2.15 Embedded and Inline CSS Retained

In Part 1, only plain HTML existed. In Part 2, the three CSS locations are used:

1. **External CSS** — `css/styles.css` for global styles (The IIE, 2026, Week 5, Slide 6)
2. **Embedded CSS** — `<style>` block in each page's `<head>` for page-specific styles (The IIE, 2026, Week 5, Slide 8)
3. **Inline CSS** — `style="..."` attributes on specific elements (The IIE, 2026, Week 5, Slide 10)

**Reference:** The three locations where CSS can live are explained in Week 5, Slides 6-11 (The IIE, 2026).

---

## 3. Summary of Changes

| **#** | **Change** | **Slides Reference** |
| :--- | :--- | :--- |
| 1 | External stylesheet created and linked | Week 5, Slide 6 |
| 2 | CSS reset added | Week 6, Slide 3 |
| 3 | Dark theme colour scheme applied | Week 6, Slide 26 |
| 4 | Typography system applied | Week 6, Slide 27 |
| 5 | Header redesigned with logo, script, and divider | Week 5, Slide 13; Week 6, Slides 16-19 |
| 6 | Navigation made horizontal with hover effects | Week 6, Slide 16 |
| 7 | Homepage feature cards added (4 in a row) | Week 6, Slide 20; Week 7, Slide 14 |
| 8 | History section and About strip added | Week 6, Slide 26 |
| 9 | Gallery grid built with gold outlines and captions | Week 6, Slides 20, 24-25 |
| 10 | League Table page split into two columns | Week 6, Slides 20-21 |
| 11 | Link pseudo-classes styled | Week 6, Slides 28-29 |
| 12 | Responsive media queries added (960px, 480px) | Week 7, Slides 12-13 |
| 13 | Responsive images applied | Week 7, Slide 8 |
| 14 | Code comments added throughout | WEDE5020POE.pdf |
| 15 | External, Embedded, and Inline CSS all used | Week 5, Slides 6-11 |

---

## 4. Changelog

| **Date** | **Version** | **Change** |
| :--- | :--- | :--- |
| 18 Sept 2026 | 1.0 | Created external stylesheet `styles.css` and linked to all 5 pages |
| 18 Sept 2026 | 1.1 | Added CSS reset, base styles, and colour scheme |
| 18 Sept 2026 | 1.2 | Applied typography (Arial body, Georgia headings, cursive script) |
| 18 Sept 2026 | 1.3 | Redesigned header with centred logo and LFA divider |
| 18 Sept 2026 | 1.4 | Made navigation horizontal with hover effects |
| 18 Sept 2026 | 1.5 | Added homepage feature cards with background images |
| 18 Sept 2026 | 1.6 | Added History section and About strip |
| 18 Sept 2026 | 1.7 | Rebuilt Gallery page as 3-column grid with captions |
| 18 Sept 2026 | 1.8 | Split League page into Fixtures (left) and Table (right) |
| 18 Sept 2026 | 1.9 | Added link pseudo-classes for all 5 states |
| 18 Sept 2026 | 2.0 | Added responsive media queries at 960px and 480px |
| 18 Sept 2026 | 2.1 | Added responsive images with `max-width: 100%` |
| 18 Sept 2026 | 2.2 | Added detailed comments to all CSS and HTML sections |

---

## 5. Referencelist

MDN Web Docs. (2026). *CSS: Cascading Style Sheets* [Online]. Available at: https://developer.mozilla.org/en-US/docs/Web/CSS (Accessed: 18 September 2026).

MDN Web Docs. (2026). *Using media queries* [Online]. Available at: https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries (Accessed: 18 September 2026).

The Independent Institute of Education. (2026). *WEDE5020 Web Development (Introduction): Module Outline 2026* [Module Documentation]. The IIE.

The Independent Institute of Education. (2026). *WEDE5020 Web Development (Introduction): Portfolio of Evidence (PoE) Assessment Brief* [Module Documentation]. The IIE.

The Independent Institute of Education. (2026). *WEDE5020 Web Development (Introduction): Week 5 Slides – Introduction to CSS* [Module Slides]. The IIE.

The Independent Institute of Education. (2026). *WEDE5020 Web Development (Introduction): Week 6 Slides – CSS Decoration, Typography, and Selectors* [Module Slides]. The IIE.

The Independent Institute of Education. (2026). *WEDE5020 Web Development (Introduction): Week 7 Slides – Responsive Web Design* [Module Slides]. The IIE.

W3Schools. (2026). *CSS Responsive Web Design* [Online]. Available at: https://www.w3schools.com/css/css_rwd_intro.asp (Accessed: 18 September 2026).

W3Schools. (2026). *CSS Media Queries* [Online]. Available at: https://www.w3schools.com/css/css_rwd_mediaqueries.asp (Accessed: 18 September 2026).

W3Schools. (2026). *CSS Selectors Reference* [Online]. Available at: https://www.w3schools.com/cssref/css_selectors.php (Accessed: 18 September 2026).

---

*All sources referenced using the Harvard referencing style adapted for The IIE, as required by the WEDE5020 module guidelines (The IIE, 2026).*



W3Schools. (2026). CSS Media Queries [Online]. Available at: https://www.w3schools.com/css/css_rwd_mediaqueries.asp (Accessed: 18 September 2026).

W3Schools. (2026). CSS Selectors Reference [Online]. Available at: https://www.w3schools.com/cssref/css_selectors.php (Accessed: 18 September 2026).
