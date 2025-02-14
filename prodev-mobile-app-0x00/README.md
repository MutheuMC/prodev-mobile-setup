# Welcome to your Expo app 👋

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

## Steps for Scaffolding the Project

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
Observations from npx expo reset-project
Running npx expo reset-project resets the project by:

Clearing cached dependencies, builds, and configurations.
Removing and reinstalling node_modules, ensuring a clean dependency tree.
Resetting the Metro bundler cache, which can resolve issues related to stale builds.
Regenerating the package-lock.json file.
Notable Observations:
The reset process helped resolve issues related to stale dependencies.
After resetting, the first build was slower due to dependency reinstallation.
If additional configurations (e.g., TailwindCSS setup) were done manually, they remained intact after the reset.
If any files were accidentally deleted, the reset command did not restore them.



This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
    npx expo start
   ```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

## Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.
