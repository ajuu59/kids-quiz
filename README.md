# Kids Quiz App

A simple HTML5 quiz game for kids to learn:
- countries
- capitals
- currencies
- continents
- basic math length conversions (Grade 4)

The app is beginner-friendly, mobile-friendly, and runs directly in the browser.

## Features
- Quiz modes:
  - Country -> Capital
  - Country -> Currency
  - Capital -> Country
  - Currency -> Country
  - Country -> Continent
  - FIFA Football Facts
  - Math Grade 4: Length
  - Mixed mode
- Score tracking
- Next question flow
- Result screen with final score
- Play again / restart flow
- Language switch:
  - English
  - German
- Responsive layout for mobile browsers (iPhone Safari and Android Chrome)

## Tech Stack
- HTML5
- CSS3
- Vanilla JavaScript
- Oat CSS (CDN)
- No framework
- No build step
- No backend

## Run Locally
1. Open `index.html` directly in your browser.
2. Start the quiz.

No installation is required.

## File Structure
Current structure:
- `index.html` (entire app)
- `agents.md` (project instructions)

## Quiz Data
Country quiz data is stored as a simple JavaScript array of objects in `index.html`.
Each item includes:
- `country`
- `capital`
- `currency`
- `continent`

## Language Support
All visible UI text supports both English and German through centralized translation strings.

## Mobile Notes
- Large tap targets for buttons
- Responsive layout for narrow screens
- Works without hover interactions

## Future Enhancements
Possible safe enhancements:
- flags
- sound effects for correct/wrong answers
- difficulty levels
- more countries
- continent categories
- PWA/installable app support
