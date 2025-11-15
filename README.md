# ProDev Mobile App

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)  
[![Expo](https://img.shields.io/badge/Powered%20by-Expo-4630EB.svg)](https://expo.dev/)  

---

## Table of Contents

- [About](#about)  
- [Features](#features)  
- [Architecture](#architecture)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Installation](#installation)  
  - [Running the App](#running-the-app)  
- [Usage](#usage)  
- [Navigation](#navigation)  
- [Folder Structure](#folder-structure)  
- [Environment Variables](#environment-variables)  
- [Testing](#testing)  
- [Contributing](#contributing)  
- [Roadmap](#roadmap)  
- [License](#license)  
- [Acknowledgments](#acknowledgments)  

---

## About

ProDev Mobile App is a cross-platform mobile application built with **React Native** and **Expo**, designed to help developers manage their professional growth. It leverages **Expo Router**, a file-based routing system inspired by Next.js, which enables navigation via a folder structure inside the `app/` directory.

---

## Features

- File-based routing using **Expo Router**  
- Modular screen architecture  
- (Add more as relevant)  
  - Authentication (login/signup)  
  - Profile management  
  - Task / milestone tracking  
  - Notifications  
  - Offline support (if applicable)  

---

## Architecture

- **Framework**: React Native + Expo  
- **Routing**: Expo Router  
- **Languages**: TypeScript / JavaScript  

---

## Getting Started

### Prerequisites

Make sure you have installed:

- Node.js (>= 14.x)  
- **Expo CLI**:  
  ```sh
  npm install -g expo-cli
    ```

* (Optional) Yarn
* Android Studio or Xcode (for simulators / emulators)
* Physical device (if you plan to run on phone)

### Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/SireTallest/prodev-mobile-app.git
   ```
2. Navigate into the project folder:

   ```sh
   cd prodev-mobile-app
   ```
3. Install dependencies:

   ```sh
   npm install
   # or
   yarn install
   ```

### Running the App

To start the development server:

```sh
expo start
```

This will launch Expo Dev Tools. From there, you can:

* Run on **Android** (emulator or device)
* Run on **iOS** (simulator or device)
* Open in **web browser**

---

## Usage

* After launching, users can **sign in** or **register**
* On successful login, navigate to dashboard
* Create and manage your professional goals
* Track progress and set reminders
* (Add screenshots or GIFs if you have them to make it visual)

---

## Navigation

```
app/
├── index.tsx             <- root / home screen  
├── login/
│   └── index.tsx         <- login screen  
├── profile/
│   └── [userId].tsx       <- dynamic profile screen  
└── tasks/
    ├── index.tsx         <- tasks list  
    └── [taskId].tsx       <- individual task detail  
```

---

## Folder Structure

```
/prodev-mobile-app
├── app/                  # Expo Router pages / screens  
├── assets/               # Images, icons, fonts  
├── components/           # Reusable UI components  
├── constants/            # App constants (e.g. colors, sizes)  
├── contexts/             # Context API providers (if any)  
├── hooks/                # Custom React hooks  
├── navigation/            # (Optional, if used)  
├── services/             # API services, local storage, etc.  
├── store/                 # State management (Redux / Zustand / etc.)  
├── utils/                 # Helper functions  
└── app.config.ts         # Expo config file  
```

---

## Environment Variables

1. Create a `.env` file in the root (if using `react-native-dotenv` or similar)
2. Add variables, for example:

   ```env
   API_URL=https://api.prodev.com
   FIREBASE_API_KEY=your_key_here
   ```
3. Make sure to add `.env` (or your config file) to `.gitignore` if it contains secrets.

---

## Testing

```sh
npm test
# or
yarn test
```
---

## Contributing

Contributions are **very welcome**! Here’s how to get started:

1. Fork the repository
2. Create a new branch:

   ```sh
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and commit:

   ```sh
   git commit -m "Add some feature"
   ```
4. Push to your branch:

   ```sh
   git push origin feature/your-feature-name
   ```
5. Open a Pull Request (PR) — describe your changes, why they’re needed, and how to test them.

**Guidelines:**

* Follow the existing code style
* Write tests for new features (if you have a testing framework)
* Make sure new code is documented (via comments or README updates)
* Be responsive to review feedback

---

## Roadmap

Here are some planned features and improvements:

* [ ] Authentication (OAuth, social login)
* [ ] Push notifications
* [ ] Profile picture upload
* [ ] Analytics / tracking user progress
* [ ] Dark mode
* [ ] Offline data sync

Feel free to suggest other features via Issues or Pull Requests!

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

* Thanks to **Expo** for making React Native development easier
* Inspired by **Next.js** folder-based routing, applied via **Expo Router**

---

## Contact

If you have any questions, feel free to reach out:

* **Author**: Oladepo Abdulbaki Opeyemi
* **GitHub**: [@SireTallest](https://github.com/SireTallest)
* **Email**: ([abdoladepo@gmail.com](mailto:a bdoladepo@gmail.com))

---