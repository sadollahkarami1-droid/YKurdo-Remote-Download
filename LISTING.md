# Directory listing text (draft for the developer portal)

**Name (≤100):** YKurdo Remote

**One-liner (≤200):** Let Claude work inside folders on your Windows PC — with a confirmation dialog for every action and a switch for every tool.

**Description (≤2000):**
YKurdo Remote connects Claude to your own Windows PC through a small desktop app. You choose which folders the assistant may use and switch tools on or off one by one (all off by default).

What Claude can do once you allow it: list, read and search files in approved folders; create and edit text files (an automatic backup is made first); run read-only git commands; and, only during a time-limited execution window that you open yourself, run PowerShell commands.

You stay in control: every request appears in a confirmation dialog on your screen, showing the exact action and path. If you do not approve within 60 seconds, it is rejected. Nothing runs when the app is closed.

Requirements: a Windows PC with the YKurdo Remote app installed (free download), and a YKurdo account. Free plan: 5,000 tool calls over 30 days, once per device. Paid plan: €19.99/month or €210/year via Stripe.

**Categories:** Developer tools; Productivity

**Documentation URL:** (the public repository README/DOCS page)
**Privacy policy URL:** (PRIVACY.md in the public repository, or the website privacy page)
**Support contact:** sadollahkarami1@gmail.com

**Use cases:** read and summarize local documents; refactor or generate code files in a project folder; inspect a git repository; guided PC maintenance (with exec window).
**Before connecting users need:** the Windows app installed and an account.
**Data access:** reads and writes (user-confirmed).

**Test & launch note for reviewers:** create a reviewer account, install the app, add one test folder, press Connect, and call each tool; the app shows a confirmation dialog for each request.
