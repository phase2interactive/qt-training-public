## 2026-11-09 11:31 CST · pass-2

**Prompt:**
Read requirements.md. Interview me about anything unclear, then write a spec to spec.md that covers every acceptance criterion.

**Summary:** Interviewed the user (stack: .NET Minimal API + static JS + SQLite; /kitchen without login; New→Ready only; polling; qty 1–20; cart in localStorage) and wrote spec.md with domain model, API, UI, persistence, AC traceability table, and test plan. Files: spec.md, prompt-log.md.

## 2026-11-09 11:43 CST · pass-2

**Prompt:**
open spec.md in vscode so i can see it

**Summary:** Opened spec.md in VS Code. No code changes; only prompt-log.md updated.

## 2026-11-09 11:51 CST · pass-2

**Prompt:**
Build the app from spec.md. Check it against every acceptance criterion in requirements.md when you're done.

**Summary:** Built the Neighborhood Pizza app (.NET 10 Minimal API, EF Core SQLite, static HTML/JS customer and kitchen pages) plus 46 xUnit tests, all passing; verified every AC in the browser, including kitchen polling and persistence across a server restart. Files: NeighborhoodPizza.slnx, dotnet-tools.json, src/NeighborhoodPizza/**, tests/NeighborhoodPizza.Tests/**, spec.md (.NET 10 and DateTime notes, run instructions), prompt-log.md.

## 2026-11-09 11:57 CST · pass-2

**Prompt:**
run it and open both the customer and kitchen views in my browser

**Summary:** Started the app on http://localhost:5268 in the background and opened the customer (/) and kitchen (/kitchen) pages in the default browser. No code changes; only prompt-log.md updated.

## 2026-11-09 11:58 CST · pass-2

**Prompt:**
ok stop the app

**Summary:** Stopped the running app on port 5268. No code changes; only prompt-log.md updated.

## 2026-11-09 12:00 CST · pass-2

**Prompt:**
ok open a pr for this branch to main and also open a pr for this back into the forked repo

**Summary:** Opened PR #2 from pass-2 into main on the fork (shwilliamson/qt-training-public-stuart) and draft PR #2 "Stuart Williamson - Pass 2" into phase2interactive/qt-training-public main. Only prompt-log.md changed.

## 2026-11-09 12:01 CST · pass-2

**Prompt:**
open both of these in my browser

**Summary:** Opened the fork PR #2 and the upstream draft PR #2 in the default browser. Only prompt-log.md changed.

## 2026-11-09 12:38 CST · pass-3

**Prompt:**
Use Playwright to check that section 2 of requirements.md (Reviewing an Order) works in the running app. Fix anything that fails.

**Summary:** Ran Playwright checks for AC-2.1–2.3. All functional checks passed, but keyboard focus was lost after +/−/Remove and after typing a quantity, and browsers cached stale JS. Fixed both: order.js updates quantities in place and restores focus, labels now name size and toppings, and Program.cs sends Cache-Control: no-cache. Added 5 cache tests (51 total passing); all 23 Playwright checks pass. Files: order.js, index.html, Program.cs, OrderApiTests.cs, spec.md, prompt-log.md.

## 2026-11-09 13:44 CST · pass-3

**Prompt:**
ok, open a pr for this branch both in this repo and in the forked repo

**Summary:** Opened PR #3 from pass-3 into main on the fork (shwilliamson/qt-training-public-stuart) and draft PR #3 "Stuart Williamson - Pass 3" into phase2interactive/qt-training-public main. Only prompt-log.md changed.

## 2026-11-09 13:59 CST · pass-4

**Prompt:**
! git checkout -b pass-4

**Summary:** User created the pass-4 branch from pass-3. No changes besides this log entry.


## 2026-11-09 14:08 · pass-4

**Prompt:**
You are a tester. Do not change code. Use Playwright to check section 3 of requirements.md (Placing an Order) against the running app. Report each acceptance criterion as pass or fail, with steps to reproduce.

**Summary:** Ran the app against a scratch database and tested AC-3.1 to AC-3.3 with Playwright plus direct API calls. All three passed. No code changed; only prompt-log.md was updated.
