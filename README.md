# DuitSense

DuitSense is an AI-powered personal finance and money habit app built with Expo and React Native. It helps users understand their spending, set smarter savings goals, track budget progress, and build healthier financial habits through gamified challenges, projections, and learning content.

The app combines budgeting, financial education, and habit-building into one experience, with features such as:

- Smart expense tracking and monthly spending summaries
- AI-driven financial insights and recommendations
- Daily quiz and knowledge feed for financial literacy
- Savings projection and future planning tools
- Challenges, streaks, rewards, and leaderboard mechanics
- Wrapped-style summary experience for progress reflection

## Why DuitSense?

Many people know they should save more and spend more intentionally, but they lack a simple, motivating system that turns financial decisions into habits. DuitSense bridges that gap by making personal finance more engaging, visual, and rewarding.

## Key Features

### Personal finance dashboard
- Monthly spending overview
- Budget pacing visualization
- AI insight cards with suggestions
- Quick access to spending history and expense logging

### Smart planning
- Future projection view for savings growth
- Adjustable target age and monthly savings boost
- Comparison between current trajectory and improved trajectory

### Financial learning
- Daily quizzes
- Knowledge feed with practical budgeting and money tips
- Educational content tailored to financial literacy

### Gamification
- XP and streak tracking
- Challenges and achievements
- Spin-wheel rewards and leaderboard progression
- Progress summaries through wrapped screens

### App flow
- Onboarding experience for first-time users
- Quiz-based personalization
- Settings and account preference management
- Modal views for history, wrapped, and expense entry

## Tech Stack

- React Native
- Expo
- Expo Router
- TypeScript
- React Native Reanimated
- Expo Linear Gradient
- React Native Chart Kit
- Native UI components via React Native and Lucide icons

## Project Structure

```text
DUITSENSE/
├── app/
│   ├── (tabs)/
│   │   ├── _layout.tsx
│   │   ├── challenges.tsx
│   │   ├── index.tsx
│   │   ├── insights.tsx
│   │   ├── leaderboard.tsx
│   │   └── projection.tsx
│   ├── components/
│   ├── _layout.tsx
│   ├── XPContext.tsx
│   ├── daily-quiz.tsx
│   ├── expense-logger.tsx
│   ├── history.tsx
│   ├── index.tsx
│   ├── onboarding.tsx
│   ├── quiz.tsx
│   ├── result.tsx
│   ├── settings.tsx
│   ├── spin.tsx
│   └── wrapped.tsx
├── backend/
│   ├── epf_calculator.js
│   ├── index.js
│   ├── projection_engine.js
│   ├── reward_manager.js
│   ├── roi_calculator.js
│   ├── simulation_utils.js
│   ├── spin_wheel_engine.js
│   ├── squad_achievement_system.js
│   └── streak_system.js
├── constants/
├── hooks/
├── scripts/
├── assets/
├── .gitignore
├── app.json
├── eslint.config.js
├── package.json
├── package-lock.json
├── tsconfig.json
├── README.md
└── global.css
```

## Backend Overview

The `backend/` folder contains financial simulation and gamification logic used to power the app experience:

- `projection_engine.js` and `epf_calculator.js` handle future value and savings projection logic
- `roi_calculator.js` evaluates return on investment assumptions
- `simulation_utils.js` supports scenario modeling and micro-adjustment simulations
- `spin_wheel_engine.js` and `reward_manager.js` drive rewards and reward distribution
- `streak_system.js` manages streak calculations and XP rewards
- `squad_achievement_system.js` handles challenge and achievement progression

## Getting Started

### Prerequisites

- Node.js 18 or newer
- npm or yarn
- Expo CLI
- Android Studio / Xcode for device emulation (optional)

### Install dependencies

```bash
npm install
```

### Start the app

```bash
npx expo start
```

You can then run the app in:

- Android emulator
- iOS simulator
- Expo Go app
- Web preview

### Useful scripts

```bash
npm run android
npm run ios
npm run web
npm run lint
```

## Development Notes

This project uses Expo Router file-based navigation and a custom layout system built around `app/`. The root layout wraps the app in an `XPProvider`, enabling shared game-state and financial progression context.

The project structure is designed so that visuals and interactive flows live in `app/`, while simulation and reward logic lives under `backend/`.

## Roadmap / Potential Enhancements

- Persistent user data and backend sync
- Real bank or transaction API integrations
- Personalized AI recommendations based on actual spending patterns
- Multi-user or family finance tracking
- Push notifications and reminders for savings goals
- Localization and region-specific financial advice

## License

This project currently has no explicit license configuration in the repository.

## Contributing

Contributions are welcome. To contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run lint checks and validate the app locally
5. Submit a pull request with a clear summary of the change

## Contact

Repository: https://github.com/qianyi-11/DUITSENSE

This README was tailored to the current project structure and feature set in the repository.
