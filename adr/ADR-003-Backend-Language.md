# ADR-003: Backend Language

- **Status**: Accepted
- **Date**: 2024-11-04
- **Deciders**: Chinedu Amaechi, Nikita Sharma, Faruq Ogukunle
- **Tags**: Backend, Node.js, Express.js, Real-time

## Context
The backend needs to support secure and responsive API management, handle concurrent requests, and ensure data integrity for real-time updates, data syncing, and secure transactions.

## Decision
Node.js with Express.js was chosen as the backend stack. Node.js’s asynchronous, event-driven architecture suits real-time interactions, while Express.js provides a minimalistic, flexible framework for rapid API development.

## Rationale
- **Real-Time Processing**: Node.js’s non-blocking nature allows it to handle concurrent requests, crucial for an app with real-time data requirements.
- **Compatibility**: Node.js is compatible with JavaScript, aligning well with React Native on the front end and simplifying development.

## Consequences
- **Positive**: Streamlined development process and robust real-time support.
- **Negative**: Node.js may not perform as well with CPU-intensive tasks, so specific processes might require alternate solutions.

## Links
- [Node.js Documentation](https://nodejs.org/en/docs/)

