# ADR-004: Permissions Management

- **Status**: Proposed
- **Date**: 2024-11-05
- **Deciders**: Chinedu Amaechi, Nikita Sharma, Faruq Ogunkunle
- **Tags**: Permissions, Privacy, Security

## Context
The app requires permissions for features like notifications, offline storage, and potentially location-based features for location-based offers. Respecting user privacy and ensuring compliance with data protection laws is critical.

## Decision
We chose to implement minimal, on-demand permissions. Permissions will be requested only when the relevant feature is accessed, such as notifications for order updates or promotions.

## Rationale
- **User Privacy and Compliance**: Requesting only necessary permissions aligns with privacy regulations like GDPR and reduces user pushback against invasive prompts.
- **User Experience**: On-demand permissions enhance the user experience by limiting unnecessary prompts.

## Consequences
- **Positive**: Improves user trust and maintains compliance with privacy regulations.
- **Negative**: The need for conditional code to handle denied permissions may increase complexity in the codebase.

