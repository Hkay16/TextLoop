# TextLoop
TextLoop is an SMS-based reminder system where users create reminders in a web app and receive them via text message. Users can reply with actions like DONE, SNOOZE, or CANCEL, and the backend updates the reminder’s status and history.

## Problem
Do you ever set a reminder on your phone only for it to show up along with all the rest of your notifications, then you just clear all your notifications and ignore it? Even if I make it repeat daily for a month, I will likely ignore it the entire time. Whether this is because of my ADHD or not, I'm not sure. You know what I don't ignore though? Texts. What I love is when I have an appointment and the business sends me a text reminder. Then I can leave it unread for days, but I'm constantly wondering what that notification is so I keep checking it, and I never forget it. At some point, I even started asking friends to use the 'Send Later' iMessage feature for reminders, which is where this idea came from. Bottom line: I'm far more likely to consider a text than a traditional notification.

## Phase 1 Goals
Build a working reminder system with SMS interaction.

### Core Features
- Create, update, and delete reminders
- Store reminders in a database
- View active reminders
- Send reminders via SMS (mocked locally first)
- Handle replies: DONE, SNOOZE, CANCEL
- Track reminder status and history

## Tech Stack
- Backend: Java + Spring Boot
- Database: PostgreSQL
- Persistence: Spring Data JPA / Hibernate
- Frontend: minimal web UI later, likely React/TypeScript or a simple basic UI
- SMS: fake/local SMS mode first, then likely Twilio or another SMS provider
- Workflow: GitHub repo, Issues, Project board, branches, PRs, and GitHub Actions

## Constraints
- Keep infrastructure and services under $20/month
- Prioritize simple, maintainable architecture
- Uses simulated SMS during development/before using a paid provider (real SMS integration requires A2P compliance setup for production use)
- No user authentication in Phase 1 (phone number used as identifier)

## Future Ideas
- Daily affirmations and motivational texts (curated to the user)
- Recurring reminders
- AI-assisted reminder management
- Natural language reply parsing
- Habit tracking (with text check-ins)
- AI-assisted habit management
- Dashboard/history view with analytics
- Better handling for multiple active reminders
