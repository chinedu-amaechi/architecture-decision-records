# ADR-005: Data Storage

- **Status**: Accepted
- **Date**: 2024-11-05
- **Deciders**: Chinedu Amaechi, Nikita Sharma, Faruq Ogunkunle
- **Tags**: Offline Storage, Cloud Sync, Data Management

## Context
The app needs offline access to the product catalog and order history, as well as secure, scalable cloud storage for customer data. Data syncing is required to update local data when the user reconnects to the internet.

## Decision
We chose **SQLite** for local storage to support offline access, and **Firebase Firestore** for cloud storage to ensure scalability and real-time syncing.

## Rationale
- **Offline Functionality**: SQLite allows offline access to key data, ensuring usability without connectivity.
- **Real-Time Syncing**: Firebase Firestore provides scalable, real-time syncing, enabling smooth transitions between offline and online states.

## Consequences
- **Positive**: Provides both offline functionality and real-time syncing, enhancing user experience.
- **Negative**: Handling offline and online data conflicts adds complexity, requiring additional code to manage synchronization effectively.

## Links
- [SQLite Documentation](https://www.sqlite.org/docs.html)
- [Firebase Firestore Documentation](https://firebase.google.com/docs/firestore)

