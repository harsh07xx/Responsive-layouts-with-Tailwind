# Contributing

Thanks for considering a contribution to Signal House's site.

## Getting started

1. Fork the repo and clone it locally.
2. This is a static site with no build step — open `index.html` directly, or run a local server:
   ```bash
   npm start
   ```
3. Make your changes.
4. Test in at least one desktop and one mobile-width browser view.

## Guidelines

- Keep it a single static `index.html` unless a build step is explicitly agreed on.
- Match the existing code style (2-space indentation — see `.editorconfig`).
- Avoid adding new dependencies unless necessary.
- Respect `prefers-reduced-motion` for any new animation.
- Test that scroll-reveal, marquee, and form interactions still work after your change.

## Submitting changes

1. Create a branch: `git checkout -b fix/short-description`
2. Commit with a clear message.
3. Open a pull request describing what changed and why.
