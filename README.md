# React Native FlatList KeyExtractor Error: Duplicate Keys

This repository demonstrates a common error in React Native's `FlatList` component: using an incorrect `keyExtractor` function that results in duplicate keys. This can lead to unexpected behavior and crashes.

## The Problem

The `keyExtractor` function in `FlatList` is crucial for efficient rendering and updating.  It must provide a unique key for every item in the data array. If duplicate keys are used, React Native can't accurately track changes, causing issues like incorrect rendering or crashes.

## Reproduction Steps

1. Clone this repository.
2. Run `npm install`.
3. Run the app (e.g., `npx react-native run-android` or `npx react-native run-ios`).
4. Observe the errors or unexpected behavior in the application.

## Solution

The solution involves implementing a correct `keyExtractor` function that ensures uniqueness for each item. The solution file (`bugSolution.js`) demonstrates the correct implementation using the item's unique ID.