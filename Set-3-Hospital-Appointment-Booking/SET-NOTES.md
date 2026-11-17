# Set 3 – Hospital Appointment Booking Application

**Scenario:** A hospital group wants a mobile application for booking, rescheduling and cancelling doctor appointments, with reminder notifications.

| Question | Folder |
|---|---|
| 1. Write the vision statement and list the stakeholders; map each stakeholder to Product Owner, Scrum Master, Developer or Customer. | [01-vision-and-stakeholders](./01-vision-and-stakeholders/) |
| 2. Create epics for Booking, Rescheduling and Cancellation, Reminders and Doctor Schedule Management, and write at least 12 user stories. | [02-epics-and-user-stories](./02-epics-and-user-stories/) |
| 3. Review each story against INVEST and rewrite those that are not independent or testable. | [03-invest-review](./03-invest-review/) |
| 4. Write Given / When / Then acceptance criteria for the booking and cancellation stories (include the 'slot already taken' case). | [04-acceptance-criteria](./04-acceptance-criteria/) |
| 5. Prioritise with business value versus effort, run a Planning Poker round, and explain how a story-point differs from an hour. | [05-prioritisation-and-estimation](./05-prioritisation-and-estimation/) |
| 6. Publish the backlog in JIRA and define the team's DoR and DoD with at least six checklist items each. | [06-jira-board](./06-jira-board/) |

**Deliverables**

- JIRA import file and board view: [06-jira-board](./06-jira-board/)
- Backlog table (story, priority, points): below and [backlog_table.csv](./05-prioritisation-and-estimation/backlog_table.csv)
- DoR / DoD: [DoR_DoD.md](./06-jira-board/DoR_DoD.md)

## Backlog (55 points)

| Story | Epic | Priority | Points |
|---|---|---|---|
| S1 to search doctors by speciality, hospital and language | Booking | Value 8 / Effort 3 | 3 |
| S2 to see a doctor's free slots for the next 14 days | Booking | Value 9 / Effort 5 | 5 |
| S3 to book a free slot and get a confirmation number | Booking | Value 10 / Effort 5 | 5 |
| S4 to pay the consultation fee online while booking | Booking | Value 6 / Effort 8 | 8 |
| S5 to book for a family member from my account | Booking | Value 6 / Effort 3 | 3 |
| S6 to reschedule my appointment to another free slot of the same doctor | Rescheduling and Cancellation | Value 8 / Effort 3 | 3 |
| S7 to cancel my appointment up to 2 hours before the slot | Rescheduling and Cancellation | Value 8 / Effort 2 | 2 |
| S8 to get a refund when I cancel a prepaid appointment | Rescheduling and Cancellation | Value 5 / Effort 5 | 5 |
| S9 an SMS and app reminder 24 hours and 2 hours before my appointment | Reminders | Value 9 / Effort 3 | 3 |
| S10 to confirm or cancel from the reminder message | Reminders | Value 7 / Effort 3 | 3 |
| S11 to see my appointments for the day in order | Doctor Schedule Management | Value 7 / Effort 2 | 2 |
| S12 to block slots for leave or surgery | Doctor Schedule Management | Value 9 / Effort 5 | 5 |
| S13 to move all of a doctor's patients to another doctor when the doctor is absent | Doctor Schedule Management | Value 6 / Effort 8 | 8 |
