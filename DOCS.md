# YKurdo Remote — Commercial 1.2.1 / Personal 1.2.0 — راهنمای دو نسخه / Product guide

## انتخاب نسخه

- **Personal، شخصی غیرتجاری:** محصول مستقل شخصی، با تنظیمات خودش و بدون ورود به حساب تجاری.
- **Commercial، تجاری:** ورود به حساب، دستگاه ثبت‌شده و مجوز سرور لازم دارد. Owner دائمی است؛ مشتریان از اشتراک یا trial معتبر استفاده می‌کنند.

نصب‌کننده دو محصول جداست؛ ارتقای هرکدام، حساب یا تنظیمات محصول دیگر را منتقل نمی‌کند. برای امکانات جدید تجاری، Commercial 1.2.1 لازم است.

## فهرست مشترک ۳۱ ابزار

| گروه | ابزارها |
|---|---|
| خواندن، ۴ ابزار | `read_file`, `read_multiple_files`, `list_directory`, `get_file_info` |
| نوشتن و ویرایش، ۵ ابزار | `write_file`, `edit_block`, `create_directory`, `move_file`, `write_pdf` |
| جستجو، ۴ ابزار | `start_search`, `get_more_search_results`, `list_searches`, `stop_search` |
| ترمینال و پردازش، ۷ ابزار | `start_process`, `read_process_output`, `interact_with_process`, `list_sessions`, `list_processes`, `force_terminate`, `kill_process` |
| تنظیمات، ۲ ابزار | `get_config`, `set_config_value` |
| گزارش و تشخیص، ۴ ابزار | `workspace_summary`, `get_usage_stats`, `get_recent_tool_calls`, `give_feedback_to_desktop_commander` |
| مدیریت ریموت، ۵ ابزار | `list_devices`, `who_am_i`, `list_remote_tool_calls`, `get_tool_result`, `shutdown` |

در نسخه تجاری، ۲۶ ابزار دستگاه به موتور مشترک نسخه شخصی متصل‌اند و ۵ ابزار مدیریت از API حساب استفاده می‌کنند. حساب‌هایی که ابزارهای قدیمی را صریحاً فعال کرده‌اند، ممکن است نام‌های سازگاری بیشتری در فهرست ببینند؛ همان ۳۱ نام اصلی نیز موجودند.

## پوشه‌ها، درایوها و پنجره اجرا

در نسخه شخصی، از «افزونه‌های AI» بخش «افزونه‌ها — دسترسی ریموت» را باز کنید. پوشه یا کل درایو را اضافه کنید و کلید دسترسی هر مسیر را روشن یا خاموش کنید. افزودن کل درایو تأیید جداگانه می‌خواهد. برای ابزارهای پردازش، پنجره اجرای ۱۵ دقیقه‌ای را باز کنید؛ دکمه بستن، آن را فوراً می‌بندد. پنجره اجرا پس از خروج از برنامه فعال باقی نمی‌ماند.

در نسخه تجاری نیز پوشه‌ها و ابزارها را از داخل برنامه مدیریت کنید. حالت دسترسی روی صفحه اصلی تجاری مشخص می‌شود: فقط‌خواندنی، با تأیید یا تمام‌خودکار. حالت پیش‌فرض فقط‌خواندنی است؛ Ask برای هر ابزار تأیید می‌خواهد و Full Auto پس از انتخاب و تأیید محلی، پرسش‌های جداگانه ابزارهای مجاز را حذف می‌کند. تغییر حالت نیازمند قطع اتصال است و بازشدن دوباره برنامه یا خروج از حساب حالت فقط‌خواندنی را برمی‌گرداند. قطع اتصال Remote همچنان تأیید جداگانه می‌خواهد. مجوز سرور و مجوزهای محلی در هر سه حالت الزامی‌اند. ابزارهای پردازش به پنجره اجرای باز در خود برنامه نیز نیاز دارند. مدل نمی‌تواند پوشه‌های مجاز یا فهرست دستورات مسدود را با `set_config_value` تغییر دهد.

## اتصال Commercial

1. برنامه به‌روز را نصب کنید و با Google یا ایمیل وارد حساب شوید.
2. اتصال دستگاه را مطابق راهنمای برنامه تنظیم کنید؛ مجوز پوشه‌ها را انتخاب و دستگاه را متصل کنید.
3. کانکتور MCP را در کلاینت پشتیبانی‌شده با `https://ykurdo-api.sdigital.app/mcp` اضافه کنید و با همان حساب وارد شوید.
4. پس از ارتقا، فهرست ابزارهای کانکتور را تازه کنید. دستگاه قدیمی برای ابزارهای جدید پیام نیاز به ارتقا می‌گیرد.

برای چند دستگاه آنلاین، `device_id` را مشخص کنید. اگر یک دستگاه سازگار آنلاین باشد، انتخاب خودکار ممکن است. درخواست طولانی، `call_id` می‌دهد؛ نتیجه را با `get_tool_result` بگیرید. نشست پردازش و جستجو تا زمان اتصال موتور دستگاه حفظ می‌شود؛ خروج از حساب یا قطع اتصال، موتور و فرایندهای فرزندش را متوقف می‌کند.

## داده و نگهداری

نتایج و آرگومان‌های صف Commercial پس از ۷ روز پاک‌سازی می‌شوند؛ رکوردهای فراخوانی پس از ۹۰ روز حذف می‌شوند. نام ابزار برای کنترل مجوز و فراداده حساب تا دوره مربوط به رکورد حفظ می‌شود. [سیاست حریم خصوصی](PRIVACY.md) را نیز بخوانید.

## English

Personal and Commercial remain separate products. Commercial 1.2.1 supports the same 31 canonical tools listed above, with the same generated argument schemas and the actual shared Personal engine for device operations. Legacy tool names explicitly enabled by an existing account may remain visible for compatibility.

Install the matching updated client, configure and connect the device, choose approved folders, and refresh your MCP connector tool list. Commercial endpoint: `https://ykurdo-api.sdigital.app/mcp`. Home provides Read Only (default), Ask, and Full Auto. Ask requires per-call consent; locally selected Full Auto skips per-call prompts for permitted tools. Restart/logout resets Read Only, mode changes require disconnecting, and shutdown still requires separate consent. Server entitlement, device authorization, tool permissions and approved roots apply in all modes. Process tools also require a locally opened execution window. Long-running requests return a `call_id` for `get_tool_result`; specify `device_id` when device selection is ambiguous.

In Personal, the extensions panel includes folder/whole-drive switches and a 15-minute execution window. Disabling a folder takes effect in the shared engine without restart. Invalid or empty policy blocks access. Installers are currently not Authenticode-signed; verify downloads against their release SHA-256 files.

Support: sadollahkarami1@gmail.com

## Ø§ØªØµØ§Ù„ Ø¨Ù‡ Claude Ùˆ ChatGPT / Connect to Claude and ChatGPT

Ø¢Ø¯Ø±Ø³ Ú©Ø§Ù†Ú©ØªÙˆØ± Ø¨Ø±Ø§ÛŒ Ù‡Ø± Ø¯Ùˆ: `https://ykurdo-api.sdigital.app/mcp` (Ø§Ø­Ø±Ø§Ø² Ù‡ÙˆÛŒØª OAuthØ› Ø¨Ø§ Ù‡Ù…Ø§Ù† Ø­Ø³Ø§Ø¨ YKurdo ÙˆØ§Ø±Ø¯ Ø´ÙˆÛŒØ¯).

**Claude:** Settings â†’ Connectors â†’ Add custom connector â†’ Ø¢Ø¯Ø±Ø³ Ø¨Ø§Ù„Ø§ Ø±Ø§ Ø¨Ú†Ø³Ø¨Ø§Ù†ÛŒØ¯ â†’ Ø¨Ø§ Ø­Ø³Ø§Ø¨ YKurdo ÙˆØ§Ø±Ø¯ Ø´ÙˆÛŒØ¯.

**ChatGPT:** Settings â†’ Connectors â†’ Advanced â†’ Developer mode Ø±Ø§ Ø±ÙˆØ´Ù† Ú©Ù†ÛŒØ¯ â†’ Create â†’ Ù†Ø§Ù… `YKurdo Remote`ØŒ Ø¢Ø¯Ø±Ø³ Ø¨Ø§Ù„Ø§ØŒ Authentication: OAuth â†’ Ø¨Ø§ Ø­Ø³Ø§Ø¨ YKurdo ÙˆØ§Ø±Ø¯ Ø´ÙˆÛŒØ¯. Ø³Ù¾Ø³ Ø¯Ø± ÛŒÚ© Ú†ØªØŒ Ú©Ø§Ù†Ú©ØªÙˆØ± Ø±Ø§ ÙØ¹Ø§Ù„ Ú©Ù†ÛŒØ¯.

Ø´Ø±Ø§ÛŒØ·: Ø¨Ø±Ù†Ø§Ù…Ù‡ Ø±ÙˆÛŒ ÙˆÛŒÙ†Ø¯ÙˆØ² Ù†ØµØ¨ Ùˆ ÙˆØ§Ø±Ø¯ Ø­Ø³Ø§Ø¨ Ø¨Ø§Ø´Ø¯ØŒ Ø­Ø¯Ø§Ù‚Ù„ ÛŒÚ© Ù¾ÙˆØ´Ù‡Ù” Ù…Ø¬Ø§Ø² Ø§Ù†ØªØ®Ø§Ø¨ Ø´Ø¯Ù‡ Ùˆ Remote Ø±ÙˆØ´Ù† Ø¨Ø§Ø´Ø¯. Ø­Ø§Ù„Øª Ù¾ÛŒØ´â€ŒÙØ±Ø¶ ÙÙ‚Ø·â€ŒØ®ÙˆØ§Ù†Ø¯Ù†ÛŒ Ø§Ø³Øª. Ø¨Ø±Ø§ÛŒ Ù‚Ø·Ø¹ Ø¯Ø³ØªØ±Ø³ÛŒØŒ Remote Ø±Ø§ Ø¯Ø± Ø¨Ø±Ù†Ø§Ù…Ù‡ Ø®Ø§Ù…ÙˆØ´ Ú©Ù†ÛŒØ¯ ÛŒØ§ Ú©Ø§Ù†Ú©ØªÙˆØ± Ø±Ø§ Ø­Ø°Ù Ú©Ù†ÛŒØ¯.

**English:** In Claude: Settings > Connectors > Add custom connector. In ChatGPT: Settings > Connectors > Advanced > Developer mode > Create, Authentication = OAuth. Use `https://ykurdo-api.sdigital.app/mcp` and sign in with your YKurdo account. The Windows app must be signed in with Remote on and at least one approved folder; the default mode is Read Only.

## Linux beta

دو بسته مستقل Linux Personal و Commercial برای Ubuntu 24.04 x64 آماده است؛ [راهنمای Linux](LINUX-INSTALL-FA.md) و [توضیحات انتشار آزمایشی](LINUX-1.3.0-beta.1.md) را بخوانید. macOS هنوز منتشر نشده است.
