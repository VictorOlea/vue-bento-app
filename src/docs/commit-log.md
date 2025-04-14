# 📘 Internal Commit Log

This document tracks meaningful commits for internal reference, performance history, and development decisions in the Bento Vue 3 application.

---

## feat(app): update project description and add favicon

- Updated the project description in `App.vue` to better reflect the app's purpose.
- Added a favicon to `index.html` for improved branding and browser tab visibility.

---

## style(css): fix bullet point visibility in section-content list

Adjusted list styling in section-content to ensure bullet points remain visible.
Set list-style-position to inside and verified alignment within padded container.

---

## fix(types): add shim for CSS Modules and ensure TS config includes it and remove bentoTestDesign component"

Adds type declaration for \*.module.css files to fix import errors in strict TS mode.
Also ensures the src/types directory is included in tsconfig.app.json.

- Remove bentoTestDesign component

---

## chore(test): comment unused sectionStyle in BentoTestDesign to fix build error

Keeps the BentoTestDesign.vue component for reference purposes, but comments out the unused sectionStyle variable to prevent TypeScript build failure on Netlify.

---

## docs: add internal commit log for tracking project changes

Creates a new documentation file under the `docs/` directory to keep a historical record of significant commits.

- Includes detailed commit messages for style, performance, and layout changes.
- Helps maintain traceability of key technical decisions.
- Serves as a reference for future improvements and onboarding.

---

## perf(assets): convert images to WebP and reduce file size for faster loading

Replaces original image assets with WebP format to improve loading performance and reduce bandwidth usage.

- All image files were optimized and converted to WebP.
- File sizes significantly reduced without noticeable quality loss.
- Cards now load faster, especially on slower connections.

---

## fix(style): apply global border-box to fix layout overflow and alignment

Adds a global box-sizing rule to ensure consistent layout behavior across all components.

- Fixes layout misalignment in BentoCard when resizing the viewport.
- Prevents padding from causing overflow or affecting element width calculations.
- Ensures all elements, including pseudo-elements, inherit border-box behavior.

---

## refactor(grid): replace fixed row layout with auto-rows for responsive height

Replaces `grid-template-rows` with `grid-auto-rows` in the BentoGrid component to allow the grid to grow dynamically based on card content.

- Removed hardcoded row count (previously causing empty space in some screen sizes).
- Auto-rows now handle dynamic card arrangements more flexibly.
- Media queries for column responsiveness are retained.
- Cards still receive `:col-span` and `:row-span` individually via props.
