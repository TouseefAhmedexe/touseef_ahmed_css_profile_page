# Profile Page with CSS

The profile page from my HTML training, styled with an external stylesheet (style.css).
Task 6 of my Bloomrix internship. No JavaScript is used.

## Files
- index.html - the profile page
- style.css - all the styling
- images/ - profile photo, header background, and bullet icon

## Inheritance Examples
1. **Header text color:** `#profile-header` sets `color: white;`. The `<h1>` and `.tagline` inside it inherit white text color without needing individual rules.
2. **Form font inheritance:** Form inputs and buttons use `font-family: inherit;` to inherit the body's font family stack instead of relying on browser defaults.

## Specificity Examples
1. **Class vs Element:** `li` sets color `#444444` `(0,0,1)`, but `.skill-item` sets color `#0b3d91` `(0,1,0)`. The class rule is more specific and wins.
2. **ID vs Class:** `#top-skill` `(1,0,0)` sets a yellow background, overriding `.skill-item` `(0,1,0)`. The rule `.skill-item#top-skill:hover` `(1,1,0)` ensures hover transitions work smoothly on `#top-skill`.
3. **Descendant & Pseudo-class vs Element:** `nav a:link` `(0,1,2)` overrides global `a:link` `(0,1,1)` to keep navigation links white instead of blue.

## Units Used
`px`, `%`, `rem`, `em`, `vh`, and `vw`.

## DevTools Verification
Inspected elements using Browser Developer Tools:
1. `h1`: Verified font-size (2.5rem), uppercase transform, and text-shadow application.
2. `#top-skill`: Verified ID specificity (1,0,0) correctly overriding `.skill-item` (0,1,0) styles.
3. `.profile-photo`: Verified box-shadow and outline rendering.
4. `input[type="text"]`: Verified padding, border-radius, and inherited font family.
5. `#page-footer`: Verified radial-gradient background and typography rules.

## How to Run
Open index.html with Live Server in Visual Studio Code, or in any web browser.