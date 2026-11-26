# Mzansi-Pages — Product Blueprint

**Tagline:** Your People. Your World. Your Pages.  
**Brand direction:** Modern African technology  
**Primary market:** South Africa, with international potential  
**Initial audience policy:** 18+ for the first release

## Product purpose

Mzansi-Pages brings social networking, interest-based communities and professional connections into one platform. Dating is a separate, optional adults-only experience and must not be mixed into general discovery.

## Core product areas

1. **Home:** Social feed, posts, reactions, comments and sharing.
2. **Discover:** People, topics, communities and events.
3. **Communities:** Public/private groups, members, discussions and moderation.
4. **Connections:** Follow and connection relationships.
5. **Messages:** Private and group conversations.
6. **Dating & Relationships:** Separate 18+ experience, enabled only after reliable age assurance.
7. **Opportunities:** Projects, collaboration, learning and organisation listings.
8. **Notifications:** Account and community activity.
9. **Profile:** Personal identity, interests, posts, skills and optional portfolio.

## MVP scope

- Registration and secure authentication
- Date-of-birth eligibility check and age-assurance integration
- User profiles and privacy controls
- Create and view text posts
- Reactions and comments
- Follow/connection relationships
- Create and join communities
- Report, block and mute
- Basic moderation and admin tools

Messaging, video, advanced recommendations, opportunities marketplace and dating matching should follow only after the core product, privacy and safety systems are stable.

## Age and dating policy

- Initial release is designed for adults aged 18 and older.
- Date-of-birth entry is an eligibility check, not proof of age.
- Production access requires a suitable age-assurance method and server-side enforcement.
- Dating must be restricted to verified adults aged 18+.
- Dating profiles must be opt-in and separate from ordinary profiles.
- No minor accounts may access, view or be recommended into dating.
- Provide clear consent controls, blocking, reporting, moderation and privacy options.
- Do not collect or retain identity-document data unless strictly necessary and legally reviewed; prefer a provider that returns a verification result or token.

## Visual identity

- Midnight Navy: `#101D38`
- Electric Blue: `#3286E8`
- African Gold: `#E7B84B`
- Cloud White: `#F5F7FB`
- Violet: `#805AD5`

Use the geometric M monogram as the starting logo concept. Avoid visual clichés; use African inspiration through confident colour, thoughtful graphic details and inclusive photography rather than decorative stereotypes.

## Technical direction

- Web: Next.js + TypeScript
- Android: React Native + Expo
- Backend: Supabase
- Database: PostgreSQL
- Media: Supabase Storage
- Realtime: Supabase Realtime
- Deployment: Vercel for web; Expo EAS for Android builds

## Core data entities

- profiles
- connections
- posts
- post_media
- comments
- reactions
- communities
- community_members
- conversations
- messages
- notifications
- opportunities
- reports
- blocks
- age_verifications
- dating_profiles
- dating_preferences
- dating_interactions
- matches

## Security and privacy requirements

- Enforce authorization with server-side checks and PostgreSQL Row Level Security.
- Never trust client-side checks as the only access control.
- Keep private profile fields private by default.
- Add rate limits and anti-spam controls.
- Provide account deletion and data export workflows.
- Review POPIA obligations and other applicable laws before launch.
- Establish moderation escalation, appeals and incident response procedures.

## Success measures

- Weekly active users
- 7-day and 30-day retention
- Meaningful connections per active user
- Community participation
- Posts and comments per active user
- Report response time
- Abuse reports per 1,000 active users
- Registration completion and age-assurance failure rates

## Current implementation status

The repository's `index.html` is a front-end demonstration. It does not yet connect to a backend, persist user data or provide production account creation. Do not use it to collect real personal information.
