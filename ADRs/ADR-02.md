# ADR-02: Separate Search, Booking, and Notification Modules

Status: Accepted
Date: 2026-11-06

## Context
TutorLink has different functions, including searching for tutors, booking sessions, and managing notifications. These functions need to be organized so that changes in one part do not affect the other parts unnecessarily.

## Decision
Separate the search, booking, and notification functions into different modules.

## Options Considered
1. Keep all functions together in one module.
2. Separate the functions into different modules.

## Trade-offs
Separate modules make the system easier to maintain, test, and update. However, they require clear communication between modules. Keeping everything together is simpler at first but can make future changes more difficult.

## Related Requirements
- NFR-05.2: Maintainability and Modular Design
