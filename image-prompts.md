# Nano Banana prompts — remaining Bhatia Arts placeholders

Style anchor for all of these: match `hero-large.png` (the real shopfront photo) —
documentary-style photography, warm golden-hour or warm tungsten indoor light,
slightly moody/cinematic color grade, real small-business setting in Punjab, India
(not stock-photo-clean, not illustrated/3D-rendered). Where a logo or shop name is
visible, it should read "BHATIA ARTS" in bold yellow lettering, matching the sign
in the hero photo. Accent colors when relevant: burnt orange (#f4623a) and teal
(#0f766e).

Each prompt lists the target file name/slot and the aspect ratio to request from
Nano Banana so it drops in without further cropping.

---

## Done

- Hero: `hero-large.png`, `hero-strip-1-press.png`, `hero-strip-2-cards.png`,
  `hero-strip-3-tshirt.png`
- "What We Do" grid: `flex.png`, `board.png`, `stickers.png`, `t-shirt.png`,
  `mementos.png`, `flyers.png`, `canopy.png`

All wired into `bhatia-arts-v2.html` / `bhatia-arts-v2.css`.

---

## About section (1 image, square 1:1)

**11. Founder / Workshop Photo** — `about-founder.png`
> A middle-aged Indian shop owner in a simple collared shirt standing inside his
> small printing workshop, arms crossed, warm confident expression, printing
> equipment and stacks of paper softly out of focus behind him, warm tungsten
> light from the side, documentary portrait photography, square 1:1.

---

### After generating

Save each file into this folder using the filename listed, then swap it in the
same way the hero photo was wired up — replace the matching
`<div class="... placeholder-img" ...>` in `bhatia-arts-v2.html` with an
`<img src="...">`, and add an `object-fit: cover; width:100%; height:100%;`
rule if the slot doesn't already have one (see `.hero-billboard img` in
`bhatia-arts-v2.css` for the pattern, including the skew/counter-skew trick for
the two hero elements that use `skewX`).
