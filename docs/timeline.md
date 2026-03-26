## Timeline



### My Plan

| Phase | Dates | Focus |
|-------|-------|-------|
| Pre-Community Bonding | April 2 – April 27 | I am planning to work on my existing PRs |
| Community Bonding | April 28 – May 25 | Setup, open PRs, mentor discussions |
| Coding Phase 1 | May 26 – July 10 | Customizable Webhook Fields |
| Midterm Evaluation | July 13 – July 17 | Review & buffer |
| Coding Phase 2 | July 18 – Aug 16 | Stripe callbacks, Zapier, extensions |
| Final Week | Aug 17 – Aug 24 | Wrap up, final report |

---

### Pre-Community Bonding — April 2nd to April 27th
- This period i would like to dedicate to getting my existing PR to a good state (probably merged), so that they dont end up being stale. 
(#38599 Intercom, #38279 Jira comments, #38481 Azure Alert, # import slack) 


### Community Bonding — April 28th to May 25th

-I would like this period to be more of research and preperatory work for my GSOC project. Going through the documentation existing work in some completion candidate and even closed WIPs as there are many which i can use to learn about(#452,)
- And most importantly develop a better bond with my mentors  (Niloth and Lauryn).

### Coding Phase 1 — May 26th to July 10th

- **Week 1:** **Backend Permissions System** — Implement core decorator in `zerver/decorator.py` to enforce `INCOMING_WEBHOOK_BOT` restrictions on read endpoints. Add unit tests for compliance.
- **Week 2:** **OAuth Infrastructure Setup** — Integrate `django-oauth-toolkit`, configure scopes (`webhook:send`, `bot:read`, `bot:write`), and register OAuth endpoints locally.
- **Week 3:** **OAuth Token Authentication** — Extend API dispatcher in `zerver/lib/rest.py` to accept Bearer tokens alongside API keys, and enforce backend scope restrictions.
- **Week 4:** **OAuth Authorization Screen** — Build and style the consent screen matching Zulip's UI for users to approve webhook access.
- **Week 5:** **UI/UX Revamp (Backend + Button)** — Update `zerver/views/documentation.py` to pass the `user_can_create_webhook` flag. Conditionally render the "Add to Zulip" button on the integrations page.
- **Week 6:** **UI/UX Revamp (Frontend Modal)** — Build the stream picker modal (`add_to_zulip_modal.hbs`), wire it up to `POST /json/bots`, and route through the new OAuth flow. Fix emerging bugs and write initial docs.

### Midterm Evaluation — July 13th to July 17th
- Buffer for any carry-over from Phase 1.
- Deliver working Backend Permissions, OAuth flow, and the `/integrations` page revamp.
- Sync with mentors on priorities for Phase 2 (the webhook field customizations).

### Coding Phase 2 — July 18th to August 16th
- **Week 7:** **Custom Webhook Fields (Backend Core)** — Define `ISSUE_FIELDS_CONFIG` for Jira. Add `created_issue_fields` parameter and refactor `handle_created_issue_event`.
- **Week 8:** **Custom Fields (Advanced Resolution)** — Add custom dot-path field resolution logic (`project.name`, `customfield_*.name`). Fallback logic handling.
- **Week 9:** **Custom Fields (Frontend State)** — Hook up `WebhookUrlOption` with the `options` field, configure backend serialization and Zod schema updates.
- **Week 10:** **Pill-based UI** — Implement pill-based UI with typeahead (`integration_field_pill.ts`), and URL builder integration inside the URL generation modal.
- **Week 11:** **Extensibility & Docs** — Extend the pill UI framework to other integrations (e.g. GitHub, PagerDuty), polishing the user experience, addressing PR review feedback.

### Final Week — August 17 to August 24
- Address all pending review comments across the entire codebase.
- Final documentation pass (API boundaries, custom fields notation).
- Submit end-of-programme report.
