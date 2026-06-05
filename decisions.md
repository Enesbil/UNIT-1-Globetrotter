# Globetrotter: Decisions Log

## Milestone 0: Setup and Planning
- Destination chosen: Istanbul
- Primary audience: Western/USA Youth (Gen-Z, 14-29 Years Old)
- One design decision that reflects the destination: Emphasis on aspects attractive to the target audience. E.g. Trendy TikTok shops, famous istanbul cats as opposed to greater emphasis on history or architecture
- Wireframe format used (hand-drawn / Figma / other): Hand drawn

## Milestone 1: HTML Structure
- Pages I went with: Home (index), Top Attractions, Eat (this is my food guide), and Cattractions (this is the photo gallery but its all cats since thats kind of Istanbul's whole thing).
- Kept the nav and footer identical on every page and basically copy pasted them. I wasnt leaning on JS for this so theres no include system, which means if I change one I have to remember to update all four.
- Tried to use semantic tags instead of div soup: nav, main, section, footer, and figure plus figcaption for the gallery captions since thats the proper way to caption an image.
- Wrote the attraction blocks and the meal blocks in a repeatable pattern so each one shares the same structure and ends up styled the same.

## Milestone 2: CSS Styling
- Put all my colors and shadow values in :root as variables so I only set them in one place. Made later tweaks a lot less painful.
- Palette is bordeaux, cream, ink, saffron, and a bosphorus green. Bordeaux is the main one because its a big color in Turkish culture so it felt right for the city.
- Pulled in two Google Fonts: Bricolage Grotesque for the big chunky headings and Inter for the body text.
- Committed to the neobrutalist look from my design spec: hard 3px ink borders, flat color blocks, and offset drop shadows with no blur.

## Milestone 3: Flexbox Layout
- Nav is flexbox with space-between so the logo sits on the left and the links sit on the right.
- The home hero is two flex columns split 50/50, one side for Europe and one for Asia.
- Footer and the "where next" button rows are flexbox too.
- I also brought in CSS Grid on the attractions page and the home features section because I wanted the pages to not all look the same, and grid made the zigzag image then text layout way cleaner than flexbox would have.

## Milestone 4: Responsive Design
- Main breakpoints I used: phones at 768 and under, tablets from 769 to 1023, and desktop at 1024 and up.
- Turned the navbar into a hamburger menu on small screens. Did it with a CSS only checkbox hack so I didnt have to add any JS just for the menu.
- The grids collapse to a single column on mobile and I reordered the cells so each image shows up right before its own text instead of getting separated from it.
- Fixed the attraction borders so the images stretch to fill the full row height. Before that the divider lines were stopping halfway down at medium screen sizes and it looked broken.
- Footer stacks the newsletter on top of the brand block once the screen gets tight, around 920 and under.
- Added a reduced motion media query so the hover and bounce animations turn off for anyone who has that setting on, which also lines up with my note about simplifying motion on smaller screens.

## Stretch Features
- Additional media: embedded a Google Map of the Sultanahmet area on the attractions page.
- Enhanced layouts: used CSS Grid on the attractions page and the home features grid.
- Travel newsletter form: theres a signup form in the footer. It doesnt save anything, it just clears the input and shows a little thanks message.
- Custom styling: added the Google Fonts plus a bunch of CSS properties we never touched in the labs, like aspect-ratio, object-fit, position sticky, clamp(), CSS columns for the cat gallery, and -webkit-text-stroke for the outlined numbers.
- Deployment: deployed the site on Render as a static site. Since its just plain HTML and CSS with no build step I added a render.yaml blueprint that points at the repo root and serves index.html, so Render can pick it up straight from GitHub.
