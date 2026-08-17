## Igor — Product Manager, AdTech · Berlin

I work on programmatic advertising by day and ship my own Android apps by night. In both, my job is the
same: decide what gets built and what "done" means. I write the specs, the review gates, and the
decision records; AI coding agents write the implementation; I own the release.

---

### 🧭 How I build

**[shipping-with-agents](https://github.com/garregusev/shipping-with-agents)** — the working agreement I
ended up with after two shipped apps. Prompts as the unit of work, acceptance written by the reviewer
rather than the executor, handover docs that survive context loss, and a review rubric where every rule
maps to a defect that actually reached production.

Design session picks the approach and writes the prompt → executor session writes code and tests and
stops → design session reviews and accepts. Separating who proposes from who accepts is most of the
value.

### 📱 Shipped

- **[Catudoku: Cat Sudoku Puzzle](https://play.google.com/store/apps/details?id=com.catudoku.app)** —
  cozy cat-themed Sudoku. Flutter. Live on Google Play, grown through ASO, monetized through ad
  mediation. [Case study](https://github.com/garregusev/shipping-with-agents/blob/main/case-studies/catudoku.md)
  — including the month the eCPM "broke" and why fixing it would have been a mistake.
- **SnipShot** — area and scrolling screenshots for Android. Native Kotlin, capture via
  AccessibilityService instead of MediaProjection so there's no consent dialog on every shot.
  [Case study](https://github.com/garregusev/shipping-with-agents/blob/main/case-studies/snipshot.md).
- **[sms-to-telegram](https://github.com/garregusev/sms-to-telegram)** — forwards incoming SMS to a
  Telegram chat. Kotlin, BroadcastReceiver plus a WorkManager catch-up pass.

### 🛠 Where I work

Projects run on Flutter and native Kotlin, with a Python/Postgres backend.

| | |
|---|---|
| **AdTech — day job** | OpenRTB 2.6 · programmatic/RTB targeting · supply and demand side mechanics |
| **AdTech — my apps** | ad mediation & eCPM diagnostics · app-ads.txt · ASO · product analytics |
| **Working with agents** | Claude Code · MCP · spec-driven development · decision records · agent workflow & review design |

### 📊 A thing I believe

Agents are fast and confident, so the expensive failure isn't bad code — it's plausible code nobody
checked against what it was supposed to do. Most of my process is turning "someone should check that"
into a step that can't be skipped.
