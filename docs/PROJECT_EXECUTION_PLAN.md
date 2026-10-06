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

The team will use **React** for the QuickBite implementation.

---

## 3. Sprint Scope

### Sprint Goal

> Allow a customer to view a restaurant menu, select items and a pickup time, and submit a simple food order.

### Sprint PBIs

**PBI-01 — View Restaurant Menu**  
Customer can view one fixed restaurant and its menu.

**PBI-02 — Select Menu Items**  
Customer can select menu items and adjust item quantities.

**PBI-03 — Select Pickup Time**  
Customer can select a pickup time for the order.

**PBI-04 — Submit Order**  
Customer can provide a pickup name, submit the order, and receive an on-screen confirmation.

### Intended Increment

Menu  
→ Select item(s) and quantities  
→ Select pickup time  
→ Enter pickup name  
→ Submit order  
→ Validate/process order  
→ Save order  
→ Display confirmation

### Out of Scope for This Sprint

- browsing multiple restaurants;
- cart page;
- employee interface;
- order-status management;
- customer account/login;
- payment;
- external order notifications.

The Sprint uses one fixed restaurant. These additional features remain in the Product Backlog for future Sprints.

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

**Technical** (To be confirmed)
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

**Technical** (To be confirmed)
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

**Technical** (To be confirmed)
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

**Technical** (To be confirmed)
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

The Product Backlog contains the currently known work for the QuickBite product.  
PBIs are ordered by product value and dependency, not by PBI number.

| Order | PBI | Title | Priority | Estimate | Sprint |
|---|---|---|---|---:|---|
| 1 | PBI-05 | Browse Restaurants | High | 3 | Future |
| 2 | PBI-01 | View Restaurant Menu | High | 3 | Current Sprint |
| 3 | PBI-02 | Select Menu Items | High | 3 | Current Sprint |
| 4 | PBI-03 | Select Pickup Time | High | 2 | Current Sprint |
| 5 | PBI-04 | Submit Order | High | 5 | Current Sprint |
| 6 | PBI-06 | Restaurant Views Incoming Orders | High | 5 | Future |
| 7 | PBI-07 | Restaurant Updates Order Status | Medium | 3 | Future |
| 8 | PBI-08 | Customer Views Order Status | Medium | 3 | Future |
| 9 | PBI-09 | Cancel Order | Medium | 3 | Future |
| 10 | PBI-10 | Restaurant Manages Menu | Medium | 5 | Future |
| 11 | PBI-11 | Customer Account and Login | Low | 8 | Future |
| 12 | PBI-12 | Order Confirmation Notification | Low | 5 | Future |
| 13 | PBI-13 | Payment Support | Low | 8 | Future |

Detailed descriptions, user stories, and acceptance criteria for each PBI are maintained in the corresponding GitHub Issues.

PBI-01, PBI-02, PBI-03, and PBI-04 are selected for the current Sprint.

### Estimation

Technique: Story Points
Scale: 1, 2, 3, 5, 8

The team used Story Points to estimate Product Backlog Items. 
 - Story Points compare PBIs based on the amount of work, technical complexity, uncertainty, risk, and dependencies. 
We used a Fibonacci-style scale of 1, 2, 3, 5, and 8. 
 - The Fibonacci-style scale reflects that larger work is harder to estimate precisely. The estimates were discussed and agreed on by the team. 


---

## 7. Definition of Done

A Sprint PBI is considered **Done** when:

- All acceptance criteria for the PBI are satisfied.
- The implementation is complete and works as expected.
- The work is committed to an appropriate feature branch.
- A pull request has been created and reviewed by at least one other team member.
- Relevant automated tests have been completed and pass.
- The feature has been integrated into the working Increment.
- No known critical defects remain.
- The GitHub Project status has been updated to **Done**.

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

### Day 1 — Sprint Planning and Setup

Meeting 1 has been completed.

The team has already confirmed:

- Product Backlog;
- Sprint scope;
- team capability;
- Scrum roles;
- technical work division;
- React as the development technology;
- Product Backlog priorities and estimates;
- Definition of Done.

**Scrum Master**
- Begin documenting Sprint Planning.
- Confirm the Sprint Goal with the team.
- Record the team capacity assessment.
- Confirm the selected Sprint PBIs:
  - PBI-01 — View Restaurant Menu;
  - PBI-02 — Select Menu Items;
  - PBI-03 — Select Pickup Time;
  - PBI-04 — Submit Order.
- Begin breaking selected PBIs into engineering tasks with the Developers.
- Begin creating the Sprint Backlog in GitHub Projects.
- Coordinate initial technical dependencies and work assignments.

**Developers**
- Participate in engineering-task breakdown.
- Confirm that assigned work is realistic for the Sprint.
- Prepare the React development environment.
- Review dependencies between assigned components.

**Product Owner**
- Finalize Part B Product Backlog work.
- Clarify PBI requirements and acceptance criteria as needed.

---

### Day 2 — Finalize Sprint Backlog and Begin Development

**Scrum Master and Developers**
- Finalize engineering tasks for the selected PBIs.
- Finalize the Sprint Backlog.
- Confirm task ownership and technical dependencies.
- Confirm the initial development sequence.
- Ensure the GitHub Project reflects the selected Sprint work.

**Developers**
- Create appropriate feature branches.
- Begin implementation of assigned Sprint work.
- Make meaningful commits.
- Update work status in GitHub Projects.

**Capture**
- Sprint Goal;
- capacity assessment;
- selected Sprint PBIs;
- engineering-task breakdown;
- Sprint Backlog;
- initial task coordination;
- initial Sprint board.

---

### Day 3 — Daily Scrum #1 and Development

**Daily Scrum #1**

Focus on:

- progress toward the Sprint Goal;
- completed or active work;
- work to do next;
- dependencies;
- impediments;
- any necessary adaptation.

**After the Daily Scrum**
- Continue implementation.
- Update the Sprint Backlog based on the discussion.
- Resolve identified dependencies or impediments.
- Continue meaningful commits and early testing.

**Capture**
- important progress;
- identified impediments;
- coordination decisions;
- adaptations made;
- updated Sprint Backlog.

---

### Day 4 — Development and Integration

Focus on:

- continuing implementation of Sprint PBIs;
- integrating related components;
- opening pull requests when work is ready;
- reviewing code from other team members;
- running relevant feature-level tests;
- keeping the Sprint Backlog current.

Do not add unnecessary scope.

---

### Day 5 — Daily Scrum #2 and Required Stakeholder Change

**Daily Scrum #2**

Focus on:

- progress toward the Sprint Goal;
- current dependencies;
- remaining work;
- impediments;
- necessary adaptations.

**Required Stakeholder Change**

Analyze:

> Customers should only select pickup times that the restaurant can realistically support based on current workload.

The team will determine:

- what changed;
- stakeholder clarification questions;
- whether PBI-03 should be modified or a new enhancement PBI should be created;
- priority of the change;
- Story Point estimate or re-estimate;
- whether the change should be implemented in the current Sprint or moved to a future Sprint;
- whether the Sprint Goal remains valid;
- any required Sprint Backlog adaptation.

Because pickup-time selection is already part of the current Sprint, the team must evaluate the impact of the new workload-based requirement before deciding how to respond.

**Capture**
- Daily Scrum #2;
- Product Backlog before the change;
- stakeholder clarification questions;
- change analysis;
- modified or new PBI;
- priority and estimate decision;
- current-Sprint versus future-Sprint decision;
- Sprint Goal impact;
- Product Backlog after the change;
- Sprint Backlog adaptation, if any.

---

### Day 6 — Finish and Verify the Increment

Focus on:

- completing remaining Sprint work;
- pull requests;
- code reviews;
- integration;
- automated testing;
- bug fixing;
- verification against acceptance criteria;
- verification against the Definition of Done.

The team should avoid introducing new functionality unless required to complete the Sprint Goal.

---

### Day 7 — Daily Scrum #3, Sprint Review, and Retrospective

**Daily Scrum #3**

Focus on:

- remaining work;
- Sprint Goal status;
- final impediments;
- final coordination or adaptation needed before the Sprint Review.

### Sprint Review

Demonstrate the working Increment:

Menu  
→ Select item(s) and quantities  
→ Select pickup time  
→ Enter pickup name  
→ Submit order  
→ Order confirmation

Obtain at least **three realistic stakeholder feedback items**.

For each feedback item, decide whether to:

- Accept;
- Reject;
- Clarify; or
- Add/Modify Product Backlog Item.

Update the Product Backlog where appropriate.

### Sprint Retrospective

Discuss:

- what went well;
- what did not go well;
- what slowed the team;
- what helped collaboration;
- whether the Definition of Done worked;
- what should change in the next Sprint.

Record at least **two concrete improvement actions**.

**Capture**
- Daily Scrum #3;
- final Sprint Backlog;
- working Increment evidence;
- stakeholder feedback;
- backlog adaptations from the Sprint Review;
- retrospective findings;
- improvement actions.

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
