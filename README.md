# Silent Crash with AsyncStorage in Expo

This repository demonstrates a common issue when working with AsyncStorage in Expo applications: silent crashes due to improper asynchronous operation handling.  The bug example shows how failing to await AsyncStorage operations can lead to unexpected app termination without informative error messages.

The solution provides a corrected version with proper error handling and `await` usage, preventing the silent crash and providing better debugging capabilities.

## How to reproduce the bug:

1. Clone this repository.
2. Run `npm install`.
3. Run the app using Expo Go or a similar tool.
4. Try to save some data. You will see the app crash without clear errors.

## Solution:

The solution involves correctly using `async/await` to handle the asynchronous nature of `AsyncStorage` and adding proper error handling.