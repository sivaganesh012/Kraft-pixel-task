# Kraft-pixel-task
)
🎯 Objective:
You must replicate the specific sections shown in the Figma file using HTML and CSS from scratch, mobile-first.

DO NOT use:

Bootstrap, Tailwind, any CSS framework.

Prebuilt components/templates.

CAN use:

Basic CSS reset if you want (optional).

Flexbox/Grid for layouts.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Us - KraftPixel</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Your content goes here -->
</body>
</html>
Sample CSS media query for tablet/desktop:

css
Copy
Edit
@media (min-width: 768px) {
  /* Adjust layouts here */
}Push your project:

bash
Copy
Edit
git init
git add .
git commit -m "Initial commit for KraftPixel task"
git branch -M main
git remote add origin https://github.com/your-username/repo-name.git
git push -u origin main<section class="about-section">
  <div class="container">
    <h2 class="section-title">About Us</h2>
    <p class="section-description">Some description here...</p>
  </div>
</section>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Us - KraftPixel</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Your content goes here -->
</body>
</html>

🏗 How to proceed practically:
4.1. Open the Figma file
Open this Figma file properly:
➔ Figma link

Focus only on the sections shown here:
➔ Reference Screenshot

4.2. Structure your HTML wisely
For every section:

Wrap it inside a <section> tag.

Inside, use <div>s with meaningful class names.
Follow Figma hierarchy:

If you see headings → use <h1>, <h2>, <h3> properly.

Paragraphs → <p>.

Images → <img> with proper alt text.

Class Naming Best Practices:

Be clear and readable (about-section, team-cards, profile-img, team-name, etc.)

4.3. Start with Mobile View (mobile-first development)
What Mobile-First means:
👉 First code it for mobile (small screens) without any media queries.
👉 Then, later add styles for larger screens inside @media (min-width: 768px) {}

🔹 In style.css, your structure should look like:
4.4. Layout decisions
When you see cards, profiles, or grids in Figma:

Use Flexbox or CSS Grid for positioning.

🔹 Example for team cards:
Mobile: Cards stacked vertically.
Desktop: Cards spread horizontally or grid layout.

4.5. Spacing and Fonts
Figma will show you:

Font sizes

Margins

Paddings

Colors

Match these as close as possible.

Example:

Headings in Figma: 32px font → use font-size: 2rem;

Margin between sections: 80px → use margin-bottom: 5rem;

4.6. Images and Icons
Download placeholder images if needed or just use <img src="placeholder.jpg"> if images are not available.

Set max-width for images:
4.7. Responsive Adjustments
Inside your @media (min-width: 768px) block:

Change layouts (e.g., change from column to row flex direction).

Increase font sizes.

Increase padding/margin.

Example for a responsive container:
🔥 Special Tips
Consistency: Stick to same units (rem, %, etc.)

Responsiveness: Focus on mobile screens first. Then check tablet/desktop.

Figma Inspection Tool: Right-click → Inspect → See exact CSS properties.

Comments: You can add comments in CSS if needed (but not necessary).

No heavy animations unless the design demands it.

🧩 In short:

Step	What to do
HTML Structure	Sections, containers, divs, headings, paragraphs
CSS	Base mobile styling first
Layout	Flexbox for stacking & grids for layouts
Media Queries	For desktop view (>768px)
Clean Code	Proper class naming, indentation
Match Figma	Fonts, colors, spacing, structure
🧩 Basic Wireframe (Structure to Follow)
1. About Us Section (Top Introduction)
2. Core Values Section (Usually Cards or Boxes)
3. Mobile View: Cards stacked vertically.

Desktop View: Cards in rows/grid.

3. Our Team Section (Team Member Profiles)
4. Contact or CTA (Optional if visible)

🖼️ Visual Layout Hierarchy (Roughly)
pgsql
Copy
Edit
-----------------------------------------
| About Section                        |
|  Title                                |
|  Description                         |
-----------------------------------------
| Core Values Section                  |
|  Title                                |
|  Cards (Icon + Title + Desc)         |
|  Cards (Icon + Title + Desc)         |
|  Cards (Icon + Title + Desc)         |
-----------------------------------------
| Team Section                         |
|  Title                                |
|  Team Card (Image + Name + Role)     |
|  Team Card (Image + Name + Role)     |
|  Team Card (Image + Name + Role)     |
-----------------------------------------
| (Optional) Contact/CTA Section       |
|  Title + Button                      |
-----------------------------------------
📏 Basic CSS Plan

Element	Mobile View	Desktop View
Container	Width: 90%	Width: 80%, max-width: 1200px
Section padding	2rem top-bottom	4rem top-bottom
Section title font size	2rem	2.5rem
Cards layout	Flex-direction: column	Flex-direction: row / grid
Spacing between cards	1.5rem	2rem
Image sizing	100% width	Fixed width/height if needed
🏗 Final Reminder:
✅ Start Mobile-First →
✅ Use proper semantic tags →
✅ Use custom CSS (no Bootstrap) →
✅ Clean, readable class names →
✅ Good structure and indents →
✅ Responsive at 768px breakpoint.
