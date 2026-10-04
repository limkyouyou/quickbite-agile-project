# QuickBite — Project Execution Plan

## 1. Objective

Complete one small Scrum Sprint that demonstrates:

- planning and backlog management;
- meaningful technical contribution from all four members;
- Git branching, commits, pull requests, and code review;
- testing and integration;
- three Daily Scrums;
- controlled response to stakeholder change;
- Sprint Review and stakeholder feedback;
- Sprint Retrospective;
- a small working software Increment.

We are not implementing the complete QuickBite system.

---

## 2. Tools

- **GitHub Projects:** Product Backlog, Sprint Backlog, estimates, priorities, tasks, work status.
- **GitHub Repository:** branches, commits, pull requests, reviews, tests, source code.
- **Google Docs:** final team report.
- **`docs/PROJECT_EXECUTION_PLAN.md`:** this plan.

Development technology will be confirmed during Sprint Planning. Python/Flask is the current candidate.

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

Not included in this Sprint:

- cart page;
- pickup-time selection;
- employee interface;
- order-status management;
- login;
- multiple restaurants;
- payment;
- notifications.

These may remain in the Product Backlog for future Sprints.

---

## 4. Scrum Team and Responsibilities

All four members are Developers and must make a meaningful technical contribution.

### Member 1 — Product Owner + Developer

**Scrum**
- Prepare initial Product Backlog with at least 10 PBIs.
- Prepare user stories and acceptance criteria.
- Prepare initial backlog ordering and top-five priority rationale.
- Propose the Sprint Goal.
- Clarify requirements during estimation and Sprint Planning.
- Manage Product Backlog priorities.
- Lead analysis of the required stakeholder change.
- Update backlog after Sprint Review feedback.

**Technical**
- Restaurant/menu page and menu rendering.
- Related test(s).

**Evidence**
- Product Backlog.
- User stories/acceptance criteria.
- priorities and estimates.
- Sprint Goal.
- backlog before/after required change.
- backlog after Sprint Review.

**Report**
- Parts A and B.
- Product aspects of Parts F and G.

---

### Member 2 — Scrum Master + Developer

**Scrum**
- Facilitate Scrum events.
- Keep Daily Scrums focused on Sprint Goal, next work, impediments, and adaptation.
- Help remove/track impediments.
- Ensure GitHub Project stays updated.
- Facilitate Sprint Retrospective.

**Technical**
- Order form and input validation.
- Related test(s).

**Evidence**
- Daily Scrum #1, #2, and #3.
- project board at different stages.
- impediments/adaptations.
- Retrospective and improvement actions.

**Report**
- Parts C, E, and H.

---

### Member 3 — Developer

**Scrum**
- Participate in estimation, capacity assessment, Sprint planning, Daily Scrums, Review, and Retrospective.

**Technical**
- Order submission/backend processing.
- Confirmation page.
- Related test(s).

**Evidence**
- branch and commits.
- pull request.
- code review.
- working order functionality.

**Report**
- Part D: implementation and Git collaboration.

---

### Member 4 — Developer

**Scrum**
- Participate in estimation, capacity assessment, Sprint planning, Daily Scrums, Review, and Retrospective.

**Technical**
- Order persistence/data handling.
- Automated/integration testing.
- Integration support.

**Evidence**
- branch and commits.
- pull request.
- test results.
- integration evidence.
- final working Increment.

**Report**
- Part D: testing, integration, and Definition of Done.

---

## 5. Shared Team Decisions

The Product Owner prepares requirements and priorities, but the whole team participates in:

- PBI estimation;
- capacity assessment;
- Sprint PBI selection;
- engineering-task breakdown;
- technical design;
- code review;
- testing and integration.

The Product Owner decides product priority.

Developers decide how the selected work will be implemented.

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

## 8. Git Workflow

For technical work:

Issue/Task  
→ Feature branch  
→ Meaningful commits  
→ Pull request  
→ Review by another member  
→ Tests  
→ Merge  
→ Move work to Done

Avoid significant direct development on `main`.

---

# 9. Seven-Day Schedule

## Before Meeting 1

### Product Owner
Prepare:
- 10+ initial PBIs;
- user stories;
- acceptance criteria;
- initial priority order;
- top-five rationale;
- proposed Sprint Goal.

### Scrum Master
Prepare:
- GitHub Project;
- board columns/statuses;
- meeting/Daily Scrum note template.

### Everyone
- review assignment;
- review proposed backlog;
- confirm availability for the Sprint.

---

## Day 1 — Meeting 1

### Sprint Planning

Complete:

1. confirm Product Backlog;
2. clarify PBIs;
3. estimate PBIs;
4. confirm backlog ordering;
5. establish Sprint Goal;
6. assess team capacity;
7. select Sprint PBIs;
8. break PBIs into engineering tasks;
9. coordinate technical work;
10. confirm Definition of Done;
11. create Sprint Backlog;
12. confirm development technology.

Begin development.

### Daily Scrum #1

After initial work has started, record:

- progress toward Sprint Goal;
- next work;
- impediments;
- necessary plan changes.

### Capture Evidence

- Product Backlog;
- acceptance criteria;
- estimates/priorities;
- Definition of Done;
- Sprint Goal;
- Sprint Backlog;
- initial board;
- Daily Scrum #1.

---

## Days 2–3 — Development

Members work independently.

- create branches;
- implement assigned work;
- make meaningful commits;
- update GitHub Project;
- open early pull requests;
- review code;
- begin integration/testing.

---

## Day 4 — Meeting 2

### Daily Scrum #2

Record:

- Sprint Goal progress;
- dependencies;
- next work;
- impediments;
- adaptations.

### Required Stakeholder Change

Analyze:

> Customers should only select pickup times that the restaurant can realistically support based on current workload.

Determine:

- what changed;
- stakeholder clarification questions;
- new/modified PBI;
- priority;
- estimate;
- whether current Sprint should change;
- whether Sprint Goal remains valid;
- what belongs in a future Sprint.

Recommended approach:

Modify the future **pickup-time PBI** to include restaurant capacity and keep it outside the current Sprint unless the team identifies a strong reason to change the Sprint.

### Capture Evidence

- Daily Scrum #2;
- backlog before change;
- change analysis;
- modified/new PBI;
- backlog after change;
- any Sprint Backlog adaptation.

---

## Days 5–6 — Finish the Increment

Focus on:

- completing existing Sprint work;
- pull requests;
- code reviews;
- integration;
- automated testing;
- bug fixing;
- acceptance criteria;
- Definition of Done.

Do not add unnecessary scope.

---

## Day 7 — Meeting 3

### Daily Scrum #3

Record:

- remaining work;
- Sprint Goal status;
- impediments;
- final adaptations.

### Sprint Review

Demonstrate the actual Increment:

Menu  
→ Select item(s)  
→ Enter name  
→ Submit order  
→ Order confirmation

Obtain at least **three realistic stakeholder feedback items**.

For each feedback item decide:

- Accept;
- Reject;
- Clarify; or
- Add/Modify Product Backlog Item.

Update the Product Backlog where appropriate.

### Sprint Retrospective

Discuss:

- what went well;
- what did not;
- what slowed the team;
- what helped collaboration;
- whether the Definition of Done worked;
- what should change next Sprint.

Record at least **two concrete improvement actions**.

---

# 10. Required Evidence Checklist

## Planning
- [ ] Product Backlog with 10+ PBIs
- [ ] user stories and acceptance criteria
- [ ] estimates and priorities
- [ ] top-five priority rationale
- [ ] Definition of Done
- [ ] Sprint Goal
- [ ] Sprint Backlog

## Execution
- [ ] board at different Sprint stages
- [ ] branches
- [ ] meaningful commits
- [ ] pull requests
- [ ] code reviews
- [ ] testing
- [ ] integration
- [ ] working Increment

## Scrum
- [ ] Daily Scrum #1
- [ ] Daily Scrum #2
- [ ] Daily Scrum #3

## Change
- [ ] backlog before change
- [ ] change analysis
- [ ] new/modified PBI
- [ ] backlog after change

## Review
- [ ] working-software demonstration
- [ ] three stakeholder feedback items
- [ ] feedback decisions
- [ ] resulting backlog updates

## Retrospective
- [ ] retrospective evidence
- [ ] two concrete improvement actions

---

# 11. Report Structure and Ownership

| Section | Primary Owner |
|---|---|
| Part A — Scrum Team | Product Owner |
| Part B — Product Backlog | Product Owner |
| Part C — Sprint Planning | Scrum Master |
| Part D — Sprint Execution | Developers 3 & 4 |
| Part E — Daily Scrums | Scrum Master |
| Part F — Respond to Change | Product Owner |
| Part G — Sprint Review | Product Owner |
| Part H — Retrospective | Scrum Master |
| Agile Reflection | Entire team |

All members review the complete report and must be able to explain the team's artifacts, decisions, implementation, and Agile process.

---

# 12. Agile Reflection

Use actual project evidence to discuss at least four of:

- incremental delivery;
- responding to change;
- stakeholder collaboration;
- working software;
- feedback;
- self-organization;
- technical quality;
- simplicity;
- sustainable work;
- continuous improvement.

Focus on what the team actually did rather than explaining Agile definitions.

---

## Team Priority

Build the **smallest complete Increment**, finish it properly, and produce clear evidence of:

**Plan → Build → Inspect → Adapt → Deliver → Get Feedback → Improve**