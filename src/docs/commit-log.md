# 📘 Internal Commit Log

This document tracks meaningful commits for internal reference, performance history, and development decisions in the Bento Vue 3 application.

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
