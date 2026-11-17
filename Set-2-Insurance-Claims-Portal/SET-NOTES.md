# Set 2 – Insurance Claims Portal

**Scenario:** An insurer is building a self-service portal where customers lodge claims, upload documents and track settlement status.

| Question | Folder |
|---|---|
| 1. Draft the product vision and a Waterfall-versus-Agile comparison (maximum half a page) explaining why Agile suits this programme. | [01-vision-and-waterfall-vs-agile](./01-vision-and-waterfall-vs-agile/) |
| 2. Define four epics (Claim Registration, Document Upload, Claim Tracking, Settlement Notifications) and split them into 12–14 user stories. | [02-epics-and-user-stories](./02-epics-and-user-stories/) |
| 3. Run an INVEST review; identify stories that are too large and split them vertically rather than by technical layer. | [03-invest-review](./03-invest-review/) |
| 4. Write acceptance criteria in Given / When / Then format for the Claim Registration stories, including a validation failure scenario. | [04-acceptance-criteria](./04-acceptance-criteria/) |
| 5. Estimate every story using Planning Poker values (1, 2, 3, 5, 8, 13), record the discussion on any outlier and compute the total backlog size. | [05-prioritisation-and-estimation](./05-prioritisation-and-estimation/) |
| 6. Create the JIRA project with the board, epics, story states (To Do, In Progress, In Review, Done) and attach the DoD. | [06-jira-board](./06-jira-board/) |

**Deliverables**

- JIRA import file and board view: [06-jira-board](./06-jira-board/)
- Backlog table (story, priority, points): below and [backlog_table.csv](./05-prioritisation-and-estimation/backlog_table.csv)
- DoR / DoD: [DoR_DoD.md](./06-jira-board/DoR_DoD.md)
- One-page note: [Roles_Events_Artifacts.md](Roles_Events_Artifacts.md)

## Backlog (55 points)

| Story | Epic | Priority | Points |
|---|---|---|---|
| S1 to log in with my policy number and an OTP | Claim Registration | High | 3 |
| S2 to register a motor claim with incident date, place and description | Claim Registration | Highest | 5 |
| S3 to register a health claim for a hospital stay | Claim Registration | High | 5 |
| S4 to save a half-filled claim as a draft | Claim Registration | Medium | 3 |
| S5 to upload photos and PDFs of my documents from my phone | Document Upload | Highest | 5 |
| S6 to see a checklist of documents still needed for my claim | Document Upload | High | 3 |
| S7 to see uploaded documents next to the claim | Document Upload | High | 3 |
| S8 to see the current status and next step of my claim | Claim Tracking | Highest | 3 |
| S9 to see the history of status changes with dates | Claim Tracking | Medium | 2 |
| S10 to message the claims officer from the claim page | Claim Tracking | Low | 8 |
| S11 to get an SMS and email when my claim is approved or rejected | Settlement Notifications | High | 3 |
| S12 to see the settled amount and any deductions explained | Settlement Notifications | High | 5 |
| S13 to download the settlement letter as PDF | Settlement Notifications | Medium | 2 |
| S14 to register a claim on behalf of a walk-in customer | Claim Registration | Low | 5 |
