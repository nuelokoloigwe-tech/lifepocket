# LifePocket — Technical Architecture

## Prototype stack
- React 18 + TypeScript
- Vite
- Lucide icons
- CSS design system (Tailwind can be introduced as component coverage expands)
- Browser localStorage for prototype-only persistence

## Target production architecture
- Frontend: React + TypeScript, Vite, responsive PWA.
- Identity: Supabase Auth.
- Data: Supabase PostgreSQL.
- Authorisation: Row Level Security on every user-owned table.
- Scheduled reminders: trusted server-side scheduler/edge function; never rely on a browser tab being open.
- Delivery: email first, then opt-in web push; notification preferences and quiet hours required.
- Hosting: Vercel for frontend; Supabase for backend services.

## Proposed data entities
- profiles: user preferences, locale, timezone.
- commitments: title, category, amount, currency, due date, recurrence rule, status, owner_id.
- tasks: title, category, due date (optional), status, owner_id.
- notification_preferences: channel, lead time, quiet hours, owner_id.
- notification_events: commitment reference, scheduled_at, sent_at, delivery status, owner_id.

## Security and privacy requirements
- Enforce per-user access with database Row Level Security.
- Do not store bank credentials or payment card details.
- Do not process or retain uploaded identity, tenancy or mortgage documents until secure storage, encryption, malware scanning, retention and deletion controls are designed.
- Keep secrets server-side; never expose service-role keys in the browser.
- Provide account export and deletion pathways before public launch.

## Important boundary
The current prototype is not a production financial product. It uses illustrative sample records and local browser storage. It does not send notifications, connect to banks, or provide regulated financial advice.
