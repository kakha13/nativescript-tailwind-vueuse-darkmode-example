# Nativescript Tailwind 4 Dark Mode Switch With @nativescript-use example

## Project Overview

This repository demonstrates the integration of Tailwind CSS 4 with NativeScript, featuring a dynamic dark mode implementation using the @nativescript-use utility library. The project showcases how to build cross-platform mobile applications with modern, utility-first CSS styling while supporting theme switching capabilities.

## Features

- **Tailwind CSS 4 Integration**: Utilizes the latest version of Tailwind CSS for styling NativeScript components
- **Dynamic Dark Mode**: Implements a theme switching mechanism between light and dark modes
- **@nativescript-use Library**: Leverages the Vue Composition API-inspired utilities for NativeScript
- **Cross-Platform Support**: Works on both iOS and Android platforms

## Setup Instructions

1. Clone this repository
2. Install dependencies:
   ```
   npm install
   ```
3. Run the application:
   ```
   ns run android
   ```
   or
   ```
   ns run ios
   ```

## Dark Mode Implementation

The project demonstrates how to:
- Configure Tailwind CSS for dark mode support
- Use the `dark:` variant prefix to apply dark mode specific styles
- Implement a theme toggle using reactive state management
- Persist user theme preferences

## Issues Fixed

- When applying dark mode classes (like `dark:text-red-400`) to certain elements, styles may unexpectedly affect other elements
- Some theme transitions might not be smooth on specific devices

## Resources

- [NativeScript Documentation](https://docs.nativescript.org/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [@nativescript-use GitHub](https://github.com/NativeScript-Use/NativeScript-Use)
