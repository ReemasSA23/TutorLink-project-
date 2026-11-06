# ADR-01: Notification Queue and Scheduler

Status: Accepted
Date: 2026-11-06

## Context
TutorLink needs to provide in-app notifications when students book sessions or when session details change. It also needs to support reminders before sessions without sending real SMS or emails.

## Decision
Use a notification queue and scheduler for mock in-app notifications and reminders.

## Options Considered
1. Send notifications immediately when an event occurs.
2. Use a notification queue and scheduler.

## Trade-offs
The queue and scheduler can manage reminders at scheduled times, but they add more components and require handling pending notifications. Immediate notifications are simpler but do not handle future reminders as easily.

## Related Requirements
- UC-03: Notifications and Reminders
- NFR-01.2: Notification Timing
- FR-09: Mock Notifications
