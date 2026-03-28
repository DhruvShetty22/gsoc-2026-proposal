## Timeline

I plan to submit small PRs throught for the ease of Review and work on multiple PRs parallely to not get stuck on the review process.

---

### Pre-Community Bonding : April 1st to April 30th
- Dedicate this period to getting existing PRs to a mergeable state, so they don't go stale during GSoC.
  - [#38599](https://github.com/zulip/zulip/pull/38599) :Intercom company events
  - [#38279](https://github.com/zulip/zulip/pull/38279) :Jira comment-event notifications
  - [#38481](https://github.com/zulip/zulip/pull/38481) :Azure Alert integration
  - [#38650](https://github.com/zulip/zulip/pull/38650) :Import Slack Canvas posts

---

### Community Bonding : May 1st to May 25th
- I would like this period to be focused on research and preparatory work for my GSoC project, going through the documentation, studying existing work in completion candidates, and even closed WIPs, as there are many I can learn from.
- Most importantly, I will discuss the plan for the coming weeks with my mentors, align on issue priorities, and gather feedback on my open PRs.

### Coding Phase 1 : May 26th to July 10th

- **Backend Permissions & OAuth Infrastructure** : Start by implementing core decorator functions to restrict `INCOMING_WEBHOOK_BOT` access on read endpoints. The primary issues here are [#16431](https://github.com/zulip/zulip/issues/16431) and [#22405](https://github.com/zulip/zulip/issues/22405).
- **OAuth Implementation** : Extend the API dispatcher to accept Bearer tokens alongside API keys and enforce scope restrictions. No dedicated open issue exists yet, will discuss the approach with mentors early in this phase.
- **Integrations Page Revamp** : Towards the end of this phase, begin work on the `/integrations` page UX, implementing the "Add to Zulip" button and stream picker modal ([#9815](https://github.com/zulip/zulip/issues/9815)).

### Midterm Evaluation : July 7th to July 10th
- **Deliverables:** Working backend permissions system, Bearer token authentication.
- Submit midterm evaluation.

---

### Coding Phase 2 : July 18th to August 16th
- With the internship winding down, I will have significantly more time in this phase. I plan to work on issues that still need feedback or experimentation to move forward.
- Focus areas include the OAuth consent screen and `/integration` page. (if not completed in Phase 1), along with:
  - [#30139: Auto populate bot avatar for webhook integrations bot](https://github.com/zulip/zulip/issues/30139)
  - [#36564: Improve "Generate integration URL" modal's "Topic" field](https://github.com/zulip/zulip/issues/36564)
  - [#33788: Add "copy" button to URL in "Generate URL for an integration" modal](https://github.com/zulip/zulip/issues/33788)
These PRs have significant work already done by other contributors which is why i think it would be realistic to complete them in this phase.

### Final Week : August 17 to August 24
- Address all outstanding review comments across PRs.
- Final documentation pass covering API boundaries, OAuth scope, and the "Add to Zulip" flow.
- Submit end-of-programme report.

---

### Summary

| Phase | Dates | Focus |
|-------|-------|:-----:|
| Pre-Community Bonding | <nobr>April 1 – April 30</nobr> | Work on existing open PRs |
| Community Bonding | <nobr>May 1 – May 25</nobr> | Research, product decision alignment, mentor discussions |
| Coding Phase 1 | <nobr>May 26 – July 10</nobr> | Backend permissions for Bot and OAuth infrastructure  |
| Midterm Evaluation | <nobr>July 7 – July 10</nobr> | Review, buffer, sync with mentors |
| Coding Phase 2 | <nobr>July 18 – Aug 16</nobr> | integrations page revamp,OAuth scope enforcement, consent screen, UX polish |
| Final Week | <nobr>Aug 17 – Aug 24</nobr> | PR reviews, docs, final report |