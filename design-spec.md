# Istanbul Guide: Design Spec

**Vibe:** Neobrutalist UI × Istanbul. Bold, warm, culturally-grounded. Magazine energy, not tourism-brochure.

## Palette
- `#7A1F2B` Bordeaux: primary
- `#F4EBD9` Cream: background
- `#0E0E0E` Ink: borders, text
- `#E8B84A` Saffron: accent / hover
- `#1F4A3A` Bosphorus green: secondary accent

## Type
- Display: **Bricolage Grotesque** (or **Fraunkfurter / Anton**): chunky, opinionated headings
- Body: **Inter**: clean, neutral, readable

## Neobrutalist rules
- Hard 2–3px ink borders on every card/button/image
- Offset drop shadows: `4px 4px 0 #0E0E0E` (no blur)
- Flat color blocks, no gradients
- Buttons: solid bordeaux fill, ink border, saffron on hover, shift -2px/-2px on hover
- Images: hard borders, no rounded corners (or chunky 8px max)

## Cultural accents (use sparingly)
- Turkish embroidery / İznik tile pattern as a divider strip between sections (1 per page max)
- Turkish-language word drops in headings (e.g., "merhaba," "lezzet," "şehir") with English subhead

## Voice
- Gen-Z, confident, slightly cheeky. "Istanbul's the only city on two continents and yes, the cats really do run the place."
- No travel-blog clichés ("hidden gem," "must-see," "bucket list").

---

# Home Page Spec

**Sections, top → bottom:**

1. **Nav bar**: sticky, cream bg, ink border-bottom. Logo wordmark left ("İSTANBUL"), links right (Home / Attractions / Eat / Gallery).

2. **Hero**: full-width, ~85vh.
   - Big bordeaux block, left side: oversized display headline ("merhaba, İstanbul.") + 1-sentence subhead + CTA button ("Start exploring →").
   - Right side: hero image (`opener-2.png`) with hard ink border + saffron offset shadow.

3. **Intro strip**: cream bg, ~3 sentences. What this site is, who it's for, why Istanbul. Set in larger body type, not display.

4. **"Why Istanbul" trio**: 3 flat cards, side-by-side on desktop, stacked on mobile. Each = emoji/icon + 2-word title + 1-sentence pitch. (e.g., "Two Continents," "Cat Capital," "TikTok Bazaar")

5. **Embroidery divider**: single decorative strip, full-width.

6. **Page teasers**: 3 cards linking to Attractions / Eat / Gallery. Each = image + title + one-line tease + arrow. Stagger the offset-shadow colors (bordeaux, saffron, green).

7. **Footer**: ink bg, cream text. Single line + nav repeat.

## Layout
- Flexbox column for the page; flex-row for hero, trio, teasers
- Desktop: 1200px max-width, centered
- Mobile (<768px): everything stacks, hero image moves below text
