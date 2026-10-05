# QuickBite — Project Execution Plan

## 1. Objective

Complete one small Scrum Sprint that demonstrates:

- planning and backlog management;
- meaningful technical contribution from all four members;
- Git branching, commits, pull requests, code review, testing, and integration;
- three Daily Scrums;
- controlled response to stakeholder change;
- Sprint Review and stakeholder feedback;
- Sprint Retrospective;
- a small working software Increment.

We are **not** implementing the complete QuickBite system.

---

## 2. Tools

- **GitHub Projects:** Product Backlog, Sprint Backlog, priorities, estimates, engineering tasks, and work status.
- **GitHub Repository:** source code, branches, commits, pull requests, reviews, and tests.
- **Google Docs:** final team report.
- **`docs/PROJECT_EXECUTION_PLAN.md`:** team execution reference.

Development technology will be confirmed during Sprint Planning. Plain HTML/CSS/JavaScript or Python/Flask are current options.

---

## 3. Sprint Scope

### Sprint Goal

> Allow a customer to view a restaurant menu and submit a simple food order.

### Sprint PBIs

**PBI 1 — View Restaurant Menu**  
Customer can view one fixed restaurant and its menu.

**PBI 2 — Place Simple Order**  
Customer can select menu items, enter a name, submit the order, and receive confirmation.

### Intended Increment

Menu  
→ Select item(s)  
→ Enter customer name  
→ Submit order  
→ Validate/process order  
→ Save order  
→ Display confirmation

### Out of Scope for This Sprint

- cart page;
- pickup-time selection;
- employee interface;
- order-status management;
- login;
- multiple restaurants;
- payment;
- notifications.

These can remain in the Product Backlog for future Sprints.

---

## 4. Scrum Team and Work Division

All four members are Developers and must make a meaningful technical contribution.

### Member 1 — Product Owner + Developer

**Report**
- Part B — Product Backlog
- Part F — Respond to Change

**Scrum / Product Responsibilities**
- Prepare initial 10+ PBIs.
- Prepare user stories and acceptance criteria.
- Propose initial backlog order.
- Prepare rationale for top five PBIs.
- Propose Sprint Goal.
- Clarify requirements during estimation.
- Manage Product Backlog priorities.
- Lead analysis of the required stakeholder change.
- Update Product Backlog after stakeholder feedback.

**Technical**
- Implement menu and menu rendering:
  - fixed restaurant information;
  - menu item data;
  - item names and prices;
  - item-selection/quantity controls;
  - rendering menu data in the UI.
- Write feature-level test(s) for menu rendering.

**Evidence**
- **Part B:** Initial Product Backlog with 10+ PBIs.
- **Part B:** User stories and acceptance criteria.
- **Part B:** Priority/order.
- **Part B:** Final team estimates.
- **Part B:** Top-five priority rationale.
- **Part B:** Definition of Done.
- **Part F:** Product Backlog before stakeholder change.
- **Part F:** Stakeholder clarification questions.
- **Part F:** New/modified pickup-time PBI.
- **Part F:** Priority/estimate decision for the change.
- **Part F:** Current-Sprint vs future-Sprint decision.
- **Part F:** Sprint Goal impact/review.
- **Part F:** Product Backlog after change.
- **Part D:** Own branch, commits, PR, review, and test evidence.

---

### Member 2 — Scrum Master + Developer

**Report**
- Part C — Sprint Planning
- Part E — Daily Scrum and Adaptation

**Scrum Responsibilities**
- Facilitate Scrum events.
- Keep Daily Scrums focused on Sprint Goal, next work, impediments, and adaptation.
- Help identify/remove impediments.
- Ensure the board stays current.
- Facilitate the Sprint Retrospective.

**Technical**
- Implement order form and validation:
  - customer-name input;
  - read selected items/quantities;
  - reject blank customer name;
  - reject orders with no selected items;
  - reject invalid quantities;
  - display useful validation messages;
  - submit validated data to order processing.
- Write feature-level tests for validation rules.

**Evidence**
- **Part C:** Sprint Planning evidence.
- **Part C:** Sprint Goal.
- **Part C:** Team capacity assessment.
- **Part C:** Selected Sprint PBIs.
- **Part C:** Engineering-task breakdown.
- **Part C:** Sprint Backlog.
- **Part C:** Initial technical-work coordination.
- **Part E:** Daily Scrum #1 evidence.
- **Part E:** Daily Scrum #2 evidence.
- **Part E:** Daily Scrum #3 evidence.
- **Part E:** Board progression.
- **Part E:** Identified impediments.
- **Part E:** Decisions and adaptations.
- **Part D:** Own branch, commits, PR, review, and test evidence.

---

### Member 3 — Developer

**Report**
- Part D — Execute Sprint and Produce Working Increment
- Part G — Sprint Review and Stakeholder Feedback

**Technical**
- Implement order processing and confirmation:
  - receive validated order input;
  - construct the order data/object;
  - calculate item totals and overall total if used;
  - generate an order identifier if used;
  - send the order to persistence;
  - display successful order confirmation.
- Write feature-level tests for order processing and confirmation:
  - correct order data is created;
  - selected items appear correctly;
  - totals are correct if used;
  - confirmation displays expected information.

**Evidence**
- **Part D:** Git branches from all members.
- **Part D:** Meaningful commit history.
- **Part D:** Pull requests.
- **Part D:** Code-review evidence.
- **Part D:** Feature-level test evidence.
- **Part D:** Working Increment screenshots.
- **Part D:** Sprint Backlog updates during implementation.
- **Part G:** Working Increment demonstrated during Sprint Review.
- **Part G:** At least three stakeholder feedback items.
- **Part G:** Decision for each feedback item: Accept / Reject / Clarify / Add or Modify PBI.
- **Part G:** Learning from each feedback item.
- **Part G:** Product Backlog after Sprint Review.
- **Part D:** Own branch, commits, PR, review, and tests.

---

### Member 4 — Developer

**Report**
- Part A — Organize the Scrum Team
- Part H — Sprint Retrospective
- Coordinate Agile Reflection

**Technical**
- Implement persistence and integration:
  - define how completed orders are stored;
  - implement save/retrieve operations;
  - use `localStorage` if browser-only, or SQLite if a backend is selected;
  - connect menu → form → processing → persistence → confirmation;
  - resolve integration issues between components.
- Implement automated integration tests for the complete workflow:
  - select item;
  - enter valid customer information;
  - submit order;
  - verify order is stored correctly;
  - verify confirmation is displayed correctly.
- Verify the final Increment against the Definition of Done.

**Evidence**
- **Part A:** Final Scrum-team role/responsibility table.
- **Part A:** Evidence that all four members have technical responsibilities.
- **Part D:** Persistence implementation.
- **Part D:** Automated integration-test results.
- **Part D:** Integration evidence.
- **Part D:** Definition of Done verification.
- **Part H:** Retrospective notes.
- **Part H:** What went well / did not go well / slowed the team / helped collaboration.
- **Part H:** DoD evaluation.
- **Part H:** At least two concrete improvement actions.
- **Agile Reflection:** Collect one concrete example from each member.
- **Part D:** Own branch, commits, PR, review, and tests.

---

## 5. Shared Responsibilities — All Members

All members must:

- participate in Sprint Planning;
- estimate PBIs together;
- assess team capacity;
- select realistic Sprint PBIs;
- create the Definition of Done;
- break selected PBIs into engineering tasks;
- create the Sprint Backlog;
- coordinate technical work;
- make a meaningful technical contribution;
- use a feature branch and meaningful commits;
- participate in pull-request/code review;
- execute the Sprint and help produce the integrated Increment;
- update the Sprint Backlog as work changes;
- participate in all three Daily Scrums;
- participate in the required stakeholder-change analysis;
- participate in Sprint Review;
- participate in Sprint Retrospective;
- contribute one concrete example to the Agile Reflection;
- review the final report and screenshots;
- participate in the TA presentation/demo;
- be able to explain the backlog, Sprint Goal, decisions, implementation, testing, Increment, adaptation, and individual contribution.

**Evidence rule:** Whoever owns an activity/work product captures its evidence. Each member must also capture their own technical Git evidence.

---

## 6. Product Backlog

Create at least 10 PBIs.

Suggested backlog:

1. View restaurant menu.
2. Place simple order.
3. Select pickup time.
4. Restaurant views incoming orders.
5. Restaurant updates order status.
6. Customer views order status.
7. Browse multiple restaurants.
8. Cancel order.
9. Restaurant manages menu.
10. Customer account/login.
11. Order confirmation notification.
12. Payment support.

Only PBIs 1–2 are initially planned for this Sprint.

Use story-point estimates:

`1, 2, 3, 5, 8`

Developers estimate collaboratively after the Product Owner explains each PBI.

---

## 7. Definition of Done

A Sprint PBI is Done when:

- acceptance criteria are satisfied;
- implementation is complete;
- work is committed on an appropriate branch;
- another team member reviewed the pull request;
- relevant tests pass;
- the feature is integrated;
- no known critical defect remains;
- GitHub Project is updated.

---

## 8. Testing Split

- **Member 1:** menu-rendering feature tests.
- **Member 2:** input-validation feature tests.
- **Member 3:** order-processing/confirmation feature tests.
- **Member 4:** automated integration tests for the full workflow.

Member 4's tests verify that components work together; they are not duplicates of Member 3's feature tests.

---

## 9. Git Workflow

Issue / Engineering Task  
→ Feature Branch  
→ Meaningful Commits  
→ Pull Request  
→ Review by Another Member  
→ Tests  
→ Merge  
→ Move Work to Done

Avoid significant direct development on `main`.

---

## 10. Seven-Day Schedule

### Before Meeting 1

**Product Owner**
- Prepare 10+ initial PBIs.
- Prepare user stories and acceptance criteria.
- Prepare initial priority order and top-five rationale.
- Propose Sprint Goal.

**Scrum Master**
- Prepare GitHub Project.
- Prepare board statuses.
- Prepare meeting/Daily Scrum note template.

**Everyone**
- Review assignment and proposed backlog.
- Confirm Sprint availability.

---

### Day 1 — Meeting 1

**Sprint Planning**
1. Confirm Product Backlog.
2. Clarify PBIs.
3. Estimate PBIs.
4. Confirm backlog ordering.
5. Establish Sprint Goal.
6. Assess team capacity.
7. Select Sprint PBIs.
8. Break PBIs into engineering tasks.
9. Coordinate technical work.
10. Confirm Definition of Done.
11. Create Sprint Backlog.
12. Confirm development technology.

Begin development.

**Daily Scrum #1**
- progress toward Sprint Goal;
- next work;
- impediments;
- necessary plan changes.

**Capture**
- Product Backlog;
- acceptance criteria;
- estimates/priorities;
- DoD;
- Sprint Goal;
- Sprint Backlog;
- initial board;
- Daily Scrum #1.

---

### Days 2–3 — Development

- Create branches.
- Implement assigned work.
- Make meaningful commits.
- Update GitHub Project.
- Open early PRs.
- Review code.
- Begin integration/testing.

---

### Day 4 — Meeting 2

**Daily Scrum #2**
- Sprint Goal progress;
- dependencies;
- next work;
- impediments;
- adaptations.

**Required Stakeholder Change**

Analyze:

> Customers should only select pickup times that the restaurant can realistically support based on current workload.

Determine:

- what changed;
- stakeholder clarification questions;
- new/modified PBI;
- priority;
- estimate;
- whether the current Sprint should change;
- whether the Sprint Goal remains valid;
- what belongs in a future Sprint.

Recommended approach: modify the future pickup-time PBI to include restaurant capacity and keep it outside the current Sprint unless the team finds a strong reason to change the Sprint.

**Capture**
- Daily Scrum #2;
- backlog before change;
- change analysis;
- modified/new PBI;
- backlog after change;
- Sprint Backlog adaptation, if any.

---

### Days 5–6 — Finish the Increment

Focus on:

- completing Sprint work;
- pull requests;
- code reviews;
- integration;
- automated testing;
- bug fixing;
- acceptance criteria;
- Definition of Done.

Do not add unnecessary scope.

---

### Day 7 — Meeting 3

**Daily Scrum #3**
- remaining work;
- Sprint Goal status;
- impediments;
- final adaptations.

**Sprint Review**

Demonstrate:

Menu  
→ Select item(s)  
→ Enter name  
→ Submit order  
→ Order confirmation

Obtain at least **three realistic stakeholder feedback items**.

For each decide:

- Accept;
- Reject;
- Clarify; or
- Add/Modify Product Backlog Item.

Update the Product Backlog where appropriate.

**Sprint Retrospective**

Discuss:

- what went well;
- what did not;
- what slowed the team;
- what helped collaboration;
- whether the DoD worked;
- what should change next Sprint.

Record at least **two concrete improvement actions**.

---

## 11. Report Ownership

| Section | Primary Owner |
|---|---|
| Part A — Scrum Team | Member 4 |
| Part B — Product Backlog | Member 1 |
| Part C — Sprint Planning | Member 2 |
| Part D — Sprint Execution | Member 3 |
| Part E — Daily Scrums | Member 2 |
| Part F — Respond to Change | Member 1 |
| Part G — Sprint Review | Member 3 |
| Part H — Retrospective | Member 4 |
| Agile Reflection | All members; Member 4 coordinates |

---

## 12. Agile Reflection

Each member contributes one concrete example:

- **Member 1:** responding to change.
- **Member 2:** self-organization/adaptation.
- **Member 3:** working software/incremental delivery.
- **Member 4:** technical quality/continuous improvement.

The reflection should use actual project evidence rather than definitions.

---

## Team Priority

Build the **smallest complete Increment**, finish it properly, and produce clear evidence of:

**Plan → Build → Inspect → Adapt → Deliver → Get Feedback → Improve**
