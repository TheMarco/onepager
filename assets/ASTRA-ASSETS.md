# GPT-6 Astra portfolio directions

Four standalone HTML designs added as index34.html through index37.html. Inline CSS and JavaScript; no build step or runtime package dependencies. Fonts and images are local assets.

## Fonts

- Space Grotesk, variable weight 300–700: `astra-sans.woff2`
- Barlow Condensed, weight 700: `astra-condensed.woff2`
- DM Mono, weight 400: `astra-mono.woff2`

Downloaded from Google Fonts, Latin subsets. Their SIL Open Font Licenses are included in this directory.

## Original artwork

The four concept artworks were generated with the built-in image_gen tool for these portfolio directions. They illustrate the design concepts; they are not photographs of Marco's commissioned work. Project references and career details come from the existing portfolio pages.

Final website assets: `shots/astra-monolith.webp`, `shots/astra-playform-cutout.webp`, `shots/astra-altitude.webp`, `shots/astra-afterimage.webp`. Each is an optimized WebP conversion of the original generated PNG, with unchanged composition. Homepage thumbnails `shots/shot34.png` through `shots/shot37.png` are real Chromium captures of the implemented pages.

## Generation prompts

### monolith

Use case: stylized-concept. Create an extraordinarily refined architectural photograph for a high-end experimental portfolio website, wide landscape 3:2 composition. A monumental minimalist brutalist concrete structure, a tall rectangular slab with an enormous perfect circular void cut through it, standing on a glossy shallow reflecting pool. Fine weathered silver concrete. Cold overcast sky, long horizontal horizon, a tiny human figure for scale at far right. Black and white only, smoky gray and white, sophisticated art direction, photographed on large-format film, deep sculptural chiaroscuro, sculptural building occupies center-right two thirds and lower area. The left and top have calm pale-gray negative space. Actual compelling realistic architecture, not illustration, no text, no logos, no interface, no borders. Entire canvas one photograph.

### playform

Use case: stylized-concept. Create a delightfully sophisticated tactile 3D art sculpture for a playful avant-garde product designer portfolio, landscape 3:2. A huge inflated tubular vermilion orange-red knot, looping and intertwining into a loose abstract asterisk, with gorgeous smooth matte rubber, slight grain and small seam details. Floating at slight diagonal above a pale buttery-yellow seamless studio background with a soft natural grounded shadow. Inflated form should be substantial, asymmetric and sculptural, occupying center of frame, with generous negative space all around. Art directed like a premium design festival campaign photographed with an 80mm lens. Warm yellow monochrome ground, vivid tomato-red object only. No text no typography no logo no graphic overlays, no other objects.

### altitude

Use case: photorealistic-natural. Create a breathtaking cinematic alpine landscape photograph for a world-class outdoor-inspired designer portfolio, wide landscape 3:2. A jagged slate-gray mountain peak towering above wisps of mist, dark green alpine conifer forest across lower third, a winding pale hiking path on the right foreground leading the eye into mountains. Atmospheric depth, ethereal low cloud and delicate sun rays. Restrained silver-gray sky in top quarter, deep forest green, muted evergreen and slate palette. Sharp foreground texture, soft distant landscape, analog outdoor photography on medium format, grand and cinematic, contemplative dawn light. Wide view, no buildings, no people close up, no text or logos or watermark. Avoid generic oversaturated travel colors.

### afterimage

Use case: stylized-concept. Create a stunning experimental darkroom botanical artwork for an avant-garde digital designer portfolio, landscape 3:2. Extreme closeup of one sculptural calla lily, its elegantly curled flowing petal fills most of the right two-thirds, thin arcing stem descends into bottom. Solarized analog photography, glowing vermilion orange and copper petal highlights, electric pale blue silver rim lines, very dark almost-black navy background. Organic sculpture with a liquid metal photographic quality, extraordinary delicate fine grain and deep rich contrast. Inspired by experimental color darkroom processes and contemporary fine art photography. Left third mostly dark negative space. Full bleed entire canvas single artwork, no labels no text no graphic overlays no border.


### Playform transparent cutout refinement

Built-in image_gen edit of the Playform artwork. Prompt: Extract this exact red inflated rubber knot sculpture onto a genuinely transparent background. Remove the yellow backdrop entirely including through all openings of the knot. Preserve exactly the sculpture's shape, colors, bright red orange rubber material, fine grain, seams, camera angle and studio lighting. Keep every part of the knot fully visible with generous transparent padding all around. The soft shadow below can be removed. Output true alpha transparency, not a checkerboard texture. No text or new objects.

The final WebP preserves the generated alpha channel.

## Validation

- 56 Chromium interaction, responsive-width, internal-link, and homepage checks passed.
- Desktop and phone captures verified in light and dark color schemes; no horizontal overflow or missing local assets in the four new pages.
- Axe WCAG A/AA checks: zero detected violations on all four pages, in both light and dark modes.
- Local desktop Lighthouse: 100 performance, accessibility, best practices, and SEO for all four pages. Measured against the local static server with provided (unthrottled) network conditions.
- No build step is required. Preview from the repository root with `python3 -m http.server 8765 --bind 127.0.0.1`, then open `http://127.0.0.1:8765/index.html#astra-pages`.
