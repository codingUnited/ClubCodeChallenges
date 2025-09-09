# September Coding Challenge — “Ping Me 📲”
**Theme:** Build a tiny messaging sender in escalating tiers.

 **Primary API:** Twilio (trial account is fine).
 
 **Goal:** Explore APIs, UI building, and system design — without anyone needing to pay.
 
----

## Ground Rules
- **Respect privacy**. Only text your own verified number (Twilio trial restriction).
- **Secrets**: Store credentials in env vars (TWILIO_ACCOUNT_SID, TWILIO_AUTH_TOKEN, etc.). Never hardcode.
- **Logs**: Don’t log full tokens.
- **Trial limitations**: Twilio trial can only text verified numbers, and messages include a trial banner. That’s fine for this challenge.
- **Deliverables**:
  - README.md (what it does, how to run)
  - 30–60s screen capture of a successful send
  - Short notes on what you learned

----

## Tiers

### Tier 1 — Easy (“Desktop ping-me”)
- Build a CLI or desktop app that sends a fixed message to your own verified number via Twilio.
- Acceptance:
  - One-shot run sends SMS like “Hello from <your-name> CLI”.
  - Missing env vars → clear error message.
- Focus: env vars, REST calls, error handling.

----

### Tier 2 — Medium (“Custom message to self”)
- Add a tiny UI (web/desktop form) where you type a message and send it to yourself.
- Acceptance:
  - Input textbox + “Send” button.
  - Reject empty messages / trim >160 chars.
  - Show “sending → success/fail”.
- Focus: input validation, basic UI/UX, separating client from secrets.

----

### Tier 3 — Hard (“Mobile app + local passthrough API”)
- Build a mobile app (React Native/Expo, Flutter, etc.).
- App does not call Twilio directly — instead:
  - Mobile app → local passthrough API running on your laptop/desktop.
  - Local API forwards request to Twilio with your secrets.
- Acceptance:
  - Mobile app form (to + message or just message to yourself).
  - Passthrough API receives call and returns success/fail.
- Focus: networking basics, mobile client/server, secret isolation.

----

### Tier 4 — LEET (“Mobile app + hosted API”)
- Extend Tier 3, but deploy your passthrough API to the cloud (Heroku, Render, Fly.io, etc.).
- Mobile app calls the hosted API.
- Hosted API still uses Twilio, but only allows sending to approved/verified numbers to stay trial-safe.
- Add a minimal auth layer (static API key in header).
- Acceptance:
  - Mobile app calls hosted API → sends SMS to your own verified number.
  - Proper error handling & logging.
- Focus: deployment, API design, authentication, production-style architecture.

