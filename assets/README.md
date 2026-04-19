# Assets

## Optional: real anatomy plate behind the hero

The hero ships with a hand-drawn SVG anatomical motif. To swap in a real
public-domain plate (Vesalius, Gray's Anatomy, etc.):

1. Download a high-resolution JPG from Wikimedia Commons. Recommended:
   - **Vesalius muscleman** — search Commons for `De humani corporis fabrica`
     plates; the standing écorché figures from Book II are iconic.
   - **Gray's Anatomy (1918) plates** — search Commons for `Gray's Anatomy plate`.
     Heart, thoracic, or full-body skeletal plates work well.
2. Save the file as `assets/hero-anatomy.jpg` (1600px wide is plenty).
3. Open `index.html` and on the `<section id="home" class="hero">` line, add
   the attribute `data-bg="photo"`:

   ```html
   <section id="home" class="hero" data-bg="photo">
   ```

The CSS already has the sepia + multiply blend treatment wired up — the image
will fade in at 28% opacity over the SVG. Tweak `opacity` in `styles.css`
(search for `[data-bg="photo"]`) to taste.

## Attribution

Public-domain works don't legally require attribution, but it's good practice.
Add a line to the footer or an `/credits` page noting the source plate(s).
