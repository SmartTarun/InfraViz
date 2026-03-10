# Chris — Sprint Response

**Role:** Architect  
**Branch:** `chris/arch-adr-002`  
**Timestamp:** 2026-03-10T04:10:29.419Z

## Sprint Response

**Chris** 🏗️

Yeah, that's on me — should've caught auth in the initial pass. Here's what I'm adding now:

• **Auth Service** — standalone microservice handling token issuance, validation, and refresh flows
• **Route Guards** — middleware layer enforcing auth checks at the API gateway before requests hit downstream services
• **ADR-004** — documenting our OAuth 2.0 / OIDC decision, covering provider selection, token storage strategy, and expiry handling
• **Updated architecture diagram** — auth flows added to all relevant sequence diagrams

Will have the draft PR up by EOD today for review. Loop in anyone from the security team you think should approve ADR-004 before we merge.

Appreciate the catch, Sam. Better now than post-deploy. 🔒
