# YKurdo Remote — directory listing (Claude and ChatGPT)

Version: Windows Commercial **1.2.6** · Updated: 10 November 2026

## Basics

| Field | Value |
|---|---|
| **Name** | YKurdo Remote |
| **Tagline** | Let Claude or ChatGPT work with the folders you approve on your own Windows PC. |
| **Category** | Productivity / Developer tools |
| **Connector URL** | `https://ykurdo-api.sdigital.app/mcp` |
| **Transport** | Streamable HTTP |
| **Authentication** | OAuth 2.1: authorization code + PKCE (S256), dynamic client registration, protected-resource metadata at `/.well-known/oauth-protected-resource` |
| **Website** | https://ydesktopcommander.win |
| **Download** | https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/latest |
| **Privacy policy** | https://ydesktopcommander.win/privacy · detailed: [PRIVACY.md](PRIVACY.md) |
| **Terms / data processing** | https://ydesktopcommander.win/terms · https://ydesktopcommander.win/refunds |
| **Support** | sadollahkarami1@gmail.com · +39 320 292 9709 |
| **Publisher** | Sadollah Karami, Via Nizza 205, 10126 Torino (TO), Italy |

## Short description

YKurdo Remote connects your AI assistant to your own Windows computer. You choose which folders it may use; it can then read, search, write and organize files, create PDFs and, only if you allow it, run commands. Read-only is the default and every sensitive action needs your approval.

## Long description

YKurdo Remote is a Windows desktop app plus a remote MCP connector. After you sign in to the app on your PC and choose approved folders, Claude or ChatGPT can work with those folders through 31 tools:

- **Files:** read, list, inspect, write, edit, move and create folders; create PDFs.
- **Search:** search file names and contents in approved folders.
- **Processes:** start and talk to command sessions, list and stop processes — only inside a short execution window the owner opens locally.
- **Account and devices:** see which account and devices are connected, review recent remote calls and fetch long-running results.

**You stay in control.** Access is limited to the folders you approve. The app starts in *Read Only*; *Ask* shows a native prompt on your PC for every action; *Full Auto* can only be switched on locally and is reset to Read Only after restart or sign-out. The assistant cannot grant itself folders or change security settings. Account, device and permission checks run on the server before every call and again before results are delivered. Turning Remote off in the app stops all remote work immediately.

**Pricing.** Every new account gets a free trial of 5,000 credits for 30 days (once per computer, no card needed). After that, a subscription is €19.99 per month or €210 per year (tax included), bought on our website with Stripe. Nothing is sold inside Claude or ChatGPT; the connector only signs in to the account you already have.

## Tools (31) and annotations

Every tool declares `readOnlyHint` or `destructiveHint` and a title.

| Group | Read-only | Changes data (destructive) |
|---|---|---|
| Files | `read_file`, `read_multiple_files`, `list_directory`, `get_file_info` | `write_file`, `edit_block`, `create_directory`, `move_file`, `write_pdf` |
| Search | `start_search`, `get_more_search_results`, `list_searches`, `stop_search` | — |
| Processes | `read_process_output`, `list_sessions`, `list_processes` | `start_process`, `interact_with_process`, `force_terminate`, `kill_process` |
| Settings | `get_config` | `set_config_value` |
| Usage | `workspace_summary`, `get_usage_stats`, `get_recent_tool_calls`, `send_feedback` | — |
| Account and devices | `list_devices`, `who_am_i`, `list_remote_tool_calls`, `get_tool_result` | `shutdown` |

## Data handling

- File contents and command output pass through our server only to deliver the request; remote call results are deleted after 7 days, call records after 90 days.
- No advertising, no sale of data. Payments are handled by Stripe; we never see card data.
- Hosting in the EU. Controller under the GDPR: Sadollah Karami (contact above).

## Reviewer instructions

No special test account is needed: the free trial starts automatically for every new account.

1. Use a **Windows 10/11 x64** computer or virtual machine (please use a disposable one; the app works on the computer it is installed on).
2. Download the latest installer from the download link above and install it. The installer is not yet Authenticode-signed, so Windows SmartScreen may ask for confirmation ("More info" → "Run anyway"); the SHA-256 is listed on the release page.
3. Open the app, create an account with an e-mail address and verify it with the code sent by e-mail. The 30-day trial with 5,000 credits starts automatically.
4. In the app, approve one **test folder** with a few sample files (no personal data), then turn **Remote** on. Leave the mode on *Read Only* for read tests; switch to *Ask* locally to test writing.
5. In Claude: Settings → Connectors → Add custom connector → paste `https://ykurdo-api.sdigital.app/mcp` → sign in with the same account. In ChatGPT: Settings → Connectors (Developer mode) → Create → paste the address → Authentication: OAuth → sign in.

**Test prompts**

1. "Which YKurdo account am I signed in to, and which devices are connected?"
2. "List the files in my approved test folder."
3. "Read notes.txt in the test folder and summarize it."
4. "Search the test folder for the word 'invoice'."
5. "Save that summary as summary.md in the test folder." *(Ask mode shows an approval prompt on the PC.)*
6. "Create a PDF from summary.md."

**To finish:** turn Remote off in the app or remove the connector; access ends immediately.

## Known limits

- Windows x64 only for this listing (a Linux build is in beta).
- The PC must be on, signed in to the app, with Remote turned on; otherwise tools report that the device is offline.
- Long-running operations return a `call_id`; fetch the result with `get_tool_result`.
