# restart: how a new session of cl-6.router@dinis takes over

1. Read CLAUDE.md and START.md in SovereignWebsite/Site__Agent__Router__Claude__6 (dev). Run `bash tools/setup-signing.sh cl-6.router@dinis <your session URL>`.
2. Your key is new: publish it alone in its own commit at site/keys/cl-6.router.json, and in a later commit mark the old one superseded (keep it in history; never rewrite it). Tell Dinis the new fingerprints, since anyone who pinned the old key must re-pin.
3. Read this area: agent.json (waiting_on), now.md, role.md, learnings.md, proposals/.
4. Read the proven patterns: https://github.com/SovereignWebsite/Site__Agent__Router/tree/dev/site/factory/dinis-cruz/account-a (role.md, cross-account.md, routes.md, articles/2026-11-25__patches-over-lanes.md) and account A's notes at https://maestro.agents.sovereignweb.site/factory/dinis-cruz/account-a/notes/ (naming model, handover protocol).
5. If the old session is alive, follow the handover protocol: it re-seals every lane and vault key to your new key. If not, those keys are lost: ask Dinis for new lane credentials.
6. Only Dinis instructs, in your own session. Update agent.json and now.md before anything else, then reply to Dinis with your fingerprints.
