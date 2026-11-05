# YKurdo Remote — Documentation

YKurdo Remote connects Claude (or another MCP client) to folders on your Windows PC. Everything runs through a confirmation dialog that you control.

## Setup (≈ 3 minutes)
1. Download and run the installer from [Releases](../../releases). The installer is not code-signed yet: Windows may show SmartScreen — choose **More info → Run anyway** and compare the SHA-256 with the `.sha256` file.
2. Open the app, register or sign in (email verification code), then press **Connect**.
3. Add the folders the assistant may use, and turn on only the tools you want (all tools are off by default).
4. In Claude: **Settings → Connectors → Add custom connector**, paste `https://ykurdo-api.sdigital.app/mcp`, and sign in with the same account.

## Tools
| Tool | What it does | Needs your confirmation |
|---|---|---|
| `device_fs_list` | List entries of an approved folder | Yes |
| `device_fs_read` | Read a UTF-8 text file (up to 64 KiB per call) | Yes |
| `device_fs_search` | Search file names/contents in an approved folder | Yes |
| `device_fs_write` | Create/overwrite a text file (up to 48 KiB, existing file backed up first, executables refused) | Yes |
| `device_fs_edit` | Replace exactly one occurrence of text in a file (backup first) | Yes |
| `device_git` | Read-only git: status, log, diff, branch | Yes |
| `device_exec`, `device_process_list`, `device_process_kill` | PowerShell commands and process control | Only while you have opened a time-limited execution window (max 60 min) in the app |

Each confirmation dialog shows the exact action and path and closes as "rejected" if you do not answer within 60 seconds.

## Plans
Free: 5,000 tool calls over 30 days, once per device. Paid: €19.99/month or €210/year (tax inclusive), processed by Stripe; cancel any time from the billing portal in the app.

## Data handling
See [PRIVACY.md](PRIVACY.md). File contents and command output pass through the service only to deliver the result of a request you approved; results are deleted after 7 days and call records after 90 days.

## Support
sadollahkarami1@gmail.com
