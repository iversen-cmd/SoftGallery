Kara BC — the SoftGallery.art brand face
========================================

The site is set up to use Kara BC everywhere the brand speaks: the front
page, the navigation, the headings and the signage inside the gallery.
The typeface file is not included, because the Design.com logo licence
covers the logo artwork only — it does not license the typeface.

To switch the site to the real face, drop ONE of these in beside this file:

    KaraBC.woff2      (best: smallest, universally supported)
    KaraBC.woff
    KaraBC.otf        (works, but two to four times the download)

Nothing else needs changing. The @font-face rule at the top of index.html
already points here, and until a file exists the browser falls back
silently to Barlow Condensed.

If the family ships as separate weight files, add one @font-face block per
weight with a matching font-weight, or use a variable font and keep the
existing "font-weight: 300 700" range.

Where the fallback came from
----------------------------
Barlow Condensed was not a guess. The wordmark outlines in Print.svg were
measured:

    cap height          33.84 units
    stem width           3.29 units   -> stem/cap 9.7%  (regular, not light)
    bar / stem ratio     1.00         -> perfectly monolinear
    glyph width          0.47-0.55 of cap height  (condensed)
    tracking in the logo 0.65 em
    tagline cap height   49% of the name  (matches the stated 23pt / 47pt)

Barlow Condensed is the closest freely licensable face on weight, width and
stroke modulation. The 0.65 em tracking is a logo treatment and is NOT
applied to text — headings use 0.01-0.03 em.
