# Question 6 – Jira board

**Question:** Create the JIRA project with the board, epics, story states (To Do, In Progress, In Review, Done) and attach the DoD.

JIRA project key **CLAIM**: 4 epics and 14 stories (55 points).

Board columns / workflow states: **To Do → In Progress → In Review → Done**. The DoD below is attached to the board (JIRA: Board settings → add it to the board description / a pinned Confluence page).

**How to load it into JIRA:** create a Scrum project with key CLAIM, then *Settings → System → External System Import → CSV*, choose `output/jira_import.csv` and map the columns (Issue Id, Issue Type, Summary, Description, Parent Id, Priority, Story Points, Status).

![board](jira_board.png)

_Board layout of the stories in `jira_import.csv` – importing the CSV into JIRA loads the same board._

## Definition of Done

- [ ] Code peer-reviewed and merged to main
- [ ] Unit and API tests pass in the CI pipeline
- [ ] Acceptance criteria verified by the tester on the staging portal
- [ ] Accessibility check (WCAG 2.1 AA) on new screens
- [ ] Customer data masked in logs; security scan has no high findings
- [ ] Product Owner accepted the story
- [ ] Help text and release notes updated


## Files in this folder

- [flowchart.svg](flowchart.svg)
- [jira_board.png](jira_board.png)
- [jira_import.csv](jira_import.csv)

## Approach

![flowchart](flowchart.svg)
