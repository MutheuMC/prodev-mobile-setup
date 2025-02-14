# Mobile Development with React Native, NativeWindCSS, and Expo

## Introduction
This project is built using **React Native**, **NativeWindCSS**, and **Expo**, providing a modern, efficient workflow for mobile app development. It leverages Expo for seamless testing and deployment, while NativeWindCSS brings utility-first styling inspired by Tailwind CSS.

## Technologies Used
- **React Native** – Framework for building mobile applications using JavaScript and React.
- **NativeWindCSS** – A Tailwind CSS-inspired styling solution for React Native.
- **Expo** – A powerful toolset for developing, testing, and deploying React Native applications.

## Prerequisites
Before setting up the project, ensure you have the following installed:
- **Node.js LTS**: [Download](https://nodejs.org/)
- **Expo CLI**: Install via `npm install -g expo-cli`
- **VS Code** (or any code editor)
- **Expo Go App** (for testing on a physical device)
  - [Google Play Store](https://play.google.com/store/apps/details?id=host.exp.exponent) (Android)
  - [Apple App Store](https://apps.apple.com/app/expo-go/id982107779) (iOS)

## Setup Instructions

1. **Create a New React Native Project with Expo**
   ```sh
   npx create-expo-app my-app
   cd my-app


Install NativeWindCSS and Dependencies

sh
Copy
Edit
npm install nativewind tailwindcss
Configure TailwindCSS

Create a tailwind.config.js file in your project root:
js
Copy
Edit
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./App.{js,jsx,ts,tsx}", "./components/**/*.{js,jsx,ts,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
Create a babel.config.js file if not already present, and update it:
js
Copy
Edit
module.exports = {
  presets: ['babel-preset-expo'],
  plugins: ['nativewind/babel'],
};
Run the Application

sh
Copy
Edit
npx expo start
Scan the QR code using the Expo Go app on your physical device to test the app.
Project Structure
bash
Copy
Edit
/my-app
 ├── /assets         # Static assets (images, icons)
 ├── /components     # Reusable React Native components
 ├── /screens        # Screen components for navigation
 ├── App.js          # Main entry point
 ├── tailwind.config.js  # Tailwind CSS configuration
 ├── babel.config.js     # Babel configuration for NativeWindCSS
 ├── package.json    # Dependencies and project metadata
