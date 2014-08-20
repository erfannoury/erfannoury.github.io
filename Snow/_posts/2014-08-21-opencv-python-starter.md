---
layout: post
category: Programming, OpenCV, Tutorial, Python, Starter Code
title: OpenCV Python Starter Code
---
به نام خدا
===========

معمولاً رسم هست که اولین کد در هر زبان برنامه‌نویسی رو با چاپ کردن عبارت `Hello World` در خروجی شروع می‌کنند.

ولی جدای از زبان‌های برنامه‌نویسی گاهی نیاز هست به سرعت بفهمیم آیا تنظیم و نصب یک کتابخانه‌ی مشخص در یک زبان برنامه‌نویسی به درستی انجام گرفته یا نه. برای اینکار لازمه تکه‌کد کوچکی رو با استفاده از این کتابخانه اجرا کنیم تا به مشکلات در صورت وجود پی ببریم. معمولاً پیدا کردن همچین تکه‌کدهای کوتاه کار راحتی نیست و بیشتر از اون که باید، گاهی زمان می‌بره. به همین دلیل تصمیم گرفتم از این به بعد کدهای کوچکی با عنوان Starter Code برای کتابخانه‌هایی که استفاده می‌کنم بر روی این وبلاگ قرار بدهم تا به عنوان یک راهنمای کوتاه برای انجام این امر باشه.

به عنوان اولین پست از این مجموعه، تکه کدی رو قرار می‌دهم تا بشه باهاش به سرعت کتابخانه‌ی `OpenCV` رو در پایتون امتحان کرد.

###نمونه کد


    import numpy as np
    import cv2

    # Open the webcam to grab frames and display them
    cap = cv2.VideoCapture(0)

    while(True):
        ret, frame = cap.read()
        gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
        cv2.imshow('frame',gray)
        if cv2.waitKey(1) & 0xFF == ord('q'):
            break

    # When everything done, release the capture
    cap.release()
    cv2.destroyAllWindows()


Sample code source: [[OpenCV-Python-Tutorials](http://opencv-python-tutroals.readthedocs.org/en/latest/py_tutorials/py_gui/py_video_display/py_video_display.html)]

این کد، ابتدا کتابخانه‌های لازم را بارگزاری می‌کنه. سپس اولین فریم از تصویر از وب‌کم گرفته میشه. بعد در یک لوپ تکرار شونده، در ابتدا یک فریم جدید از وب‌کم گرفته میشه، سپس با تبدیل نمایش فریم گرفته شده از حالت رنگی به سیاه‌سفید، تصویر نهایی در خروجی نمایش داده میشه. در نهایت هرگاه کلید `q` توسط کاربر وارد بشه، برنامه از لوپ خارج شده و نمایش تصاویر از وب‌کم متوقف میشه.
