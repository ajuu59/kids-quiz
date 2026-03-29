# AGENTS.md

## Project overview
This project is a simple HTML5 quiz game for kids.

The app teaches:
- countries
- capitals
- currencies

The app supports:
- English
- German
- mobile browsers on Android and iPhone
- simple one-file architecture

Main goal:
Keep the app easy to understand, easy to run, and easy to extend.

## Tech stack
- HTML5
use https://github.com/knadh/oat UI as much as possible
- CSS3
- Vanilla JavaScript
- No framework
- No build step
- No backend

## Architecture rules
- Prefer a simple structure.
- Keep the app runnable by opening `index.html` directly in a browser.
- Avoid unnecessary libraries.
- Do not introduce React, Vue, Angular, Node backend, or database unless explicitly requested.
- Keep the project beginner-friendly.
- Prefer readable code over clever code.

## File structure
Preferred structure for now:
- `index.html` for the full app

If the app grows, it may be split into:
- `index.html`
- `css/style.css`
- `js/app.js`
- `js/data.js`

But do not split files unless it clearly improves maintainability.

## Functional requirements
The app should support:
- quiz mode: country → capital
- quiz mode: country → currency
- quiz mode: capital → country
- mixed quiz mode
- score tracking
- restart/play again
- language switch between English and German
- mobile-friendly layout

## Language rules
- All visible UI text must support both English and German.
- When adding new UI text, add translations for both languages.
- Keep wording simple and child-friendly.
- Do not use complex grammar.
- Keep labels short and clear.

## Mobile compatibility rules
- The app must work well on:
  - iPhone Safari
  - Android Chrome
- Use large tap targets for buttons.
- Avoid hover-only interactions.
- Keep layout responsive for small screens.
- Prefer event listeners over fragile inline browser-specific behavior when reliability is important.
- Do not add features that break local browser execution.

## UX rules
- Design for kids.
- Keep the UI colorful, simple, and friendly.
- Use large buttons and readable text.
- Keep question flow straightforward.
- Show clear feedback for correct and wrong answers.
- Avoid clutter.

## Code style
- Use clear function names.
- Keep functions small.
- Add comments only where helpful.
- Avoid deeply nested logic.
- Prefer constants for reusable text and configuration.
- Keep translation strings centralized.
- Do not duplicate logic when a shared function can be used simply.

## Data rules
- Country quiz data should be easy to edit.
- Use a simple array of objects for country, capital, and currency.
- If more countries are added, keep the format consistent.
- Do not fetch remote APIs unless explicitly requested.
- Keep the app fully usable offline if possible.

## Performance rules
- Keep the app lightweight.
- Avoid heavy animations.
- Avoid large dependencies.
- Keep startup fast on mobile devices.

## Testing and verification
After making changes, verify:
1. The app opens directly in browser from `index.html`
2. English language works
3. German language works
4. Quiz mode selection works
5. Score updates correctly
6. Next question flow works
7. Result screen works
8. Restart works
9. Layout works on narrow mobile width
10. Language switch works on iPhone-compatible behavior

## Change guidelines
When implementing a change:
- preserve simplicity
- preserve bilingual support
- preserve mobile compatibility
- do not rewrite the whole app unnecessarily
- make the smallest clean change that solves the problem

## Preferred enhancements
Safe enhancements:
- flags
- sound for correct/wrong answers
- difficulty levels
- more countries
- categories by continent
- PWA support
- installable mobile web app support

## Avoid unless requested
- backend
- login/auth
- database
- multiplayer
- admin dashboard
- analytics
- third-party UI frameworks
- TypeScript migration
- complex state management

## Output expectations for Codex
When changing code:
- explain briefly what changed
- keep edits minimal
- preserve existing functionality
- mention any mobile/browser-specific fixes
- mention if translations were added or updated