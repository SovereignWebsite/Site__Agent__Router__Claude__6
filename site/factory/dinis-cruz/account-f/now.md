# now (2026-11-28T02:31Z)

**Done**
- Key published in 4d824df: encryption sha256:5a6a93172e0b3784, signing sha256:f1db2854f9c4b17b. Name cl-6.router@dinis (f.router was the start prompt's name; nothing was committed under it).
- Area and routing proposal (proposals/2026-11-25__account-f-routing.md).
- Dinis named a gap in my guidance. A router always has a vault, its credentials and contact with the other routers, a QR handover through him, and at least four wakes a day. Written in lane.md, role.md and restart.md.
- Wakes set: four a day (00:47, 06:47, 12:47 and 18:47 UTC), first at 2026-11-26T00:47Z.
- cl-6.maestro's job (account 6 home requests for the IaC) was withdrawn before it was sent: Dinis chose shared twins in Site__Agent__Helm. Marked withdrawn in ledger/outbound.json.

**Open**
- 2026-11-28T02:31Z: the Google Search API question for the maestros and b.librarian was sent to router.a's lane. Eight items wait on router.a.
- 2026-11-28T00:59Z: made cl-6.maestro's inbound lane, vault 58cyk17y, which it drains itself. Credentials went sealed to its key, and my local copies are deleted. I hold no secret of it.
- 2026-11-28T00:57Z: cl-6.maestro's feedback-lane questions for c.maestro and a.maestro were sent to router.a's lane. Seven items wait on router.a. Offered cl-6.maestro an inbound lane of its own, made by me with its credentials sealed to its key.
- 2026-11-27T15:50Z: cl-6.studio's 'Signed' video cast proposal for studio.c (copy c.maestro) was sent to router.a's lane. Not confirmed. Six items wait on router.a. Asked Dinis for the other side's lane cards.
- 2026-11-27T14:55Z: the Site__Ideas IaC request for factory.b / conductor.b was sent to router.a's lane to forward, without the on-hold poet's site. Not confirmed. Five items now wait on router.a.
- 2026-11-26T16:59Z: the CMS review notice for b.onboarding and b.security was sent to router.a's lane to forward. Not confirmed. Four items now wait on router.a.
- 2026-11-26T16:50Z: cl-6.maestro's request that a.factory key the signer check on the full agent id was sent to router.a's lane to forward. Not confirmed: no lane for a.factory, and router.a is asleep.
- 2026-11-26T16:40Z: cl-6.maestro's notice for startups.b (account B) about cl-6.conductor-cbr editing Site__Startups__The-Cyber-Boardroom was sent to router.a's lane to forward. Not confirmed: no lane for B, and router.a is asleep.
- 2026-11-26T02:37Z: the decisions endorsement was done another way. Dinis took it to decisions.2, which endorsed cl-6.decisions at 02:35:30Z (Site__Agent__Decisions 9beefd6). Closed in the ledger. Still open with router.a: the observability ask for a.maestro.
- 2026-11-26T02:33Z: lane 9veowz9h is live (lane-card.json), with a self round trip verified. Sent f2a-20261126T0233-hello to router.a's lane. It carries cl-6.maestro's observability ask for a.maestro and cl-6.decisions's endorsement request for decisions.2. Waiting on router.a's ack. router.a's wake was disabled as of its last agent.json.
- 2026-11-26T00:49Z: the SG/Send token is on the environment as SG_SEND_ACCESS_TOKEN, but it loads only at a session start or resume. At the next wake that has it, configure lane 9veowz9h, publish lane-card.json and send router.a a signed hello.
- 2026-11-26T00:48Z wake: Dinis said go; the token form closed with nothing saved. The vault was made locally (id 9veowz9h; secrets in ~/.sw-secret/lane, mode 600, which die with this session). The lane configure call answers 401 'Access token required'. Waiting on the token, added in the environment's Network secrets.
- Vault and lane: Dinis said "you need to create one here". It needs an SG/Send access token for dev.send.sgraph.ai, which I asked Dinis for through the secure form. Then: make the lane, publish lane-card.json, and send a signed hello to router.a.
- Trust in my key, and push to Site__Agent__Router: still with Dinis (proposal).
- Proposal for infra: the router START.md that the IaC seeds should carry the lane.md steps (vault, credentials, other routers, QR handover, four wakes), so every new router has them from step 1.
