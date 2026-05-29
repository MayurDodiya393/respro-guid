# Respro � Master User Guide

**For business users, coordinators, managers, and administrators**  
*Plain-language guide � no technical background required*

**Last updated:** May 2026  
**Application:** Respro Dashboard (Flow Monitoring System)

---

## Table of contents

1. [What is Respro?](#1-what-is-respro)
2. [Logging in and signing out](#2-logging-in-and-signing-out)
3. [How to move around the app (navigation)](#3-how-to-move-around-the-app-navigation)
4. [Your account, photo, and roles](#4-your-account-photo-and-roles)
5. [Permissions � why some menus are hidden](#5-permissions--why-some-menus-are-hidden)
6. [Home dashboard](#6-home-dashboard)
7. [Work center](#7-work-center)
8. [Workflow](#8-workflow)
9. [Checklist engine](#9-checklist-engine)
10. [MECA benchmark](#10-meca-benchmark)
11. [Monthly planning](#11-monthly-planning)
12. [Delegation engine](#12-delegation-engine)
13. [Masters (setup data)](#13-masters-setup-data)
14. [Settings](#14-settings)
15. [Which tool to use for which job](#15-which-tool-to-use-for-which-job)
16. [Complete path reference (quick lookup)](#16-complete-path-reference-quick-lookup)

---

## 1. What is Respro?

Respro is a web application that helps your organization **plan work, assign it to people, track deadlines, and measure performance** � without relying only on spreadsheets and email.

It brings together:

| Area | What it is for (simple terms) |
|------|-------------------------------|
| **Work center** | Your daily tasks (FMS), alerts, and personal profile |
| **Workflow** | Multi-step business processes (FMS templates, running instances, SLA) |
| **Checklist engine** | Repeating operational checklists (daily, weekly, monthly) |
| **MECA benchmark** | REACTOR / SCT benchmark tracking and analytics |
| **Monthly planning** | Monthly plan batches and day-to-day execution tasks |
| **Delegation engine** | One-off follow-up tasks between people |
| **Masters** | Departments, users, roles, holidays, media links |
| **Settings** | Theme, working hours/SLA rules, role permissions |

---

## 2. Logging in and signing out

| Step | What to do |
|------|------------|
| Open the app | Use the web address your IT team or admin gave you (example: `https://your-company/respro`) |
| Log in | Enter your **email** and **password**, then click **Login** |
| Log out | Top-right corner ? click your **name/photo** ? **Logout** |

If you cannot log in, contact your administrator � they manage users under **Masters ? Users**.

---

## 3. How to move around the app (navigation)

After login you see a **dark sidebar on the left** (main menu) and a **top bar** with the page title.

### Main sidebar (left)

| Menu item | What it opens |
|-----------|----------------|
| **Home** | Main dashboard with summaries |
| **Work center** | Sub-menu: FMS Task, Notifications, My profile |
| **Workflow** | Sub-menu: instances, SLA monitor, logs, design studio |
| **Checklist** | Sub-menu: checklist dashboards and tasks |
| **Benchmark** | Sub-menu: MECA benchmark pages |
| **Planning** | Sub-menu: monthly planning |
| **Delegation** | Sub-menu: delegation dashboard and tasks |
| **Masters** | Sub-menu: departments, roles, users, holidays, media |
| **Settings** | Sub-menu: theme, SLA, permissions |

**How sub-menus work**

1. Click a main item (e.g. **Work center**).
2. A second panel opens with links inside that section.
3. Click the page you need.
4. Click outside the panel or the backdrop to close it.

**Important:** If you **do not see** a main menu item (e.g. no **Checklist**), your role does not have **view** access to any page in that section. This is normal � ask your admin to adjust your role if you need access.

### Top bar (top of screen)

| Item | Purpose |
|------|---------|
| **Page title** | Shows where you are |
| **Bell icon** | Opens **Notifications** (if you have permission) |
| **Your name + photo** | Opens menu: Profile, Change Password, 2FA, **Switch Role** (if you have multiple roles), Logout |

---

## 4. Your account, photo, and roles

### My profile � view

**Path:** `/app/profile`  
**Menu:** Work center ? **My profile**

| Field | Can you change it? |
|-------|-------------------|
| Name | Yes � on **Edit profile** only |
| Email | **No** � account identifier (admin changes if needed) |
| Phone | **No** � account identifier (admin changes if needed) |
| Status | **No** � shown for information (e.g. ACTIVE) |
| Department | **No** � shown as department **name** |
| Role | **No** � shown as role **name** |
| Profile photo | Yes � on **Edit profile** only |

### Edit profile

**Path:** `/app/profile/edit`  
**Menu:** My profile ? button **Edit profile**

- Change your **display name**.
- Upload or change your **profile photo** (most image types accepted).
- Replacing a photo **deletes the old photo** from the system; other users� photos are not affected.
- Click **Save** when finished. You return to the profile view.

### Switch Role (multiple roles)

If your admin assigned more than one role:

1. Top-right ? your name ? **Switch Role**.
2. Pick the role you want to work as.
3. Menus and allowed actions update to match that role�s permissions.

Your **active role** controls what you can see and do until you switch again.

---

## 5. Permissions � why some menus are hidden

Respro uses **role-based access**. Each role has allowed actions such as **View**, **Edit**, **Create**, **Delete**, and special actions like **Mark as done**.

**In plain language:**

- **View** � you can open the page and read data.
- **Edit** � you can change existing records.
- **Create** � you can add new records.
- **Delete** � you can remove records.
- **Mark as done** (FMS tasks) � you can complete tasks and use bulk complete.

If **every** sub-page in a section is denied for your role, the **whole section disappears** from the main sidebar (same idea as a typical ERP system).

Admins configure permissions under **Settings ? Permission approval** (or **Masters ? Roles** ? edit role ? permissions).

---

## 6. Home dashboard

**Path:** `/app`  
**Menu:** **Home** (first item in sidebar)

**Who uses it:** Everyone with Home view permission.

**What you see:**

- Summary cards and charts for modules you can access (checklist, delegation, benchmark, monthly planning, FMS, etc.).
- High-level counts: pending work, overdue items, team performance where applicable.

**What to do here:** Start your day � check overall status before opening detailed task lists.

---

## 7. Work center

**Purpose:** Day-to-day work that applies to **you personally** � FMS tasks assigned to you, system notifications, and your profile.

### 7.1 FMS Task (your workflow steps)

**Path:** `/app/fms/tasks`  
**Menu:** Work center ? **FMS Task**

**What it is:** Tasks from **FMS workflows** (Flow Monitoring System) that are assigned **to you** � one step at a time in a larger process.

**Tabs:**

| Tab | Meaning |
|-----|---------|
| **Pending** | Work waiting for you |
| **Completed** | Work you already finished |
| **Overdue** | Pending work past its planned date |

**Views:**

| View | What it shows |
|------|----------------|
| **Journey** (default) | Full workflow as a **timeline** � all steps, who did each step, planned/actual dates, delay (green = on time, red = delay). Your pending steps appear with **Complete** buttons. |
| **List** | Table view � good for **selecting many tasks** and completing them together |

**Common actions:**

| Action | Permission needed | How |
|--------|-------------------|-----|
| View tasks | View | Open the page |
| Switch Journey / List | Edit | Toggle top-right |
| Complete one task | Mark as done | **Complete** on a row or journey card |
| Complete many tasks | Mark as done | List or Journey: select checkboxes ? choose outcome ? **Mark selected done** |
| Filter by FMS type | View | Dropdown **FMS** at top |

**Complete a single task (detail screen)**

**Path:** `/app/fms/tasks/{task-id}/complete`

Opens a form: outcome (Yes/No), remarks, step fields, checklist items if configured. **Save / Mark complete** requires **Mark as done** permission.

**Old path note:** `/app/my-tasks` automatically redirects to `/app/fms/tasks`.

---

### 7.2 Notifications

**Path:** `/app/notifications`  
**Menu:** Work center ? **Notifications**  
**Also:** Bell icon in top bar (if you have permission)

**What it is:** System messages � task assignments, reminders, workflow alerts, checklist and delegation notices, monthly planning reminders.

**Tabs:** FMS Task Notifications | Checklist Tasks | Delegation Tasks | Monthly Planning

**Actions:** Open a tab ? read items ? **Mark read** on one item or **Mark all read**.

---

### 7.3 My profile

See [Section 4](#4-your-account-photo-and-roles).

---

## 8. Workflow

**Purpose:** Design and run **multi-step business processes** (FMS), monitor delays (SLA), review history, and build templates in the design studio.

### 8.1 FMS Workflow instances

**Path:** `/app/fms/workflow/instances`  
**Menu:** Workflow ? **FMS Workflow instances**

**What it is:** List of **running or completed workflows** (each row is one �case� going through your defined steps).

**Typical uses:**

| Who | Action |
|-----|--------|
| Coordinator | **Start** a new workflow instance |
| Coordinator / Admin | **Edit** instance details |
| Doer | Complete steps via **FMS Task** (Work center) |
| Manager | Monitor status and references |

**Related paths:**

| Path | Purpose |
|------|---------|
| `/app/fms/workflow/instances/start` | Start a new workflow |
| `/app/fms/workflow/instances/{id}/edit` | Edit an existing instance |

**Permissions:** View, Create, Edit, Delete (per role).

---

### 8.2 FMS SLA monitor

**Path:** `/app/fms/sla-monitor`  
**Menu:** Workflow ? **FMS SLA monitor**

**What it is:** Monitor **service level / delay** � which workflow steps are on time, late, or at risk.

**Who uses it:** Coordinators and managers tracking operational performance.

**Permissions:** View, Edit.

---

### 8.3 FMS Workflow logs

**Path:** `/app/fms/workflow-logs`  
**Menu:** Workflow ? **FMS Workflow logs**

**What it is:** **Audit trail** � who did what and when on workflow instances (history for review).

**Who uses it:** Coordinators, auditors, managers investigating issues.

**Permissions:** View, Edit.

---

### 8.4 Design studio

**Path:** `/app/workflow/designer`  
**Menu:** Workflow ? **Design studio**

**What it is:** Build and maintain **workflow templates** � steps, transitions, forms, assignments, formulas. This is the **setup** side of FMS (usually admins or process owners).

**Also used for (legacy links redirect here):**

- Workflow templates list: `/app/workflow/templates`
- Form templates

**Permissions:** View, Edit, Create, Delete.

**Who uses it:** Administrators and process designers � not typical daily doers.

---

## 9. Checklist engine

**Purpose:** **Repeating** operational tasks (daily inspections, weekly checks, monthly audits) generated automatically from rules you define.

### 9.1 Dashboard (Operations hub)

**Path:** `/app/checklist`  
**Menu:** Checklist ? **Dashboard**

**What it is:** Overview of checklist operations � summaries and shortcuts into task queues and masters.

**Permissions:** View, Button view (for action buttons on the hub).

---

### 9.2 Task queue

**Path:** `/app/checklist/tasks`  
**Menu:** Checklist ? **Task queue**

**What it is:** Manage **generated checklist tasks** � approve, skip, edit, delete, bulk operations (coordinators/supervisors).

**Permissions:** View, Edit, Create, Delete, Approved, Skips.

---

### 9.3 Assignments

**Path:** `/app/checklist/assignments`  
**Menu:** Checklist ? **Assignments**

**What it is:** Assign checklist templates to users, roles, or departments. Often opened with a template selected (`?templateId=` in URL).

**Permissions:** View, Create, Update, Delete.

---

### 9.4 My checklist tasks

**Path:** `/app/checklist/my-tasks`  
**Menu:** Checklist ? **My checklist tasks**

**What it is:** **Your** checklist tasks for today / current period � complete them here as a doer.

**Permissions:** View.

---

### 9.5 Checklist masters

**Path:** `/app/checklist/masters`  
**Menu:** Checklist ? **Checklist masters**

**What it is:** Define checklist templates � name, department, priority, items, assignment rules, recurrence links.

**Permissions:** View, Create, Edit, Delete, Recurrence, Assignment.

---

### 9.6 Recurrence config

**Path:** `/app/checklist/recurrence`  
**Menu:** Checklist ? **Recurrence config**

**What it is:** Configure **when** checklists repeat (daily, weekly, monthly, etc.) and generate future tasks.

**Permissions:** View, Recurrence, Delete.

---

### 9.7 Scoreboard

**Path:** `/app/checklist/scoreboard`  
**Menu:** Checklist ? **Scoreboard**

**What it is:** **Performance view** � completion rates and scores for checklist work (teams/individuals).

**Who uses it:** Managers for reviews and recognition.

**Permissions:** View.

---

## 10. MECA benchmark

**Purpose:** Track and analyze **REACTOR SCT / MECA benchmark** data � records, stages, and executive dashboards.

### 10.1 Dashboard (Benchmark hub)

**Path:** `/app/benchmark`  
**Menu:** Benchmark ? **Dashboard**

**What it is:** Entry point and summary for the benchmark module.

**Permissions:** View, Edit.

---

### 10.2 Analytics dashboard

**Path:** `/app/benchmark/dashboard`  
**Menu:** Benchmark ? **Analytics dashboard**

**What it is:** **Executive / analytics** charts and KPIs for benchmark performance.

**Who uses it:** Managers and leadership.

**Permissions:** View.

---

### 10.3 Benchmark records

**Path:** `/app/benchmark/records`  
**Menu:** Benchmark ? **Benchmark records**

**What it is:** List and manage **benchmark data records** (often filtered by department).

**Related paths:**

| Path | Purpose |
|------|---------|
| `/app/benchmark/create` | Add new record |
| `/app/benchmark/edit/{id}` | Edit existing record |

**Permissions:** View, Edit, Create, Delete.

---

### 10.4 Stage configuration

**Path:** `/app/benchmark/stages`  
**Menu:** Benchmark ? **Stage configuration**

**What it is:** Define **stages** used in benchmark processes (master setup for stages).

**Permissions:** View, Create, Edit, Delete.

---

## 11. Monthly planning

**Purpose:** **Monthly plan batches** � plan work for a month, approve batches, and execute **daily tasks** from those plans.

### 11.1 Dashboard (Planning hub)

**Path:** `/app/monthly-planning`  
**Menu:** Planning ? **Dashboard**

**What it is:** Overview of monthly planning module and navigation into batches and tasks.

**Permissions:** View, Edit.

**Related:** Planning grid may be linked from hub actions � `/app/monthly-planning/grid` for grid-style planning view.

---

### 11.2 Plan batches

**Path:** `/app/monthly-planning/batches`  
**Menu:** Planning ? **Plan batches**

**What it is:** Create and manage **monthly plan batches** (containers for a month�s planned work).

**Related path:** `/app/monthly-planning/batches/{id}/edit` � edit one batch.

**Permissions:** View, Edit, Create, Delete, Approve.

---

### 11.3 My tasks today

**Path:** `/app/monthly-planning/my-tasks`  
**Menu:** Planning ? **My tasks today**

**What it is:** **Your** tasks for today from monthly plans � mark complete, reschedule, or skip (per permissions).

**Permissions:** View, Mark complete, Reschedule, Skip.

---

## 12. Delegation engine

**Purpose:** **One-off** tasks assigned from one person to another � follow-up, revisions, scoring (not the same as repeating checklists).

### 12.1 Dashboard (Delegation hub)

**Path:** `/app/delegation`  
**Menu:** Delegation ? **Dashboard**

**What it is:** Summary of delegation activity � pending, completed, scores overview.

**Permissions:** View, Edit.

---

### 12.2 Workspace

**Path:** `/app/delegation/workspace`  
**Menu:** Delegation ? **Workspace**

**What it is:** Main working area with **tabs** � add tasks, follow-up, pending, completed, scores, by department, revisions (tab access depends on role).

**Permissions:** View plus tab-level permissions (Tab add, Tab followup, Tab pending, etc.).

---

### 12.3 My delegation tasks

**Path:** `/app/delegation/my-tasks`  
**Menu:** Delegation ? **My delegation tasks**

**What it is:** Tasks **delegated to you** � complete or update as the assignee.

**Permissions:** Edit (used as access to this page for doers).

---

## 13. Masters (setup data)

**Purpose:** **Reference data** used across the whole app. Usually maintained by **administrators**, not daily doers.

### 13.1 Departments

**Path:** `/app/masters/departments`  
**Menu:** Masters ? **Departments**

**What it is:** Organizational units (plants, teams, divisions). Users and checklists link to departments.

**Permissions:** View, Create, Edit, Delete.

---

### 13.2 Roles

**Path:** `/app/masters/roles`  
**Menu:** Masters ? **Roles**

**What it is:** Job roles (Buyer, Manager, Operator, etc.). Used for assignment and permissions.

**Actions:** **Add role** opens permission setup at `/app/settings/permissions/add`. **Edit** opens `/app/settings/permissions/edit/{id}`.

**Permissions:** View, Create, Edit, Delete.

---

### 13.3 Users

**Path:** `/app/masters/users`  
**Menu:** Masters ? **Users**

**What it is:** User accounts � name, email, phone, department, roles, status.

**Related paths:**

| Path | Purpose |
|------|---------|
| `/app/masters/users/add` | Create user |
| `/app/masters/users/{id}/edit` | Edit user (including multiple roles) |

**Note:** Email and phone are account identifiers � users change **name and photo** only on their own profile (if allowed).

**Permissions:** View, Create, Edit, Delete.

---

### 13.4 Holidays

**Path:** `/app/masters/holidays`  
**Menu:** Masters ? **Holidays**

**What it is:** **Holiday calendar** � dates when SLA/due-date calculations should skip non-working days.

**Permissions:** View, Create, Edit, Delete.

---

### 13.5 Media master

**Path:** `/app/masters/media`  
**Menu:** Masters ? **Media master**

**What it is:** Store links to **flowcharts and training videos** (e.g. Google Drive) by department and type.

**Permissions:** View, Create, Edit, Delete.

---

## 14. Settings

**Purpose:** Application preferences and **security/permission** configuration.

### 14.1 Theme and appearance

**Path:** `/app/settings/theme`  
**Menu:** Settings ? **Theme & appearance**

**What it is:** Personalize colors, font, and font size (saved to your user account).

**Permissions:** View.

---

### 14.2 SLA and working hours

**Path:** `/app/settings/sla`  
**Menu:** Settings ? **SLA & hours**

**What it is:** Configure **working hours** and SLA rules used when calculating due dates and delays.

**Permissions:** View, Edit.

---

### 14.3 Permission approval (role permissions)

**Path:** `/app/settings/permissions`  
**Menu:** Settings ? **Permission approval**

**What it is:** List of roles and their **permission sets** � which pages and actions each role may use.

**Related paths:**

| Path | Purpose |
|------|---------|
| `/app/settings/permissions/add` | Create role with permissions |
| `/app/settings/permissions/edit/{id}` | Edit role permissions |

**Who uses it:** Administrators only.

**Permissions:** Tied to Masters Roles view access.

---

## 15. Which tool to use for which job

| If your work is� | Use this module |
|------------------|-----------------|
| A **repeating** daily/weekly/monthly task | **Checklist engine** |
| A **multi-step process** with approvals and handoffs | **Workflow (FMS)** + complete steps in **FMS Task** |
| A **one-off** �please do this by Friday� assignment | **Delegation engine** |
| **Monthly** planned work broken into daily tasks | **Monthly planning** |
| **Benchmark / REACTOR** data entry and reports | **MECA benchmark** |
| Setting up **teams, users, holidays** | **Masters** |
| Changing **who can see which menu** | **Settings ? Permission approval** |

---

## 16. Complete path reference (quick lookup)

All paths start after login. Base URL is your server + `/app`.

### Login

| Path | Page |
|------|------|
| `/login` | Login screen |

### Home

| Path | Page |
|------|------|
| `/app` | Home dashboard |

### Work center

| Path | Page |
|------|------|
| `/app/fms/tasks` | FMS Task (my tasks) |
| `/app/fms/tasks/{id}/complete` | Complete one FMS task |
| `/app/notifications` | Notifications |
| `/app/profile` | My profile (view) |
| `/app/profile/edit` | Edit profile (name + photo) |

### Workflow

| Path | Page |
|------|------|
| `/app/fms/workflow/instances` | Workflow instances list |
| `/app/fms/workflow/instances/start` | Start workflow |
| `/app/fms/workflow/instances/{id}/edit` | Edit instance |
| `/app/fms/sla-monitor` | SLA monitor |
| `/app/fms/workflow-logs` | Workflow logs |
| `/app/workflow/designer` | Design studio |
| `/app/workflow/templates` | Templates (redirects to designer) |

### Checklist

| Path | Page |
|------|------|
| `/app/checklist` | Checklist dashboard |
| `/app/checklist/tasks` | Task queue |
| `/app/checklist/assignments` | Assignments |
| `/app/checklist/my-tasks` | My checklist tasks |
| `/app/checklist/masters` | Checklist masters |
| `/app/checklist/recurrence` | Recurrence config |
| `/app/checklist/scoreboard` | Scoreboard |

### MECA benchmark

| Path | Page |
|------|------|
| `/app/benchmark` | Benchmark hub |
| `/app/benchmark/dashboard` | Analytics dashboard |
| `/app/benchmark/records` | Benchmark records |
| `/app/benchmark/create` | New record |
| `/app/benchmark/edit/{id}` | Edit record |
| `/app/benchmark/stages` | Stage configuration |

### Monthly planning

| Path | Page |
|------|------|
| `/app/monthly-planning` | Planning hub |
| `/app/monthly-planning/grid` | Planning grid |
| `/app/monthly-planning/batches` | Plan batches |
| `/app/monthly-planning/batches/{id}/edit` | Edit batch |
| `/app/monthly-planning/my-tasks` | My tasks today |

### Delegation

| Path | Page |
|------|------|
| `/app/delegation` | Delegation hub |
| `/app/delegation/workspace` | Delegation workspace |
| `/app/delegation/my-tasks` | My delegation tasks |

### Masters

| Path | Page |
|------|------|
| `/app/masters/departments` | Departments |
| `/app/masters/roles` | Roles |
| `/app/masters/users` | Users |
| `/app/masters/users/add` | Add user |
| `/app/masters/users/{id}/edit` | Edit user |
| `/app/masters/holidays` | Holidays |
| `/app/masters/media` | Media master |

### Settings

| Path | Page |
|------|------|
| `/app/settings/theme` | Theme & appearance |
| `/app/settings/sla` | SLA & working hours |
| `/app/settings/permissions` | Permission approval (roles) |
| `/app/settings/permissions/add` | Add role |
| `/app/settings/permissions/edit/{id}` | Edit role permissions |

---

## Role quick guide (who does what)

| Role type | Typical daily pages |
|-----------|---------------------|
| **Doer** | Home, FMS Task, My checklist tasks, My delegation tasks, My tasks today, Notifications, My profile |
| **Coordinator** | Above + Workflow instances, Checklist task queue, Delegation workspace |
| **Manager** | Above + SLA monitor, Scoreboard, Analytics dashboard, dashboards |
| **Admin** | Masters, Design studio, Settings, Permission approval, all setup screens |

---

## Tips for a smooth day

1. **Start at Home** � see what needs attention.
2. **Open FMS Task** (Journey view) � understand where each workflow stands before completing steps.
3. **Check Notifications** � do not miss new assignments.
4. **Use List view** on FMS Task when you need to complete several similar tasks at once.
5. **Switch role** if you wear multiple hats (e.g. Operator vs Supervisor).
6. **Update your profile photo and name** on Edit profile so teammates recognize you in the top bar.
7. If a menu is missing, ask admin for the correct **role** and **permissions** � do not share passwords.

---

## Support

For access problems, wrong department, or role changes ? contact your **Respro administrator** (Users / Roles under Masters).

For process questions (which checklist or workflow to use) ? contact your **coordinator or line manager**.

---

*End of Master User Guide � Respro Dashboard*
