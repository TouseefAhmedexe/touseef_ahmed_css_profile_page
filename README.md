# Profile Page with CSS

The profile page from my HTML training, styled with an external stylesheet (style.css).
Task 6 of my Bloomrix internship. No JavaScript is used.

## Files
- index.html - the profile page
- style.css - all the styling
- images/ - profile photo, header background and list icon

## Inheritance examples
1. The h1 and the tagline have no color rule. They are white because they inherit
   the color of #profile-header. The footer text inherits white from #page-footer the same way.
2. Form fields and buttons do not inherit the page font by default, so they have
   font-family: inherit. This makes them use the same font as the rest of the page.

## Specificity examples
1. li sets a gray color, and .skill-item sets a blue color. The class selector (0,1,0)
   is more specific than the element selector (0,0,1), so the class color wins.
2. #top-skill is written before .skill-item, but its yellow background still wins.
   The ID selector (1,0,0) is more specific than the class selector (0,1,0).
   Source order is used only when two selectors have the same specificity.
3. nav a:link (0,1,2) is more specific than a:link (0,1,1), so navigation links are white
   and not blue.
4. input[disabled] and input[type="text"] have the same specificity (0,1,1). The disabled
   rule is written later, so it wins on the disabled field.

## Units used
px, %, rem, em, vh and vw.

## How to run
Open index.html with Live Server in Visual Studio Code, or in any web browser.