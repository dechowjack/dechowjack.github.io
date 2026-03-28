# Homepage Sticky Hero Design

Date: 2026-03-28
Status: Approved for implementation review

## Summary

Adjust the homepage so the top navigation remains fixed and the homepage hero banner image uses a desktop-only fixed-background effect while the rest of the page scrolls normally.

## Scope

- Apply the change only to the homepage.
- Keep the existing fixed masthead behavior.
- Use the current homepage hero section and image source.
- Limit the fixed-background behavior to desktop layouts.
- Preserve normal scrolling behavior on tablet and mobile layouts.

## Goals

- Keep the navigation visible while users scroll.
- Make the homepage banner image feel visually fixed on desktop.
- Avoid restructuring the homepage layout or changing the hero content model.
- Minimize CSS risk by building on the current Minimal Mistakes override pattern.

## Non-Goals

- Do not make the full hero section itself sticky or fixed.
- Do not apply the change to research, publications, CV, or other interior pages yet.
- Do not redesign hero copy, buttons, spacing, or page information architecture.

## Current Context

- The masthead is already fixed globally in `assets/css/main.scss`.
- The homepage uses the `home-academic` body/page class and renders a hero through Minimal Mistakes `header.overlay_*` front matter.
- The homepage hero already uses a homepage-scoped `background-attachment: fixed` rule in source, but the current task is to validate and tighten that behavior as the intended solution for the homepage only.
- Mobile styles already reset hero background attachment to normal scrolling, which should remain in place.

## Recommended Approach

Use homepage-scoped CSS on `.home-academic .page__hero--overlay` to preserve a fixed-background image effect on desktop while leaving the masthead fixed globally.

Implementation intent:

- Keep `.masthead` unchanged.
- Keep or refine the homepage-only `background-attachment: fixed` behavior on desktop.
- Ensure the fixed masthead offset still clears the hero and page content correctly.
- Preserve the existing mobile breakpoint behavior that switches hero background scrolling back to normal.

## Rationale

This is the smallest viable change that matches the requested effect. It avoids introducing new stacking, overlap, or scroll-container complexity while letting the homepage act as the test case before considering rollout to other pages.

## Risks

- `background-attachment: fixed` can behave inconsistently across browsers and is commonly reduced or disabled on mobile, which is why the effect remains desktop-only.
- The fixed masthead and hero may need minor spacing confirmation to avoid visual overlap at the top of the page.

## Validation

- Confirm the homepage masthead stays fixed while scrolling.
- Confirm the homepage hero image appears fixed on desktop as content scrolls.
- Confirm tablet and mobile fall back to normal hero scrolling.
- Confirm no new overlap, clipping, or jumpiness appears around the top of the homepage.
