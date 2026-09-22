# Editable Profile

## What will change
- Extend the existing profile-preferences record with a display name and locally stored avatar image; keep the current default name and “FL” initials when nothing custom is saved.
- Add a small shared profile hook so edits update all visible profile surfaces immediately and remain after refresh.
- Add a compact Edit action beside the existing Profile identity block. The editor will support name input, device photo selection, preview, save, cancel, and removing a custom photo.
- Reuse the existing avatar component for the Profile page and desktop header, preserving their current sizes and styling.
- Personalize the existing Home greeting with the saved display name without changing the page structure.

## Guardrails
- Keep all current routes, authentication behavior, learning data, institution settings, question flows, navigation, and page layouts unchanged.
- Store the avatar through the current device-based preference architecture; resize and compress it before saving to reduce storage usage.
- Validate image type and size, provide accessible labels and keyboard-friendly controls, and retain the default avatar on missing or invalid images.

## Verification
- Edit the name and upload a photo on mobile.
- Confirm Profile, Home, and the existing desktop avatar surface update immediately.
- Refresh and confirm both values persist.
- Verify removing the photo restores the default initials.
- Check the existing Profile layout at mobile and desktop sizes and confirm no console or page errors.
