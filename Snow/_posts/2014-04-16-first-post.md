---
layout: post
category: عمومی, بلاگ
title: اولین پست، ولی آزمایشی
---
#به نام خدا

این یک آزمایش است.

This is only a test.

بعد از اینکه  دیدم سایت [Koding](www.koding.com) داون شد، دیدم که مطمئن‌ترین جا برای نوشتن این پست‌ها، همین کامپیوتر خودم هست. بخاطر همین هم Octopress و Jekyll رو کلاً انداختم کنار و رو آوردم به the real thing، یعنی .Net :دی

الان دارم از یک نسخه‌ی تغییر یافته از پروژه‌ی [Sandra.Snow](https://github.com/Sandra/Sandra.Snow) استفاده می‌کنم. بعضی تغییرات رو توش اعمال کردم تا کلاً بلاگ برای نمایش فارسی بهتر بشه. البته از کد جاوااسکریپ [bidiweb](https://github.com/hasenj/bidiweb) هم استفاده کردم تا متونی که احیاناً بخاطر تغییر زبان به هم بریزن رو درست بکنه. همچنین از کتابخونه‌ی خیلی خوب [MathJax](http://mathjax.org) هم برای نمایش \\(\LaTeX\\) استفاده کردم. بعضی وقتا شاید به درد بخورن. 

حالا یکم قابلیت‌هایش رو تست بکنیم.

This is a text written in English, and yes it is displayed correctly (not that it wouldn't normally :D)



این هم یه تیکه کد:

	using System;
	
	public class test
	{
		public static void Main(string[] args)
		{
			Console.WriteLine("Hello World, from Sandra.Snow!");
		}
	}
	
و حالا یکم ریاضی درون یک نوشته‌ی انگلیسی

When \\(a \ne 0\\), there are two solutions to \\(ax^2 + bx + c = 0\\) and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

و همون پاراگراف قبلی به صورت یک پاراگراف فارسی

هرگاه \\(a \ne 0\\)، دو پاسخ برای معادله‌ی \\(ax^2 + bx + c = 0\\) داریم که برابر هستند با:
$$ x_{1,2} = \frac{-b \pm \sqrt{b^2 - 4ac}}{2 a}$$.

و همین دیگه. امیدوارم اونطوری که می‌خوام بتونم بنویسم اینجا و برای خودم و دیگران هم مفید باشه.

تا پستِ بعدی :)