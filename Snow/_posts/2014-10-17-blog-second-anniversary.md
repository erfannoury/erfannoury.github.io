---
layout: post
category: Visualization, Blog
title: دومین سالگرد وبلاگ :)
---
به نام خدا
===========

امروز دومین سالگرد اون یکی وبلاگمه. دو سال پیش در همین روز بود که اولین پستم رو توی اون بلاگ منتشر کردم.امروز به مناسبت دومین سالگرد چون حوصله‌ی پست نوشتن اونجا رو نداشتم، یعنی در واقع حوصله‌ی پست‌نویسی به سبک اونجا رو نداشتم، تصمیم گرفتم اینجا در مورد اون بلاگ بنویسم.

البته نوشتن که چه عرض کنم، بیشتر با چند تا عدد بازی کنم و یه چندتایی نمودار بکشم. هدف بیشتر کار با `matplotlib` بود تا کار مهم دیگه‌ای.

تو این مدت دو ساله، 77 پست رو ارسال کردم تو اون یکی بلاگم

![Timeline post distribution](/stylesheets/images/timeline_raw.png)


![Timeline post distribution](/stylesheets/images/timeline_distribution.png)

خیلی واضحه از روی پست که در یکسال اول، خیلی بیشتر از یکسال دوم پست نوشتم. شاید نشون میده که یکسال دوم، یعنی از یکسال پیش، آرامیش بیشتری به زندگیم حاکم بوده. از طرف دیگه شاید بشه گفت که  هیجان زندگیم کمتر شده، چیز کمتری بوده تو زندگیم که در موردش بنویسم. البته اگر به آخرهای این مدت زمان نگاهی بندازیم، میبینیم که باز شروع کرده بودم به مرتب نوشتن، ولی باز از حوصله افتادم و الان خیلی وقته که ننوشتم. درسته که فقط دوبار اتفاق افتاده، ولی شاید این تحلیل رو هم بشه کرد که در نزدیکی‌های سالگردها، خیلی کمتر نوشتم.


از نظر زمانی فکر می‌کردم بیشتر پست‌هام رو در روزهای آخر هفته می‌نوشتم. ولی این نمودار چیز دیگه‌ای رو نشون میده

![Weekly post distribution](/stylesheets/images/weekly_distribution.png)

اینطوری که مشخصه بیشترین پست‌هام رو در روز دوشنبه منتشر کردم. هر چند آخرهفته‌ها هم فعال بودم.

یه موضوع دیگه‌ای که مطرحه اینه که بیشتر در چه زمان‌هایی از شبانه‌روز اقدام به ارسال پست می‌کردم؟ حدس خودم اینه که شب‌ها بیشتر می‌نوشتم. داده‌ها هم این حدس رو تایید می‌کنن.

![Daily post distribution](/stylesheets/images/daily_distribution.png)

البته خیلی هم مطابقت نداره با حدسم. بیشترین پست‌ها رو ساعت 20 شب منتشر کردم. در حالی که من حدس می‌زدم زمان ارسال‌هام چند ساعتی دیرتر باشن. این نکته هم جالبه که ساعت 2 و 3 بامداد و همچنین نیمه‌ی روز هیچوقت ارسال پست نداشتم.

موضوع بعدی که دوست داشتم در مورد پستم بدونم این بود که چقدر می‌نویسم؟ خودم که همیشه دوست دارم پست‌هایی که می‌نویسم یا می‌خونم طولانی باشن، بخاطر همین حدس می‌زنم بیشتر پست‌هام طولانی باشن. ولی چقدر طولانی؟ از روی بررسی پست‌ها مشخص میشه که طولانی‌ترین پستم از 4170 کلمه‌ تشکیل شده. فکر می‌کنم خیلی کم نباشه :دی

نمودار پایین هم توزیع پست‌ها بر اساس طولشون رو نشون میده. هر دسته بازه‌ای به طول 400 کلمه است.

![Daily post distribution](/stylesheets/images/post_length_hist.png)

نکته‌ی دیگه‌ای که بهش پرداختم، بررسی رابطه‌ی بین طول پست و زمان ارسال پست بود. یعنی بعضی شبا که میشینم، با خودم هی فکر می‌کنم، آیا نتیجه‌اش این میشه که پست‌های طولانی می‌نویسم؟
محور عمودی طول پست، و محور افقی زمان ارسال پست هست.
شکل پایین این موضوع رو بررسی کرده.

![Post length vs. Publishing time scatter plot](/stylesheets/images/length_vs_time_scatter.png)

یا اگر جور دیگه‌ای بهش نگاه کنیم، اینطوری:

![Post length vs. Publishing time hex plot](/stylesheets/images/length_vs_time_hex.png)

این نمودار آخر به خوبی این ارتباط رو نشون میده. این که بیشتر شب‌ها پست‌های طولانی‌تری می‌نویسم.البته چون داده‌های زمانی ه صورت ترتیبی نیستن، بلکه دوری هستن، نمیشه یک رابطه‌ی خطی بینشون پیدا کرد. اگر بتونم راه‌حلی برای این مورد پیدا کنم، سعی می‌کنم فرمولی برای این رابطه به دست بیارم.


بجز این موارد چیز دیگه‌ای به ذهنم نرسید. یعنی بیشتر به تحلیل متن احتیاج داشتم، ولی همچین چیزی فعلاً بلد نیستم. تنها کاری که تونستم انجام بدم این بود که ماتریس شباهت پست‌هام رو به هم پیدا کردم. در شکل پایین ماتریس شباهت پست‌ها رو می‌بینید.

![Post Similarity Matrix](/stylesheets/images/post_similarity.png)

انتظار دیدن همچین چیزی رو نداشتم. به طرز عجیبی بین سه تا از پست‌ها شباهت زیادی وجود داره، یعنی پست‌های "یه دوست خاص"، "متاسفم"، و "عصبانی". برام این موضوع خیلی عجیب بود. چون نباید این اتفاق میوفتاد. اینقدر شباهت در متن پست‌ها خیلی عجیبه. در نتیجه تصمیم گرفتم متن این پست‌ها رو به دقت و از نزدیک بررسی کنم. وقتی که این کار رو کردم به این نوشته در همه‌شون رسیدم:

> برای نمایش مطلب باید رمز عبور را وارد کنید

و اینطوری بود که از راز شباهت این سه پست هم پرده برداشته شد :دی

اگر بهتر به این ماتریس نگاه کنیم، تعدادی پست‌ها هستن که خیلی با پست‌های دیگه تفاوت دارن. اینا پست‌هایی هستن که توشون کلمات انگلیسی زیادی به کار برده شده. ولی بین بعضی دیگر از پست‌ها شباهت‌های خوبی هست. نیاز هست که دقیق‌تر این پست‌ها رو باز بررسی کنم.



نکته‌ی جالبی که رخ داد اینه که بیان دسترسیم رو بلاگم قطع کرده بخاطر اینکه درخواست زیاد فرستادم.
