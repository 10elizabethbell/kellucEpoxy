# Kelluc Epoxy — handoff at ~60%

**Live:** https://10elizabethbell.github.io/kellucEpoxy/ · **Repo:** https://github.com/10elizabethbell/kellucEpoxy · **Built:** 2026-10-20 from Muse brief (Muse run 2026-10-20, found in "Essex County Contractor Referrals") · **Call Sheet:** site set (entry added; Muse hadn't listed it)

## What's built
- One page, calm band style: paper header (logo badge + wordmark, Facebook icon top right) → photo hero → "A floor we'd put in our own home" (paper, 3 claims: two from their post plus flake finishes & custom colours) → "What we transform" service rows (navy) → recent work (paper, one photo + "Click to see more of our work." Facebook row under it) → How it works (deep navy, 3 steps) → free-quote form (paper) → close (navy, "Transform your concrete into something you'll love." from their page description) → footer.
- Palette from the logo: graphite navy `#1f2836` / deep `#141a25` stand in for the logo's black, red `#d42a2f` is the one accent fill, `#b01e24` when red is text on light, `#ff6b6b` on navy.
- Hero: their own flake-finish front entrance (the only photo obtainable) under a dark navy overlay, eyebrow "Booking indoor jobs all fall & winter", H1 "Concrete you'll love in Windsor-Essex" with the letter bounce-in (waits up to 700ms for Cal Sans), promise "Durable, beautiful and built to last." (their logo line). The photo is blurred 3px on phones so the railing never runs through the headline; white text samples at 9.2:1 or better on the worst pixel.
- Contact is **Facebook Messenger only**: hero ghost button, the floating circle (shows after the hero, hides over the form and the closing band), and the closing button open `m.me/100072376201501` with "Hi Kelluc Epoxy! I found your website and I'd like a free quote." pre-filled. The form (job chips, finish, name, town, size) composes a message, copies it to the clipboard and opens Messenger with `?text=`; a "Copy message / Open Messenger" fallback box appears in case Messenger drops the text.
- `CONFIG` at the top of the script: `FB_ID`, `PHONE`, `PHONE_LABEL`, `FLOAT`. Setting `PHONE` shows the tap-to-call number top right in place of the Facebook icon.
- og.jpg (1200×630) for the Facebook link preview; favicon and home-screen icon are the red triquetra cropped from the logo.

## Assumptions I made
- **White text on red fills** instead of the calm style's navy-on-accent: navy on this red is ~2.9:1 and fails; white is 5.3:1. Hover darkens the red.
- **"We" voice**, from "we're still working" / "we're booking" in their posts. Owner name unknown, so no "I'm …" intro.
- "A floor we'd put in our own home." and "You'll walk across it every day, so we treat it that way. One floor at a time, done right." are my words built on their sign-off ("one floor at a time"). Swap in the owner's own if they give any.
- Services list = the surfaces named in their caption (garages, basements, porches, front entrance) plus "flake finishes and custom colours". "Have another concrete surface in mind? Ask us." stands in for their "& more".
- How it works step 3, "Indoor projects all fall and winter", is from their seasonal post; drop it in spring.
- The form's town placeholder names Windsor, LaSalle, Tecumseh as examples only (real Windsor-Essex towns; not claimed as a service list).
- `m.me/100072376201501` redirects to Messenger thread `105100248561993` (checked with curl), so the link resolves. Whether Messenger keeps the `?text=` pre-fill varies by app version; hence the clipboard copy and fallback box.

## Placeholders and gaps
- **No phone and no email** anywhere (brief). Header has no number; footer has no email. Both appear by setting `CONFIG.PHONE` (email needs a line added to the footer).
- **One photo only**: the front-entrance after shot (800×600). The garage floor and the before/during shots in the group post weren't retrievable (group/timeline restricted). The house number was cropped out and the photographer's reflection in the right window blurred. Hero photo is upscaled on desktop; the heavy overlay hides the softness.
- No reviews, prices, hours, years in business, owner name: none shown.
- Logo is the 720px Facebook profile image (JPEG); no vector.

## Questions for the owner
- A phone number that takes calls/texts? An email for the footer?
- Your first name (for "you'll deal with …")?
- The garage floor photos and the before/during set from the 2026-10-20 post, plus any other jobs (before/after pairs would make a slider).
- Which towns you'll travel to, beyond "Windsor-Essex County and surrounding areas"?
- Do you do commercial / shop floors, or homes only?
- Any reviews from customers you're happy to quote?

## Ideas not built (yours to pick)
- **Opt-in signature motion (runner-up worlds):** (1) *flake broadcast* — coloured vinyl flakes scattered across the hero that settle into a glossy coat as you drag (best fit); (2) a squeegee wipe that pulls glossy epoxy across bare grey concrete in the hero; (3) a gloss sheen that follows the finger over a flake floor; (4) custom-colour swatches that recolour a floor tile; (5) a "cold weather's coming" seasonal band that swaps by month.
- A before/after slider once the owner supplies a pair.
- A finish/colour picker in the form (chips with real flake swatches) once we have their swatch photos.
- **Impeccable findings kept against its advice (your calm-style choices):** four eyebrow pills (craft floor bans them), the diagonal band texture (detector `repeating-stripes-gradient`, suppressed for index.html in `.impeccable/config.json`), the H1 bounce-in (~1.5s), the floating circle, Cal Sans. `flat-type-hierarchy` is also suppressed: what's left is the 14/16/18 UI text steps.
- **Impeccable suggestions not applied:** a pulse on the pre-selected chip when a service row is tapped; hiding the float while a service row's arrow is in the bottom 80px (it can briefly sit over the arrow); a 1px border on form fields (the `#e7eaf0` fill on white is 1.2:1, the house `--field` choice); a header shadow after scrolling (header isn't sticky); "See more of our work on Facebook" wording (kept your "Click to see more of our work.").
- Work card shows the same photo as the hero (it's the only one). Swap in a garage-floor shot when available.

## Not verified
- Real Messenger hand-off on iOS and Android (in-app browser and Safari/Chrome), including whether `?text=` is kept.
- Clipboard copy inside Facebook's in-app browser (may be blocked; the fallback box covers it).
- Real-device touch and frame rate on old phones (automated checks ran in Playwright Chromium and WebKit at 360/390/430px).
