# YKurdo Remote — دانلود / Download

دو برنامه مستقل برای Windows x64. **نسخه تجاری: 1.2.1 — نسخه شخصی: 1.2.0**

| محصول | دانلود نصب‌کننده |
|---|---|
| **Personal — شخصی غیرتجاری** | [دانلود Personal 1.2.0](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/download/v1.2.0-91b33d881736/YKurdo-Remote-Personal-Setup-x64-1.2.0-91b33d881736.exe) |
| **Commercial — تجاری** | [دانلود Commercial 1.2.1](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/download/v1.2.1-89672b94765a/YKurdo-Remote-Commercial-Setup-x64-1.2.1-89672b94765a.exe) |

[توضیحات نسخه، SHA-256 و همه دانلودها](https://github.com/sadollahkarami1-droid/YKurdo-Remote-Download/releases/latest)

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

هر ابزار مجوز مستقل دارد. اجرای ابزار روی دستگاه تابع حالت انتخاب‌شده در خود برنامه است و ابزارهای پردازش به پنجره اجرای باز نیاز دارند. مسیرها را در خود برنامه انتخاب و مدیریت کنید. درخواست نامعتبر، دستگاه آفلاین یا مجوز لغوشده اجازه اجرا نمی‌گیرد.

در Commercial، مالک اصلی با نقش سروری Owner دسترسی دائمی دارد. مشتریان به اشتراک معتبر یا trial فعال نیاز دارند.

## استفاده از نسخه تجاری

1. نصب‌کننده **Commercial** را دانلود و برنامه را باز کنید.
2. با Google یا حساب ایمیل خود وارد شوید و اتصال دستگاه را مطابق راهنما تنظیم کنید.
3. پوشه‌ها و مجوزهای موردنیاز را در برنامه انتخاب و دستگاه را متصل کنید.
4. در کلاینت پشتیبانی‌شده، کانکتور MCP را با `https://ykurdo-api.sdigital.app/mcp` اضافه کنید و ورود را تکمیل کنید. پس از ارتقا، فهرست ابزارهای کانکتور را تازه کنید.

برای مجموعه کامل ۳۱ ابزار، برنامه Commercial را به 1.2.1 ارتقا دهید.

## اشتراک Commercial

دوره آزمایشی: ۵۰۰۰ فراخوانی ابزار در ۳۰ روز، یک بار برای هر دستگاه. ماهانه: ۱۹٫۹۹ یورو؛ سالانه: ۲۱۰ یورو. قیمت نهایی و مالیات در صفحه رسمی Stripe مشخص می‌شود. مدیریت یا لغو اشتراک از پورتال پرداخت انجام می‌شود.

## بررسی فایل دانلود

نصب‌کننده‌ها فعلاً امضای Authenticode ندارند. SHA-256 هر فایل در همان انتشار موجود است:

```powershell
Get-FileHash .\YKurdo-Remote-*-Setup-x64-*.exe -Algorithm SHA256
```

## English

Two independent Windows x64 products: **Personal (noncommercial)** and **Commercial**. Version 1.2.0 brings all 31 Personal tools to the Commercial endpoint and adds approved-folder/whole-drive switches and a 15-minute execution window to Personal.

Commercial supports verified Gmail sign-in to existing accounts. Owner access is permanent; customers retain subscription or metered-trial requirements. Commercial 1.2.1 adds Read Only, Ask and Full Auto on Home. Exactly one local mode is active; restart/logout restores Read Only. Full Auto skips per-call prompts after local opt-in, while tool permissions, approved roots, execution windows and server checks remain enforced. Shutdown still asks separately. Process tools also need an execution window. Install the matching product, connect the device and refresh the MCP connector's tool list.

Commercial MCP endpoint: `https://ykurdo-api.sdigital.app/mcp`. Trial: 5,000 tool calls over 30 days, once per device. Plans: EUR 19.99/month or EUR 210/year; final price and tax appear in Stripe Checkout.

Installers preserve separate product identities and settings. They are currently not Authenticode-signed; compare their SHA-256 against the release checksums. This repository distributes binaries and documentation; the development repository remains private.
