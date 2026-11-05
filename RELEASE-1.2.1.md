# Commercial 1.2.1 — حالت دسترسی هوش مصنوعی روی صفحه اصلی

برای مالک و مشتریان، سه حالت فقط‌خواندنی (Read Only)، با تأیید (Ask) و تمام‌خودکار (Full Auto) به صفحه اصلی نسخه تجاری اضافه شد. فقط یک حالت فعال می‌ماند. انتخاب حالت در خود دستگاه انجام می‌شود؛ Full Auto تأیید اولیه می‌خواهد. حالت انتخابی با خروج از حساب یا اجرای دوباره برنامه به فقط‌خواندنی برمی‌گردد. برای تغییر حالت، اتصال را متوقف کنید.

مجوز مستقل ابزارها، پوشه‌های مجاز، پنجره اجرای دستور، احراز هویت و کنترل اشتراک/دستگاه/مجوز/نشست سمت سرور حفظ می‌شوند. قطع اتصال Remote همچنان تأیید جداگانه می‌خواهد. این به‌روزرسانی داده‌های پرداخت یا پایگاه‌داده را تغییر نمی‌دهد. نسخه شخصی همچنان 1.2.0 است.

آزمون نسخه بسته‌بندی‌شده تجاری، حالت‌های دسترسی و صف فرمان، اندازه‌های مختلف صفحه، ورود و نشست و اتصال و قطع اتصال، و موتور واقعی خواندن/نوشتن/پردازش روی داده‌های موقت موفق بود. حالت فقط‌خواندنی نوشتن را رد کرد و محتوای فایل بدون تغییر ماند. Full Auto نتوانست کنترل مجوز سرور یا بسته‌بودن پنجره اجرا را دور بزند. پیش‌نمایش صفحه نیز بررسی شد.

برای دریافت تغییرات، نصب‌کننده جدید Commercial را نصب کنید؛ نصب فعال شما خودکار جایگزین نشده است. نصب‌کننده فعلاً امضای Authenticode ندارد؛ فایل SHA-256 برای بررسی همراه آن است.

## English

Commercial 1.2.1 adds an exclusive Read Only / Ask / Full Auto card on Home for Owner and customers. Read Only is the restart/logout default. Ask honors per-call consent; locally opted-in Full Auto skips individual tool prompts. Disconnect before changing mode. Tool permissions, approved folders, execution windows, server entitlement, device/ACL/lease authorization and separate shutdown consent remain enforced. No server, database or payment changes. Personal remains 1.2.0.

Packaged Commercial UI/security regressions and queued-policy checks passed. The actual shared engine passed isolated real-file read/write/process tests, including blocked Read Only writes with unchanged file contents. Rendered Home reviewed. The installer is currently unsigned; verify the attached SHA-256. Install Commercial 1.2.1 to apply this client update.

Source revision: 89672b94765a04879e90286bdbf8b2d97987a90c
