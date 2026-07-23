# Build notes

- Reference review and project inspection — 12 minutes (actual)
- Page structure, styling, and interactive behavior — 24 minutes (actual)
- Elementor export packaging — 7 minutes (actual)
- Responsive visual QA and screenshots — 11 minutes (actual)

**Total — 54 minutes (actual)**

## Deliverables

- `zoominfo-company-profile-elementor-template.json`: Elementor template export with an HTML widget mount.
- `preview.html`, `profile.css`, `profile.js`: standalone, dependency-free preview and its source assets.
- `screenshots/`: captures at 1440px, 768px, and 375px after QA.

## Elementor import

1. In WordPress, upload `preview.html`, `profile.css`, and `profile.js` to Media Library or a child-theme directory, then replace the three `/wp-content/uploads/...` paths in the exported HTML widget if their final paths differ.
2. In Elementor Templates, import `zoominfo-company-profile-elementor-template.json`.
3. Insert the template into the target page.

The design intentionally uses original copy, abstract placeholder marks, and custom styling; no ZoomInfo text, logos, images, or CSS were copied.

## Verification

- Verified JSON parses successfully as an Elementor template file.
- Verified at 1440px, 768px, and 375px via a local browser render.
- Verified tabs activate their corresponding panel, the intelligence modal opens, and the About disclosure expands.
