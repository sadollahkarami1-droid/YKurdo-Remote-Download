# YKurdo Remote Linux 1.3.0-beta.1

اولین انتشار آزمایشی به‌روز لینوکس، با دو بسته جداگانه **Personal** و **Commercial** و مسیر نصب و میان‌بر مستقل. برای هر نسخه فایل Ubuntu/Debian `.deb` و آرشیو نصب بدون مدیر `.tar.gz` ارائه می‌شود. Node 24.20.0 و ripgrep 14.1.0 با هش ثابت داخل بسته‌اند.

- Personal: موتور مشترک ۲۶ ابزار محلی MCP، اتصال کلاینت‌های سازگار، پوشه‌های مجاز و کلیدهای مستقل ابزار؛ تا انتخاب پوشه، دسترسی فایل بسته است.
- Commercial: اتصال به ۳۱ ابزار اصلی سرویس، موتور واقعی دستگاه برای ۲۶ ابزار، ورود ایمیل و مسیر Google، نقش Owner معتبر سروری و اشتراک/آزمایشی مشتریان؛ سه حالت فقط‌خواندنی/با تأیید/تمام‌خودکار، بازه اجرای ۱۵ دقیقه‌ای و پوشه‌های مستقل تجاری.
- مجوز محلی و سرور، حساب/دستگاه و اجاره فرمان، رد تأیید و انقضا بررسی می‌شوند. انتخاب Full Auto پرداخت یا مجوز سرور را دور نمی‌زند. قطع اتصال راه‌دور تأیید جداگانه می‌خواهد.
- نصب هیچ سرویس، حساب یا دسترسی راه‌دوری را خودکار فعال نمی‌کند. خروج از حساب و توقف پنل، موتور و گروه پردازش محلی را متوقف می‌کند.

آزمون‌ها: ۱۰ آزمون Linux روی Ubuntu 24.04 در WSL2؛ سرور واقعی برنامه با DB موقت و موتور واقعی خواندن/نوشتن/ویرایش/پردازش؛ کشف ۳۱ ابزار، رد نوشتن در Read Only، رعایت رد تأیید، پنجره اجرا، مسیر نامجاز، مجوز لغوشده، جلوگیری از انتقال متغیر محرمانه، کنترل Host/Origin/token، جداسازی دو نسخه و callback مصنوعی Google با PKCE/state. هر دو آرشیو در HOME موقت نصب و تست شدند؛ هر دو `.deb` استخراج و موتورشان بررسی شد؛ آزمون انتهابه‌انتهای تجاری با خود کد و Node داخل بسته نیز اجرا شد.

**دامنه تأیید:** Ubuntu 24.04 x64 در WSL2. ورود Google با حساب واقعی روی دسکتاپ Linux، بار چند کاربر و اجرای طولانی هنوز تأیید نشده‌اند. PDF از Markdown به Chrome/Chromium نیاز دارد. Google Drive نسخه ویندوز و رابط WPF در این انتشار منتقل نشده‌اند. نشست Linux با مجوز فایل خصوصی نگهداری می‌شود و هنوز مخزن کلید سیستم‌عامل ندارد. دستورهای شل مجازشده در sandbox سیستم‌عامل نیستند. تصاویر پنل با داده نمونه رندر شده‌اند.

هیچ سرور تولیدی، DB، داده پرداخت یا نصب فعال ویندوز در این انتشار تغییر نکرد. macOS فاز بعدی است و بسته مک هنوز ساخته/تأیید نشده است. [راهنمای نصب](LINUX-INSTALL-FA.md) را بخوانید و فایل‌ها را با SHA256SUMS همراه انتشار بررسی کنید.

## English

Separate Personal and Commercial Linux x64 beta packages, each as `.deb` and per-user `.tar.gz`, with bundled checksum-pinned Node 24.20.0 and ripgrep 14.1.0. Commercial uses the existing authenticated service and all 31 canonical tools (26 shared-engine device tools plus five service-management tools). Read Only/Ask/Full Auto, independent approved folders, local/server execution windows, tool ACLs, account/device/lease authorization and separate shutdown consent remain enforced. Personal is a separate local MCP product.

Validated on Ubuntu 24.04 in WSL2: 10 Linux tests, isolated real-service/real-engine integration, Google callback/PKCE with synthetic data, both per-user installations, both extracted Debian payloads, and Commercial integration using the actual packaged client/runtime. No live Google account login, broad desktop-distribution testing or long-duration/multi-user load claim. PDF rendering requires installed Chrome/Chromium. Credentials use private Linux files, not an OS keychain yet. Shell commands are not OS-sandboxed. Screenshots use sample data. No production server, payment DB or existing Windows install changes. macOS remains the next phase.

Private source revision: `1f144b0fe2aae5cd52ed92b0ea05c8d8f7c4a614`
