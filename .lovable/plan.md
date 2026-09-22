# Dark-mode institution refinement

## Scope
- Replace the global dark brown foundation with deep neutral black and charcoal tokens.
- Keep every light-mode palette unchanged.
- Preserve institution selection, logos, navigation, page structure, learning data, and all study logic.

## Changes
- Update only the `.dark` semantic foundation in `src/styles.css`: background, cards, popovers, muted/secondary surfaces, default answers, text, and shadows become neutral black/charcoal.
- Refine each institution’s existing `dark` palette in `src/data/institutions.ts`:
  - PKN STAN: deep navy and richer blue accents.
  - UNPAD: golden yellow and orange accents over neutral charcoal.
  - UI: retain its gold identity over neutral charcoal.
  - ITB: retain its blue/cyan identity over neutral charcoal.
- Add institution-aware dark Liquid Glass variables through the existing palette pipeline, so glass stays mostly charcoal with a restrained accent tint.
- Keep home surfaces dark and use institution color only in borders, glow, buttons, progress, selected states, and existing decorative details.

## Verification
- Check PKN STAN, UNPAD, UI, and ITB in Dark Mode on Home and Profile.
- Confirm neutral black/charcoal page backgrounds, readable text, subtle glass tint, no brown/sepia appearance, no horizontal overflow, and no console errors.
- Recheck Light Mode to ensure its existing appearance is unchanged.
