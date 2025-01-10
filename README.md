# Expo CLI Android Build Failure: Gradle/AGP Version Mismatch

This repository demonstrates a common but elusive bug encountered when building Android apps with the Expo CLI. The issue stems from inconsistencies between the Gradle and Android Gradle Plugin (AGP) versions, leading to cryptic build errors.  Even standard troubleshooting steps like cleaning the build cache often fail to resolve the problem.

The `bug.js` file shows a sample Expo project exhibiting this issue.  The `bugSolution.js` file provides a potential solution involving a complete project rebuild and verification of Gradle/AGP compatibility.

## Reproducing the Bug

1. Clone this repository.
2. Navigate to the project directory.
3. Attempt to build the Android app using `expo build:android`. 
4. Observe the unclear error messages.

## Solution

The most reliable solution involves performing a full project rebuild.  Sometimes, simply deleting the `android` folder within the project isn't sufficient.  A complete re-generation from scratch is necessary to ensure Gradle/AGP version alignment.

Refer to the `bugSolution.js` for implementation details. Please note that in some cases, manually adjusting Gradle/AGP versions within the project's `gradle` files may be required but is not guaranteed to solve the problem.   Ensure compatibility with current Expo version.