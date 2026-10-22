# Starting an FG-TIDA Working Group Charter

This guide explains how an FG-TIDA Working Group (WG) creates, maintains and publishes its charter using the FG-TIDA Working Group Charter template.

No prior Sphinx or reStructuredText experience is required. Working Group editors update the charter source files in GitHub, and the web version and PDF are generated automatically.

---

## 1. Purpose of a Working Group Charter

An FG-TIDA Working Group Charter defines the mandate of a Working Group.

It describes:

- the problem the Working Group is expected to address;
- the goals of the Working Group;
- what is in scope and what is explicitly out of scope;
- the deliverables the Working Group intends to produce;
- the expected milestones;
- dependencies and coordination with other groups;
- the criteria for completing the chartered work.

The charter is a scope and delivery agreement. It is not intended to be a tutorial, technical specification, research paper or detailed description of the solution.

A final charter should normally remain concise:

- approximately **600–1,200 words**;
- generally **one to two pages**, excluding administrative tables where appropriate.

---

## 2. FG-TIDA Charter Repository Model

The GitHub organization is:

`FG-TIDA`

The Working Group Charter template repository is:

`FG-TIDA/wg-charter-template`

Each Working Group should normally maintain one charter repository created from this template.

For example:

```text
wg1-charter
wg2-charter
wg-agent-identity-charter
wg-trust-framework-charter
```

The exact repository naming convention may be adjusted by the FG-TIDA management team, but names should remain short, predictable and clearly associated with the relevant Working Group.

Each charter repository provides:

- the editable charter source;
- version history through Git;
- Pull Request review;
- an automatically generated HTML publication;
- an automatically generated PDF;
- an issue tracker for charter-related discussion;
- synchronization to the corresponding FG-TIDA GitLab repository where configured.

---

## 3. Create a New Working Group Charter

A new Working Group should create its charter repository from the official template.

### Step 1 — Open the template

Go to:

`https://github.com/FG-TIDA/wg-charter-template`

### Step 2 — Create the repository

Click:

**Use this template → Create a new repository**

Set:

**Owner**

`FG-TIDA`

**Repository name**

Use the agreed Working Group naming convention, for example:

`wg1-charter`

or:

`wg-trust-framework-charter`

Set the repository visibility according to FG-TIDA policy.

Then click:

**Create repository**

### Step 3 — Enable GitHub Pages

In the new repository, go to:

**Settings → Pages**

Under **Build and deployment**, set:

**Source → GitHub Actions**

No additional Save button is normally required.

### Step 4 — Verify the initial build

Go to:

**Actions → Build and deploy docs**

Run the workflow if necessary.

A successful run should complete both:

```text
Build
Deploy
```

The published charter site will normally be available at:

```text
https://fg-tida.github.io/<repository-name>/
```

The downloadable PDF is published as:

```text
wg-charter.pdf
```

For example:

```text
https://fg-tida.github.io/wg1-charter/wg-charter.pdf
```

---

## 4. Main Files to Edit

Most Working Group editors only need to work with two files:

```text
src/doc/index.rst
src/doc/conf.py
```

The build infrastructure should normally not be modified by Working Group authors.

---

## 5. Complete the Charter in `src/doc/index.rst`

The actual Working Group Charter is contained in:

```text
src/doc/index.rst
```

The template contains all mandatory and optional charter sections.

These include:

1. Group Information
2. Background and Problem Statement
3. Goals
4. Scope and Non-Goals
5. Programme of Work and Deliverables
6. Milestones
7. Coordination,
