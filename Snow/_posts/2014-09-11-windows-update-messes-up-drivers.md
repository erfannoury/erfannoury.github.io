---
layout: post
category: Windows, Windows Update, Problem
title: حل مشکل درایورها پس از ایجاد مشکل توسط Windows Update
---
به نام خدا
===========

چند روز پیش سری به قسمت آپدیت‌های ویندوز آپدیت زدم. من خودم نصب آپدیت‌های ویندوز را در حالت خودکار گذاشتم ولی هر از چند گاهی به قسمت آپدیت‌های ویندوز سر می‌زنم تا ببینم آپدیت‌های اختیاری جدیدی وجود دارند یا نه. این با که به این قسمت سر زدم، با آپدیت جدیدی برای درایور Intel HD Graphics مواجه شدم. اینتل از چند نسل قبل در پردازنده‌های خود یک پردازنده‌ی گرافیکی نیز تعبیه کرده است. این پردازنده‌ی گرافیکی با اینکه در ابتدا توان بسیاری نداشت، ولی در نسل‌های اخیر پردازنده‌های اینتل به پردازنده‌ی بسیار قدرتمندی تبدیل شده است. همچنین به دلیل یکپارچه بودن با پردازنده، ویندوز بسیاری از پردازش‌های گرافیکی را توسط این پردازنده‌ی گرافیکی انجام می‌دهد. در این صورت بار محاسباتی بر روی پردازنده‌ی اصلی کمتر شده و همچنین مصرف برق نیز کاهش میابد. به همین خاطر است که بروزرسانی درایور این پردازنده‌ی گرافیکی در بهتر کردن تجربه‌ی کاربری ویندوز مفید است.
البته این بار بعد از به روزرسانی درایور پردازنده‌ی گرافیکی اینتل از طریق Windows Update مشکلی رخ داد. اولین مشکل عمده این بود که امکان تغییر روشنایی نمایشگر از بین رفت و نمایشگر در روشن‌ترین حالت خود قرار گرفت و این آزاردهنده بود. مشکل دوم این بود که کیفیت تصویر به میزان بسیار قابل توجهی کاهش یافت و این مشکل، حتی بیشتر آزاردهنده بود. پس از نصب چندین و چند باره‌ی انواع درایور دیگر که اتفاقاً جدیدترین درایورها از طرف اینتل و همچنین Lenovo بودند، باز این مشکل برطرف نشد.

در نهایت به راه‌حل جالب دیگری دست یافتم. البته این راه‌حل، دست‌مایه‌ی جستجوهای فراوان در اینترنت است.

اگر بعد از به روزرسانی درایوری مشاهده کردید که عملکرد سخت‌افزار مورد نظر با مشکل همراه است، یک روش ساده برای بازگرداندن درایور قبلی وجود دارد.

(اگر آپدیتی از طرف Windows Update مشکلی ایجاد کرد، راه‌حل کلی این است که آپدیت مورد نظر را پاک کنید، ولی کاهی امکان پاک‌کردن بعضی آپدیت‌ها وجود ندارد؛ مورد اخیر نیز از این دسته آپدیت‌ها بود)

راه حل
=======
1.  به Device Manager بروید. در ویندوز 8 می‌توان با جستجوی این عبارت به مکان مورد نظر رفت. در ویندوزهای قبلی نیز می‌توان با راست‌کلیک بر روی آیکون My Computer و انتخاب `Manage`، به Device Manager رفت.
2.  از لیست سخت‌افزارها، سخت‌افزار مورد نظر که درایور آن مشکل پیدا کرده است را پیدا کنید.
3.  بر روی نام درایور راست‌کلیک کنید و گزینه‌ی

    Update Driver Software...

    را انتخاب کنید.

4.  در صفحه‌ای که باز می‌شود گزینه‌ی

    Browse my computer for driver software

    را انتخاب نمایید.
5.  در صفحه‌ی بعدی که باز می‌شود، گزینه‌ی

    Let me pick from a list of device drivers on my computer

    را انتخاب کنید.
6.  در نهایت، در صفحه‌ای که باز می‌شود، از لیست موجود، درایوری از تاریخی گذشته را که سخت‌افزار بدون مشکل عمل می‌کرد انتخاب نمایید. توجه کنید که تیک قسمت `Show Compatible Hardware` زده شده باشد.

![Device Manager - Revert to old driver software](/stylesheets/images/device-manager.png)

با انجام این دستورات، می‌توانید درایور سخت‌افزاری مورد نظر را به تاریخی گذشته برگردانید و مشکل را حل نمایید.