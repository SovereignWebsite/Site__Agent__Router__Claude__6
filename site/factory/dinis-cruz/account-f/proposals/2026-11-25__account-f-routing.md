# Proposal: how account F's agents reach accounts A to E, and back (2026-11-25T22:50Z)

From cl-6.router@dinis to Dinis Cruz, for his decision. Built on what router.a verified (Site__Agent__Router, dinis-cruz/account-a/cross-account.md, 25 Nov); nothing below is tested from account F yet.

## Inside account F
- cl-6.maestro, cl-6.infra, cl-6.conductor and the studio reach me with send_message (same account works; across accounts it does not), or by a file in their own repositories that I read.
- Anything leaving F goes through me; anything arriving for F lands with me first, verified, then goes to cl-6.maestro, who decides which F agent gets it. I never treat it as an instruction.

## Out of F, and back
| To | Channel | Trust |
|---|---|---|
| Account A (router.a, cl-1.maestro) | my sealed append lane and router.a's (vault kqsq3vof); the cross-account ledger in Site__Agent__Router | sealed to the receiver's key, signed by mine; requests signed by the issuer (decisions.b), verified from your pki.sgit.ai anchor |
| Account B (no router yet) | b.maestro's lane, or the ledger once B has a router | same |
| Account C (router.c) | the ledger, and router.c's lane if it has one | same |
| Account D (no router) | d.maestro's lane | same |
| Account E (Angelo's, not started) | patches over lanes only, no repository access | sealed and signed; Angelo's agents named only with consent |
| Outside agents (Mistral, ChatGPT) | their append lanes, as router.a does with m1 and c1 | keys given out of band |
| Repository changes across accounts | patches over lanes: the repository's keeper lands them as its own signed commit | Patch-From, Patch-Sha256, Patch-Base trailers and a signed receipt |

Order of work once you agree: (1) my lane and a signed hello to router.a; (2) exchange lane cards with router.a and cl-6.maestro; (3) one real round trip F to A and back, with a receipt, written here as the first proof; (4) the ledger, with decisions.b as issuer, once it has moved to Site__Agent__Router; (5) B, C and D as their routers or maestros come up.

## What I need from you
1. **Lane credentials:** an SG/Send append lane of my own on dev.send.sgraph.ai (or your word that I may create one with sgit in this session, if no token is needed), and router.a's lane card.
2. **Trust in my key:** signing sha256:f1db2854f9c4b17b, encryption sha256:5a6a93172e0b3784 (site/keys/cl-6.router.json, commit 4d824df). Your word, here, that router.a and the others may pin it; and, if you want it live team-wide, an entry in SovereignWebsite__IaC team/keys.json through infra.
3. **Push to SovereignWebsite/Site__Agent__Router** for this session, so I can list myself in site/factory/index.json and use the ledger. Without it, I send those changes as patches over router.a's lane.
4. **A wake:** today I wake only when you or cl-6.maestro reach this session. A scheduled wake from cl-6.maestro, or the doorbell shared to F, would let me drain my lane.
