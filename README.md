# YKurdo Remote — دانلود | Download

**فارسی** | [English](#english)

برنامهٔ ویندوز برای اتصال امن Claude و ChatGPT به رایانهٔ خودتان، با کنترل کامل شما بر هر اجازه.

## این برنامه چه می‌کند
YKurdo Remote یک رابط MCP روی ویندوز است. بعد از ورود و فشردن «اتصال»، دستیار هوش مصنوعی شما می‌تواند فقط در پوشه‌هایی که خودتان تأیید کرده‌اید کار کند:
- فهرست‌کردن، خواندن و جستجوی فایل‌ها
- نوشتن و ویرایش فایل‌های متنی (قبل از تغییر، نسخهٔ پشتیبان ساخته می‌شود)
- دستورهای فقط‌خواندنی git
- اجرای دستور ترمینال، فقط در «پنجرهٔ اجرا»ی زمان‌دار که خودتان در برنامه باز می‌کنید

## کنترل با شماست
- هر ابزار کلید جدا دارد و پیش‌فرض خاموش است؛ خودتان روشن می‌کنید.
- هر درخواست نوشتن یا ویرایش، پنجرهٔ تأیید روی صفحهٔ خودتان نشان می‌دهد. تأیید نکنید یا ۶۰ ثانیه بگذرد، رد می‌شود.
- برنامه فقط به پوشه‌هایی دسترسی دارد که خودتان اضافه کرده‌اید.

## قیمت
- **دورهٔ رایگان:** ۵٬۰۰۰ تماس ابزار در ۳۰ روز، فقط یک بار برای هر دستگاه.
- **ماهانه:** ۱۹٫۹۹ یورو در ماه؛ **سالانه:** ۲۱۰ یورو در سال. پرداخت امن از طریق Stripe و لغو در هر زمان از پورتال.

## نصب
1. آخرین نسخه را از بخش **Releases** همین صفحه دانلود کنید (`YKurdo-Remote-Commercial-Setup-x64-….exe`).
2. اجرا کنید. بعد از نصب، راهنمای کامل ۷ زبانه باز می‌شود (در منوی Start هم هست).
3. وارد حساب شوید، پوشه‌های مجاز را اضافه کنید و «اتصال» را بزنید.
4. در Claude یا ChatGPT یک کانکتور MCP با این آدرس اضافه کنید: `https://ykurdo-api.sdigital.app/mcp`

### هشدار SmartScreen
فعلاً نصب‌کننده **امضای دیجیتال ندارد** (مرحلهٔ اول انتشار). ویندوز ممکن است بنویسد «Windows protected your PC». در این صورت **More info** و بعد **Run anyway** را بزنید. برای اطمینان، SHA-256 فایل دانلودشده را با مقدار فایل `.sha256` کنار همان نسخه مقایسه کنید:

```powershell
Get-FileHash .\YKurdo-Remote-Commercial-Setup-x64-*.exe -Algorithm SHA256
```

## English
Windows app that securely connects Claude and ChatGPT to your own PC, with you controlling every permission.

**What it does.** After you sign in and press Connect, your AI assistant can work only inside folders you approved: list, read and search files; write and edit text files (a backup is made first); read-only git commands; and run terminal commands only during a time-limited execution window that you open yourself in the app.

**You stay in control.** Every tool has its own switch (off by default). Each write or edit request shows a confirmation dialog on your screen; no answer within 60 seconds means rejected.

**Pricing.** Free: 5,000 tool calls over 30 days, once per device. Paid: €19.99/month or €210/year via Stripe; cancel any time from the billing portal.

**Install.** Download the latest installer from **Releases**, run it (a 7-language user guide opens at the end), sign in, add allowed folders, press Connect, then add an MCP connector in Claude or ChatGPT with `https://ykurdo-api.sdigital.app/mcp`.

**SmartScreen notice.** The installer is currently **not code-signed**. If Windows warns, choose **More info → Run anyway**, and compare the file's SHA-256 with the `.sha256` file published with the release.

---
© YKurdo Remote. All rights reserved. This repository hosts release binaries only and contains no source code.
