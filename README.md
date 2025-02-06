# Expo Linking.getInitialURL() Intermittent Null Return

This repository demonstrates a bug where Expo's `Linking.getInitialURL()` method inconsistently returns `null`, disrupting deep link handling. The issue is intermittent and its cause is not fully understood but may be related to timing, Expo client version, or platform inconsistencies.

## Reproduction

1. Clone the repository.
2. Run `npm install`.
3. Run the app on either Android or iOS.
4. Attempt to open the app via a deep link.  Observe that sometimes the deep link is handled correctly, and sometimes `Linking.getInitialURL()` returns null, resulting in no action.

## Potential Solutions (See bugSolution.js)

The provided solution explores different approaches to address the issue, including asynchronous handling and retries.