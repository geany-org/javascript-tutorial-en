# مقدمه ای بر جاوا اسکریپت

بیایید ببینیم چه چیزی در مورد جاوا اسکریپت بسیار خاص است, چه کاری با آن می توانیم انجام دهیم و چه تکنولوژی های دیگری با آن کار می کنند

## جاوا اسکریپت چیست؟

جاوا اسکریپت* در ابتدا برای *"صفحات پویای وب"* ایجاد شد*

برنامه های این زبان, اسکریپت نامیده می شوند و می توان آن ها را به طور مستقیم در اچ تی ام ال نوشت و به صورت خودکار در صفحه اجرا کرد

اسکریپت ها به عنوان یک متن ساده, نوشته و اجرا می شوند و به انجام عملیات خاص نیازی ندارند

در این زمینه, جاوا اسکریپت از زبان دیگری به نام جاوا بسیار متفاوت است

```smart header="چرا <u>جاوا</u>اسکریپت؟"
وقتی جاوا اسکریپت ساخته شد, ابتدا نام دیگری با عنوان "لایو اسکریپت" داشت اما زبان جاوا در آن زمان بسیار محبوب بود و این زبان جدید تصمیم گرفت به عنوان "برادر کوچک جاوا" به مردم کمک کند 

پس از تکامل به یک زبان کاملا مستقل تبدیل شد و در حال حاضر هیچ ارتباطی با جاوا ندارد
```

در حال حاضر جاوا اسکریپت می تواند علاوه بر مرورگر, بر روی سرور یا هر دستگاهی که دارای موتور جاوا اسکریپت است, اجرا شود

مرورگر دارای یک موتور جاسازی شده است که از آن با نام "ماشین مجازی جاوا اسکریپت" نیز یاد می شود

موتورهای مختلف, نام های مختلفی دارند به عنوان مثال

- وی ۸ در کروم و اپرا
- اسپایدار مانکی در فایرفاکس
- نام های دیگری مانند "تری دنت" و "چاکرا" برای نسخه های مختلف اینترنت اکسپلورر, "چاکرا کور" برای مایکروسافت اج, "نیترو" و "اسکورل فیش" برای سافاری و غیره

واژه های بالا بهتر است به خاطر سپرده شوند زیرا در مقاله های موجود در اینترنت به کار برده می شوند و ما نیز از آن ها استفاده خواهیم کرد 

```smart header="موتورها چگونه کار می کنند؟"

موتورها یا انجین ها پیچیده هستند اما مبانی آن ها ساده است

۱- موتور (تعبیه شده در مرورگر) اسکریپت را خوانده و آن را تجزیه می کند
۲- سپس این اسکریپت را به زبان ماشین ترجمه می کند
۳- و در نهایت کد ماشین به سرعت اجرا می شود

این موتور, بهینه سازی را در هر مرحله از روند کار انجام می دهد, حتی اسکریپت ترجمه شده را اجرا و داده ها را از طریق آن تجزیه و تحلیل و در نهایت بهینه سازی ها را به کد ماشین اعمال می کند. لازم به ذکر است که اسکریپت ها بسیار سریع هستند
```

## جاوا اسکریپت چه کاری می تواند انجام دهد؟

جاوا اسکریپت مدرن, زبان برنامه نویسی "امنی" است. در این زبان امکان دسترسی های سطح پایین به حافظه یا پردازنده وجود ندارد زیرا در ابتدا برای مرورگر هایی ساخته شده بود که به چنین دسترسی هایی نیازی نداشتند

این قابلیت ها کاملا به محیطی که جاوا اسکریپت را اجرا می کنند بستگی دارد. به عنوان مثال نود جی اس از توابعی پشتیبانی می کند که جاوا اسکریپت را قادر به خواندن/نوشتن فایل های دلخواه, انجام درخواست های شبکه و غیره می کند

در مرورگر, جاوا اسکریپت می تواند همه چیز مربوط به صفحه وب را دستکاری کند یا با کاربر و سرور تعامل داشته باشد

به عنوان مثال جاوا اسکریپت در مرورگر قادر است تا

- اچ تی ام ال جدیدی را به صفحه اضافه کند, محتوای موجود را تغییر دهد یا استایل ها را اصلاح کند
- به اقدامات کاربر مانند کلیک یا حرکت ماوس, و فشار کلید صفحه کلید واکنش نشان دهد
- درخواست هایی را در شبکه به سرور ارسال کند یا آپلود و دانلود انجام دهد
- کوکی ها را دریافت و تنظیم کنید, سوالات را به بازدید کننده بفرستید و پیام ها را نشان دهید
- داده های سمت کاربر را یه خاطر (ذخیره سازی محلی) داشته باشد

## جاوا اسکریپت چه کارهایی را در مرورگر نمی تواند انجام دهد؟

توانایی های جاوا اسکریپت در مرورگر به خاطر ایمنی کاربر محدود است. هدف این است که از دسترسی به اطلاعات خصوصی یا آسیب رساندن به اطلاعات کاربر جلوگیری شود

نمونه هایی از این محدودیت ها عبارتند از

- جاوا اسکریپت در یک صفحه وب, ممکن است فایل های دلخواه خواندن/نوشتن, کپی کردن یا اجرای برنامه ها را بر روی هارد دیسک نداشته باشد. بنابراین دسترسی مستقیم به توابع سیستم عامل را ندارد

- مرورگرهای پیشرفته, اجازه کار با فایل ها را می دهند اما دسترسی محدود است و فقط در صورتی انجام می شود که کاربر اقدامات خاصی مانند حذف یک فایل در پنجره مرورگر یا انتخاب آن را انجام دهد

راه هایی برای ارتباط با دوربین/میکروفون و سایر دستگاه ها وجود دارد اما آن ها نیاز به اجازه صریح کاربر دارند. بنابراین در صفحه ای که جاوا اسکریپت فعال است, ممکن است وب سایت دوربین را فعال نکند و امکان مشاهده محیط وجود نداشته باشد 
- زبانه ها/ پنجره های مختلف معمولا در مورد یکدیگر چیزی نمی دانند. 

    This is called the "Same Origin Policy". To work around that, *both pages* must contain a special JavaScript code that handles data exchange.

    The limitation is again for user's safety. A page from `http://anysite.com` which a user has opened must not be able to access another browser tab with the URL `http://gmail.com` and steal information from there.
- JavaScript can easily communicate over the net to the server where the current page came from. But its ability to receive data from other sites/domains is crippled. Though possible, it requires explicit agreement (expressed in HTTP headers) from the remote side. Once again, that's safety limitations.

![](limitations.png)

Such limits do not exist if JavaScript is used outside of the browser, for example on a server. Modern browsers also allow installing plugin/extensions which may get extended permissions.

## What makes JavaScript unique?

There are at least *three* great things about JavaScript:

```compare
+ Full integration with HTML/CSS.
+ Simple things done simply.
+ Supported by all major browsers and enabled by default.
```

Combined, these three things exist only in JavaScript and no other browser technology.

That's what makes JavaScript unique. That's why it's the most widespread tool to create browser interfaces.

While planning to learn a new technology, it's beneficial to check its perspectives. So let's move on to the modern trends that include new languages and browser abilities.


## Languages "over" JavaScript

The syntax of JavaScript does not suit everyone's needs. Different people want different features.

That's to be expected, because projects and requirements are different for everyone.

So recently a plethora of new languages appeared, which are *transpiled* (converted) to JavaScript before they run in the browser.

Modern tools make the transpilation very fast and transparent, actually allowing developers to code in another language and autoconverting it "under the hood".

Examples of such languages:

- [CoffeeScript](http://coffeescript.org/) is a "syntactic sugar" for JavaScript, it introduces shorter syntax, allowing to write more precise and clear code. Usually Ruby devs like it.
- [TypeScript](http://www.typescriptlang.org/) is concentrated on adding "strict data typing", to simplify development and support of complex systems. It is developed by Microsoft.
- [Dart](https://www.dartlang.org/) is a standalone language that has its own engine that runs in non-browser environments (like mobile apps). It was initially offered by Google as a replacement for JavaScript, but as of now, browsers require it to be transpiled to JavaScript just like the ones above.

There are more. Of course even if we use one of those languages, we should also know JavaScript, to really understand what we're doing.

## Summary

- JavaScript was initially created as a browser-only language, but now it is used in many other environments as well.
- At this moment, JavaScript has a unique position as the most widely-adopted browser language with full integration with HTML/CSS.
- There are many languages that get "transpiled" to JavaScript and provide certain features. It is recommended to take a look at them, at least briefly, after mastering JavaScript.
