# ADR-001: Choose App Type (Native, Web, or Hybrid)

- **Status**: Accepted
- **Date**: 2024-10-20
- **Deciders**: Chinedu Amaechi, Natalia Hassan
- **Tags**: App Type, React Native, Cross-platform

## Context
The retail mobile app must be available on both iOS and Android, providing a feature-rich, responsive interface with capabilities like offline mode, real-time syncing, and secure transactions. A cross-platform solution that balances development efficiency with a near-native experience is essential.

## Decision
We decided to develop a **hybrid app using React Native**. This framework allows us to maintain a single codebase for both platforms, reducing development and maintenance costs while ensuring a responsive user experience.

## Rationale
- **Efficiency**: React Native enables cross-platform development, allowing code reuse across iOS and Android.
- **User Experience**: Provides a near-native experience, supporting features like real-time syncing and smooth interactions.
- **Flexibility**: React Native’s native module support allows for device-specific optimizations, enhancing scalability as the app grows.

## Consequences
- **Positive**: The single codebase reduces both initial development time and ongoing maintenance effort. Updates and improvements can be deployed across platforms simultaneously.
- **Negative**: For certain device-specific functionalities, performance may require native code integration, adding some complexity in specific cases.

## Links
- [React Native Documentation](https://reactnative.dev/docs/getting-started)

