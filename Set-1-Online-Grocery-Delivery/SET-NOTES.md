# Set 1 – Online Grocery Delivery Application

**Scenario:** A regional supermarket chain is launching a grocery ordering and home-delivery application. Management wants an estimated, prioritised backlog before the first sprint begins.

| Question | Folder |
|---|---|
| 1. Write a product vision statement and identify the three Scrum roles for the team, listing one anti-pattern for each role. | [01-vision-and-scrum-roles](./01-vision-and-scrum-roles/) |
| 2. Create at least three epics (for example Browse and Search, Cart and Checkout, Delivery Tracking) and break them into 12 user stories in the 'As a / I want / so that' format. | [02-epics-and-user-stories](./02-epics-and-user-stories/) |
| 3. Apply the INVEST checklist to every story and rewrite at least two stories that fail it. | [03-invest-review](./03-invest-review/) |
| 4. Write Given / When / Then acceptance criteria for five stories, including one negative scenario. | [04-acceptance-criteria](./04-acceptance-criteria/) |
| 5. Prioritise the backlog using MoSCoW, estimate the stories with Fibonacci story points using Planning Poker, and justify the reference story chosen. | [05-prioritisation-and-estimation](./05-prioritisation-and-estimation/) |
| 6. Publish the epics and stories on a JIRA board with the Definition of Ready and Definition of Done recorded. | [06-jira-board](./06-jira-board/) |

**Deliverables**

- JIRA import file and board view: [](.//)
- Backlog table (story, priority, points): below and [backlog_table.csv](./05-prioritisation-and-estimation/backlog_table.csv)
- DoR / DoD: [DoR_DoD.md](./06-jira-board/DoR_DoD.md)

## Backlog (60 points)

| Story | Epic | Priority | Points |
|---|---|---|---|
| S1 to browse products by category and sub-category | Browse and Search | Must | 3 |
| S2 to search products by name and get results even with small spelling mistakes | Browse and Search | Must | 5 |
| S3 to filter results by price, brand and veg / non-veg | Browse and Search | Should | 3 |
| S4 to see whether an item is in stock at my nearest store | Browse and Search | Must | 5 |
| S5 to add items to my cart and change quantities | Cart and Checkout | Must | 3 |
| S6 to apply a coupon code to my cart | Cart and Checkout | Should | 3 |
| S7 to choose a 2-hour delivery slot | Cart and Checkout | Must | 5 |
| S8 to pay by UPI, card or cash on delivery | Cart and Checkout | Must | 8 |
| S9 to reorder a previous order in one tap | Cart and Checkout | Could | 2 |
| S10 to see my order status (packed, out for delivery, delivered) | Delivery Tracking | Must | 3 |
| S11 to get a notification when my order is out for delivery | Delivery Tracking | Should | 2 |
| S12 to report a missing or damaged item after delivery | Delivery Tracking | Should | 5 |
| S13 to track the delivery partner live on a map | Delivery Tracking | Won't (this release) | 13 |
