# Photo Update Instructions — Blankets Consulting Group Website

There are **3 photo placeholders** across 2 pages that need to be replaced with real photos of Jorge Mosquera.

---

## Photo Requirements

Before making any edits, prepare your photos:

- **Format:** JPG or WebP (recommended for web)
- **Recommended dimensions:** At least **800 × 1000 px** (portrait orientation, roughly 4:5 ratio)
- **File size:** Under 500 KB per image (compress at [squoosh.app](https://squoosh.app) if needed)
- **Tone:** Professional headshot or business portrait — suit or business casual, neutral/clean background preferred
- **Save files to:** The same folder as your HTML files (e.g., `jorge-hero.jpg`, `jorge-about.jpg`)

---

## Placeholder 1 — Homepage Hero (Right Column)

**File:** `index.html`
**Location on site:** Top of the homepage, right side of the hero banner
**Around line:** 1034

### Find this block and delete it:

```html
<div class="hero-photo" role="img" aria-label="Professional photo placeholder">
  <div class="hero-photo-icon">
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
      <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z" />
    </svg>
  </div>
  <span>Photo Coming Soon</span>
</div>
```

### Replace it with:

```html
<img
  class="hero-photo"
  src="jorge-hero.jpg"
  alt="Jorge Mosquera, Founder of Blankets Consulting Group"
  loading="eager"
/>
```

### Also update the CSS for `.hero-photo` in the `<style>` block of `index.html`:

Find these lines (around line 338):
```css
.hero-photo {
  background: linear-gradient(145deg, #243555 0%, #1B2A4A 100%);
  border-radius: 12px;
  aspect-ratio: 4/5;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: 1px solid rgba(255,255,255,0.08);
  gap: 16px;
}
```

Replace with:
```css
.hero-photo {
  border-radius: 12px;
  aspect-ratio: 4/5;
  width: 100%;
  object-fit: cover;
  object-position: center top;
  display: block;
}
```

---

## Placeholder 2 — Homepage "Meet Jorge" Section (Left Column)

**File:** `index.html`
**Location on site:** "Meet Your Strategic Partner" section, left side
**Around line:** 1269

### Find this block and delete it:

```html
<div class="jorge-photo" role="img" aria-label="Jorge Mosquera photo placeholder">
  <div class="jorge-photo-icon">
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
      <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z" />
    </svg>
  </div>
  <span>Photo Coming Soon</span>
</div>
```

### Replace it with:

```html
<img
  class="jorge-photo"
  src="jorge-meet.jpg"
  alt="Jorge Mosquera, Founder of Blankets Consulting Group"
  loading="lazy"
/>
```

### Also update the CSS for `.jorge-photo` in the `<style>` block of `index.html`:

Find the existing `.jorge-photo` rule (around line 701) and replace it with:
```css
.jorge-photo {
  border-radius: 12px;
  width: 100%;
  aspect-ratio: 4/5;
  object-fit: cover;
  object-position: center top;
  display: block;
}
```

> **Tip:** You can use the same photo file for both hero and "Meet Jorge" (just reference the same filename), or use two different crops if you'd like a variety.

---

## Placeholder 3 — About Page Hero (Left Column)

**File:** `about.html`
**Location on site:** Top of the About page, left column
**Around line:** 870

### Find this block and delete it:

```html
<div class="about-hero-photo" role="img" aria-label="Professional portrait photo of Jorge Mosquera — coming soon">
  <div class="about-photo-icon">
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
      <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z" />
    </svg>
  </div>
  <div class="about-photo-name">Jorge Mosquera, PMP</div>
  <span class="about-photo-label">Photo Coming Soon</span>
</div>
```

### Replace it with:

```html
<img
  class="about-hero-photo"
  src="jorge-about.jpg"
  alt="Jorge Mosquera, PMP — Founder of Blankets Consulting Group"
  loading="eager"
/>
```

### Also update the CSS for `.about-hero-photo` in `about.html`:

Find the existing `.about-hero-photo` rule (around line 312) and replace the full block with:
```css
.about-hero-photo {
  border-radius: 12px;
  width: 100%;
  aspect-ratio: 4/5;
  object-fit: cover;
  object-position: center top;
  display: block;
}
```

You can also delete the now-unused CSS rules for `.about-photo-icon`, `.about-photo-label`, `.about-photo-name`, and the `::after` pseudo-element that were part of the old placeholder styling.

---

## Summary Checklist

- [ ] Photo files ready (compressed, properly named, placed in the website folder)
- [ ] Placeholder 1 replaced in `index.html` (Hero section)
- [ ] Hero photo CSS updated in `index.html`
- [ ] Placeholder 2 replaced in `index.html` (Meet Jorge section)
- [ ] Meet Jorge photo CSS updated in `index.html`
- [ ] Placeholder 3 replaced in `about.html` (About page hero)
- [ ] About page photo CSS updated in `about.html`
- [ ] Preview all three pages in a browser to confirm photos display correctly

---

*Instructions prepared for Blankets Consulting Group — April 2026*
