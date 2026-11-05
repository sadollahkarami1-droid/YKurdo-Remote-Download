# YKurdo Remote 1.2.0

دو نسخه مستقل برای Windows x64:

- **Personal — شخصی غیرتجاری:** همان ۳۱ ابزار، به‌همراه بخش افزودن پوشه و کل درایو، کلید دسترسی هر مسیر و پنجره اجرای ۱۵ دقیقه‌ای با امکان بستن فوری. تغییر دسترسی پوشه در موتور واقعی اعمال می‌شود.
- **Commercial — تجاری:** هر ۳۱ ابزار نسخه شخصی در مسیر MCP تجاری پشتیبانی می‌شوند. ابزارهای فایل، PDF، جستجو و پردازش از همان موتور مشترک استفاده می‌کنند. نشست‌های پردازش و جستجو در طول اتصال دستگاه حفظ می‌شوند.

در نسخه تجاری، نقش Owner دائمی است و مشتریان همچنان به اشتراک یا trial معتبر نیاز دارند. اجرای ابزار دستگاه به مجوزها و تأیید محلی مالک وابسته است. ابزارهای پردازش به پنجره اجرای باز در برنامه نیاز دارند. پوشه‌های مجاز و حساب‌ها از هم جدا هستند.

اصلاح ورود Gmail به حساب موجود و نمایش درست نقش Owner نیز در نسخه تجاری موجود است. شناسه حساب، پرداخت‌ها، مجوز Owner و تنظیمات محصول در ارتقا حفظ می‌شوند.

دو نصب‌کننده محل نصب و تنظیمات جدا دارند. نسخه جدید Commercial برای اجرای ابزارهای جدید لازم است. پس از ارتقا، برنامه را باز کنید، دستگاه را متصل کنید و فهرست ابزارهای کانکتور MCP را تازه کنید. آدرس سرویس تجاری: `https://ykurdo-api.sdigital.app/mcp`.

فایل‌های `.sha256` برای بررسی یکسان‌بودن فایل دانلودشده منتشر شده‌اند. نصب‌کننده‌ها فعلاً امضای Authenticode ندارند.

---

Two separate Windows x64 products:

- **Personal (noncommercial):** the same 31 tools plus approved-folder/whole-drive controls, live path switches and a 15-minute execution window with immediate close.
- **Commercial:** all 31 Personal tools through the commercial MCP endpoint. File, PDF, search and process operations use the actual shared Personal engine. Process/search sessions persist while the device engine is connected.

Permanent Owner access is separate from customer subscriptions. Customers still require a valid paid plan or metered trial. Device tools require local owner consent and enabled permissions; process tools also require an execution window. The update preserves account/payment records and separate product settings. Existing-account Gmail sign-in is fixed and Owner is shown explicitly.

Install the matching product, connect the device and refresh the MCP connector's tool list. Commercial endpoint: `https://ykurdo-api.sdigital.app/mcp`. New tools require the updated Commercial client. SHA-256 files identify the published downloads; installers are currently not Authenticode-signed.
