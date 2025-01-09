# Expo Go: Custom Native Module Loading Issue

This repository demonstrates a bug where Expo Go fails to load an app that utilizes a custom native module.  The issue arises because Expo Go doesn't include the native modules from your project.

## Problem

When running an Expo project containing a custom native module within Expo Go, the app crashes, displaying an error indicating that the native module cannot be found.  This prevents the application from functioning correctly within the Expo Go environment.

## Solution

The primary solution is to avoid relying on custom native modules when developing apps intended to run within Expo Go.  Expo Go is designed for rapid prototyping and testing using JavaScript-only components. For production-ready applications that require native module functionality, a standalone app build is necessary, bypassing the limitations of Expo Go.

This repository includes example code illustrating the issue and a corrected approach focusing on JavaScript-only solutions or utilizing a standalone build for production deployments.