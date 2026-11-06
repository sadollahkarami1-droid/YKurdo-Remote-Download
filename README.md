# YKurdo Remote — دانلود / Download

نسخه‌های پایدار برای Windows x64؛ نسخه‌های آزمایشی Linux نیز در ادامه آمده‌اند. **نسخه تجاری: 1.2.4 — نسخه شخصی: 1.2.0**

| محصول | دانلود نصب‌کننده |
|---|---|
| **Personal — شخصی غیرتجاری** | [دانلود Personal 1.2.0](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/download/v1.2.0-91b33d881736/YKurdo-Remote-Personal-Setup-x64-1.2.0-91b33d881736.exe) |
| **Commercial — تجاری** | [دانلود Commercial 1.2.4](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/download/v1.2.4-f0bbc143ffa7/YKurdo-Remote-Commercial-Setup-x64-1.2.4-f0bbc143ffa7.exe) |

[توضیحات نسخه، SHA-256 و همه دانلودها](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/latest)

## Linux — نسخه آزمایشی 1.3.0-beta.1

دو بسته مستقل **شخصی غیرتجاری** و **تجاری** برای Ubuntu 24.04 x64 آماده‌اند. Node و ripgrep داخل بسته قرار دارند؛ رابط برنامه پنل محلی در مرورگر همان دستگاه است.

| محصول Linux | نصب Ubuntu / Debian |
|---|---|
| Personal — شخصی غیرتجاری | [دانلود بسته شخصی `.deb`](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/download/linux-v1.3.0-beta.1-1f144b0fe2aa/ykurdo-remote-personal_1.3.0.beta.1-1f144b0fe2aa_amd64.deb) |
| Commercial — تجاری | [دانلود بسته تجاری `.deb`](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/download/linux-v1.3.0-beta.1-1f144b0fe2aa/ykurdo-remote-commercial_1.3.0.beta.1-1f144b0fe2aa_amd64.deb) |

[همه فایل‌های Linux، آرشیو نصب بدون دسترسی مدیر و SHA-256](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/tag/linux-v1.3.0-beta.1-1f144b0fe2aa) · [راهنمای نصب و محدودیت‌ها](LINUX-INSTALL-FA.md)

نسخه تجاری Linux به همان سرویس و ۳۱ ابزار اصلی متصل است و سه حالت دسترسی، پوشه‌های مستقل و بازه اجرای ۱۵ دقیقه‌ای دارد. نسخه شخصی اتصال محلی MCP و تنظیمات مستقل دارد. آزمون‌ها روی Ubuntu در WSL2 انجام شده‌اند؛ ورود Google با حساب واقعی و اجرای طولانی روی دسکتاپ‌های مختلف هنوز تأیید نشده است. PDF از Markdown به Chrome/Chromium نصب‌شده نیاز دارد. **این نسخه آزمایشی است و جایگزین نسخه پایدار ویندوز نشده است.**

macOS فاز بعدی است؛ هنوز نصب‌کننده مک منتشر نشده است.

## تغییرات Commercial 1.2.4 — Windows

رفع کرش و قطع اتصال هنگام دریافت پاسخ بزرگِ تأیید نتیجه ابزار. پاسخ‌های مدیریتی محدود خوانده می‌شوند و خطای داده نامعتبر کل برنامه را نمی‌بندد. نصب، حساب و تنظیمات قبلی را حفظ می‌کند.

## تغییرات Commercial 1.2.3 — Windows

ترجمه‌های شش زبان فعال همگام شدند: هر زبان ۴۱۸ عبارت دارد. متن‌های حالت دسترسی، مجوز اجرا، Owner، ورود Google و اتصال تکمیل شدند. پنجره تأیید درخواست نیز ترجمه می‌شود و تغییر چندباره زبان برای متن‌های پویا اصلاح شده است.

## تغییرات Commercial 1.2.2 — Windows

- دکمه روشن‌کردن Remote هر ۳۱ ابزار و Full Auto را آماده می‌کند؛ مجوز اجرای فرمان خودکار تمدید می‌شود و دکمه جداگانه ۱۵ دقیقه‌ای لازم نیست.
- خاموش‌کردن Remote موتور محلی و درخواست‌های جاری را متوقف و دستگاه را آفلاین می‌کند.
- تغییر مجوز ابزارها خودکار ذخیره می‌شود و حالت دسترسی هنگام اتصال هم قابل تغییر است.
- پوشه‌های مجاز، حساب تأییدشده و الزام اشتراک یا trial مشتریان برقرارند. نصب، تنظیمات و ورود ذخیره‌شده را حفظ می‌کند.
- شروع خودکار برنامه همچنان حالت پیش‌فرض فقط‌خواندنی را حفظ می‌کند؛ فعال‌سازی کامل با دکمه اصلی Remote انجام می‌شود.

## تغییرات Commercial 1.2.1

روی صفحه اصلی تجاری، بخش «حالت دسترسی هوش مصنوعی» اضافه شده است:

- **فقط‌خواندنی · Read Only:** حالت پیش‌فرض؛ ابزارهای تغییر، اجرا و مدیریت رد می‌شوند.
- **با تأیید · Ask:** اجرای هر ابزار دستگاه به تأیید جداگانه شما نیاز دارد.
- **تمام‌خودکار · Full Auto:** پس از انتخاب و تأیید داخل برنامه، ابزارهای مجاز بدون پرسش جداگانه اجرا می‌شوند.

فقط یک حالت فعال است. برای تغییر حالت، اتصال را متوقف کنید. با بازشدن دوباره برنامه یا خروج از حساب، حالت فقط‌خواندنی برمی‌گردد. مجوز ابزارها، پوشه‌ها، بازه اجرای دستور و کنترل‌های سرور در همه حالت‌ها برقرارند؛ قطع اتصال از راه دور همچنان تأیید جداگانه می‌خواهد.

## تغییرات 1.2.0

- هر **۳۱ ابزار نسخه شخصی** در نسخه تجاری پشتیبانی می‌شود: فایل و پوشه، ویرایش، PDF، جستجو، ترمینال و نشست پردازش، تنظیمات مجاز، گزارش‌ها و مدیریت دستگاه.
- به نسخه **شخصی غیرتجاری** بخش افزودن پوشه یا کل درایو، روشن و خاموش‌کردن دسترسی هر مسیر و پنجره اجرای ۱۵ دقیقه‌ای اضافه شده است.
- ورود Gmail به حساب موجود در نسخه تجاری اصلاح شده و نقش Owner با عنوان دسترسی دائمی مالک نمایش داده می‌شود.
- دو نصب‌کننده، محل نصب و تنظیمات مستقل دارند؛ نصب هرکدام، محصول دیگر را تبدیل نمی‌کند.

## کنترل دسترسی

هر ابزار مجوز مستقل دارد. در Commercial ویندوز 1.2.2، زدن دکمه روشن‌کردن Remote هر ۳۱ ابزار و Full Auto را فعال و مجوز زمان‌دار اجرا را خودکار تمدید می‌کند. خاموش‌کردن Remote اجرای جاری و موتور محلی را متوقف می‌کند. مجوزها خودکار ذخیره می‌شوند و همچنان می‌توان ابزارهای خاص را خاموش کرد. پوشه‌های مجاز و احراز هویت برقرار می‌مانند. مسیرها را در خود برنامه انتخاب و مدیریت کنید. درخواست نامعتبر، دستگاه آفلاین یا مجوز لغوشده اجازه اجرا نمی‌گیرد.

در Commercial، مالک اصلی با نقش سروری Owner دسترسی دائمی دارد. مشتریان به اشتراک معتبر یا trial فعال نیاز دارند.

## استفاده از نسخه تجاری

1. نصب‌کننده **Commercial** را دانلود و برنامه را باز کنید.
2. با Google یا حساب ایمیل خود وارد شوید و اتصال دستگاه را مطابق راهنما تنظیم کنید.
3. پوشه‌ها و مجوزهای موردنیاز را در برنامه انتخاب و دستگاه را متصل کنید.
4. در کلاینت پشتیبانی‌شده، کانکتور MCP را با `https://ykurdo-api.sdigital.app/mcp` اضافه کنید و ورود را تکمیل کنید. پس از ارتقا، فهرست ابزارهای کانکتور را تازه کنید.

برای کنترل خودکار اجرا با کلید Remote، برنامه Commercial ویندوز را به 1.2.2 ارتقا دهید.

## اشتراک Commercial

دوره آزمایشی: ۵۰۰۰ فراخوانی ابزار در ۳۰ روز، یک بار برای هر دستگاه. ماهانه: ۱۹٫۹۹ یورو؛ سالانه: ۲۱۰ یورو. قیمت نهایی و مالیات در صفحه رسمی Stripe مشخص می‌شود. مدیریت یا لغو اشتراک از پورتال پرداخت انجام می‌شود.

## بررسی فایل دانلود

نصب‌کننده‌ها فعلاً امضای Authenticode ندارند. SHA-256 هر فایل در همان انتشار موجود است:

```powershell
Get-FileHash .\YKurdo-Remote-*-Setup-x64-*.exe -Algorithm SHA256
```

## English

Two independent Windows x64 products: **Personal (noncommercial)** and **Commercial**. Version 1.2.0 brings all 31 Personal tools to the Commercial endpoint and adds approved-folder/whole-drive switches and a 15-minute execution window to Personal.

Commercial supports verified Gmail sign-in to existing accounts. Owner access is permanent; customers retain subscription or metered-trial requirements. Commercial 1.2.2 makes an explicit Remote On enable all 31 permissions and Full Auto, automatically renews the bounded execution lease, and stops the local engine and in-flight requests on Off. Permission changes save automatically. Approved roots and subscription/trial checks remain enforced. Commercial 1.2.1 added Read Only, Ask and Full Auto on Home. Exactly one local mode is active; restart/logout restores Read Only. Full Auto skips per-call prompts after local opt-in, while tool permissions, approved roots, execution windows and server checks remain enforced. Shutdown still asks separately. In Commercial Windows 1.2.2 the process execution lease is managed automatically while Remote is On. Install the matching product, connect the device and refresh the MCP connector's tool list.

Commercial MCP endpoint: `https://ykurdo-api.sdigital.app/mcp`. Trial: 5,000 tool calls over 30 days, once per device. Plans: EUR 19.99/month or EUR 210/year; final price and tax appear in Stripe Checkout.

Installers preserve separate product identities and settings. They are currently not Authenticode-signed; compare their SHA-256 against the release checksums. This repository distributes binaries and documentation; the development repository remains private.
