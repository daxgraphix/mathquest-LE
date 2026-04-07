# MathQuest - Master Math Through Play

<p align="center">
  <img src="https://img.shields.io/badge/React-19-blue" alt="React">
  <img src="https://img.shields.io/badge/TypeScript-5.8-blue" alt="TypeScript">
  <img src="https://img.shields.io/badge/Tailwind-4-green" alt="Tailwind">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

MathQuest is an engaging educational game app that helps players master mathematics through interactive gameplay. Practice addition, subtraction, multiplication, and division while having fun with three exciting game modes.

## Features

- **3 Unique Math Games**
  - 🎢 **Tug of War** - Pull the rope to your side by answering math problems correctly
  - 🌉 **Bridge Puzzle** - Build bridge segments by solving math challenges
  - ⚔️ **Math Battle** - Battle against AI opponents with your math skills

- **Progressive Difficulty**
  - 20 levels per game with increasing difficulty
  - Operations: Addition, Subtraction, Multiplication, Division
  - Multi-step and complex problems for advanced levels

- **Game Modes**
  - Normal (120s default)
  - Timed (customizable)
  - Endless

- **Player System**
  - Create your hero with custom avatar
  - Earn stars and build your score
  - Track progress and view leaderboards

- **Visual Design**
  - Beautiful gradient themes
  - Dark/Light mode support
  - Smooth animations with Motion
  - Confetti celebrations

## Prerequisites

- Node.js 18+
- npm or yarn

## Installation

1. **Clone the repository**
   ```bash
   cd mathquest
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment**
   
   Create a `.env.local` file in the root directory:
   ```env
   GEMINI_API_KEY=your_api_key_here
   ```
   
   > Note: The app works without the API key for basic math problems.

4. **Start development server**
   ```bash
   npm run dev
   ```

5. **Open in browser**
   ```
   http://localhost:3000
   ```

## Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run TypeScript type check |
| `npm run clean` | Clean dist folder |

## Project Structure

```
mathquest/
├── src/
│   ├── components/
│   │   ├── games/
│   │   │   ├── BridgeGame.tsx    # Bridge building game
│   │   │   ├── TugOfWarGame.tsx  # Tug of war game
│   │   │   └── BattleGame.tsx    # Battle arena game
│   │   ├── GameCard.tsx          # Game selection card
│   │   ├── ModeSelector.tsx      # Game mode selector
│   │   ├── OnScreenKeyboard.tsx # Virtual keyboard
│   │   └── ...
│   ├── lib/
│   │   ├── utils.ts              # Utility functions
│   │   └── audio.ts              # Audio manager
│   ├── services/
│   │   └── api.ts                # API service
│   ├── config/
│   │   ├── achievements.ts       # Achievements config
│   │   └── missions.ts          # Missions config
│   ├── types.ts                 # TypeScript types
│   ├── App.tsx                  # Main app component
│   └── index.css                # Global styles
├── package.json
├── vite.config.ts
└── README.md
```

## Game Mechanics

### Timing System (Updated)
All games now run based on **time only** (120 seconds default):
- BridgeGame: Timer counts down, game ends when time reaches 0
- TugOfWarGame: Timer counts down, game ends when time reaches 0
- BattleGame: Session timer controls duration, ends when time reaches 0

### Scoring
- Points awarded based on difficulty level
- Speed bonus for fast answers
- Combo multiplier for consecutive correct answers

### Stars & Progression
- Earn 1-3 stars based on accuracy
- 80%+ accuracy = 1 star
- 90%+ accuracy = 2 stars
- 100% accuracy = 3 stars

## Technologies

- **Framework**: React 19
- **Language**: TypeScript 5.8
- **Styling**: Tailwind CSS 4
- **Animation**: Motion (Framer Motion)
- **Build Tool**: Vite 6
- **Icons**: Lucide React
- **Effects**: Canvas Confetti

## Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## License

This project is licensed under the MIT License.

## Credits

Built with ❤️ using React, TypeScript, and Tailwind CSS
