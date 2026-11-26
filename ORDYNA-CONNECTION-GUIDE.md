# Connecting Beyond the Obvious with ORDYNA

ORDYNA · BUSINESS & TECHNOLOGY: "Business, rethought."

## The idea: the Thought-to-Thing continuum
Beyond the Obvious is where ideas take shape. ORDYNA is where they become something real.
The visitor never meets a plain "our other website" button. They meet a question, then a transition.

Where it appears on Beyond the Obvious:
- Home page: the "Thought-to-Thing continuum" section (open door, "Follow the idea").
- Services page: "Need it built as a product or a platform?".
- Footer link and the Ctrl K menu: "ORDYNA · Business & Technology".

What happens on click: the page dims, gold particles gather, light sweeps across, the serif title "Beyond the Obvious" dissolves into "ORDYNA", then the visitor lands on the second website.

## Status: SWITCHED ON
`assets/config.js` now points to `https://budair-ahmad.github.io/ordyna/`. Clicking the big ORDYNA block, the ORDYNA word in the headline, "Follow the idea", the footer link or the Ctrl K entry plays the transition and opens ORDYNA.

## How it was switched on (for reference)
1. Open `assets/config.js`.
2. Set `ordyna:{url:"https://YOUR-ORDYNA-ADDRESS/", name:"ORDYNA", tagline:"Business & Technology", slogan:"Business, rethought."}`.
3. Upload the file. Nothing else changes.
While `url` is empty the transition plays and a panel says ORDYNA is being prepared and collects emails (tag "ordyna").

## The return journey (build this into ORDYNA)
Link back to: `https://budair-ahmad.github.io/aBudair/?from=ordyna`
Beyond the Obvious then plays the reverse transition (ORDYNA dissolves into the serif title) and cleans the address bar.
Visitors arriving at ORDYNA carry `?from=bto`. Suggested snippet for ORDYNA:

```html
<script>
if(/[?&]from=bto/.test(location.search)){
  // show a welcome line, for example: "You followed an idea from Beyond the Obvious."
  history.replaceState(null,"",location.pathname);
}
</script>
```

## Shared identity
| | Beyond the Obvious | ORDYNA |
|---|---|---|
| Role | Thinking | Making |
| Colours | Navy #0B1421, ivory #F2EEE5, champagne #BCA77F | To be confirmed. The transition currently uses deep blue #041733, cyan #7FD8FF, periwinkle #8C9BFF as placeholders |
| Type | Cormorant Garamond, Manrope, DM Mono | To be confirmed (the transition uses Manrope bold with wide tracking) |
Send me ORDYNA's real logo and colours and I will match the transition exactly.

## Address note
The live site is a project site: `https://budair-ahmad.github.io/aBudair/`. All canonical, social and sitemap addresses use it.
- Search Console: add a URL-prefix property with that exact address and submit `sitemap.xml`.
- `robots.txt` is only honoured at a domain root, so it does nothing under /aBudair/.
