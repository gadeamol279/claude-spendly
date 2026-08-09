# Claude Code prompts — claude-spendly-az

A running log of the prompts used with Claude Code to build this project.
Kept here so the team has a record of what changed, why, and which files
were touched. Add a new entry every time a prompt is run against this repo.

---

## 2026-08-09 — Add Terms and Privacy links to footer

**Goal:** Add two placeholder footer links ("Terms and conditions",
"Privacy policy") to the shared footer. Routes are stubs for now — the
actual pages come later.

**Files touched:** `app.py`, `templates/base.html`, `static/css/style.css`

**Prompt used:**

```text
Add two placeholder footer links — "Terms and conditions" and "Privacy policy" — to the Spendly footer.

1. app.py — add two new routes, /terms and /privacy, each returning a plain
   placeholder string (e.g. "Terms and Conditions — coming soon"), matching
   the existing stub pattern already used for /logout and /profile. Do not
   create templates for these yet.

2. templates/base.html — inside the existing <footer>, add a .footer-links
   div containing the two links. Use url_for('terms') and url_for('privacy')
   for the hrefs (not hardcoded paths), so the links work on every page that
   extends this layout.

3. static/css/style.css — add minimal .footer-links and .footer-links a
   styles consistent with the existing .footer-copy rule (0.8rem font-size,
   --ink-faint color, hover to --paper).

Keep the diff minimal: no new dependencies, no real Terms/Privacy page
content yet — just the links and their placeholder targets.
```

**Commit message:**

```
Add Terms and conditions and Privacy policy links to footer
```

---

## Template — copy this for the next entry

## YYYY-MM-DD — <short title>

**Goal:** <one line on what changed and why>

**Files touched:** `<file1>`, `<file2>`

**Prompt used:**

```text
<paste the exact prompt text here>
```

**Commit message:**

```
<commit subject line>
```
