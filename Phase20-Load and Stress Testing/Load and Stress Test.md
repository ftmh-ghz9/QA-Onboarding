## آشنایی عمیق‌تر با مفاهیم تست فشار و بار

<p>

تست عملکرد یک تست کلیدی برای فهم نحوه کار سیستم است. بدون یک تست عملکردی مناسب شما نمی‌توانید بفهمید نرم‌افزار در شرایط مختلف -پیش‌بینی شده و نشده- چگونه کار می‌کند. 
تست بار و تست استرس دو نوع از تست عملکرد سامانه هستند. اینکه چگونه و چه زمانی از تست بار استفاده شود، بستگی به اهداف تست دارد، مثلا:
- هنگامی که همه چیز طبق سناریوهای مورد انتظار است نرم افزار شما چگونه کار می‌کند؟
- هنگامی که اتفاقات غیر منتظره می‌افتد (تعداد کاربر بالا، داده بیش از حد و …) نرم افزار شما چه رفتاری نشان می‌دهد؟ 
</p>

## تست بار در مقابل تست استرس (Stress Testing vs. Load Testing)


<p>

**تست عملکرد** 
(**Performance Testing**)
یک مفهوم کلی است که شامل هر دو نوع تست بار و استرس می‌شود. هنگام توسعه یک نرم‌افزار، برای مانیتور کردن دقیق‌تر و بهتر عملکرد نرم‌افزار، نیاز است یک معیار مشخص و استاندارد وجود داشته باشد که با استفاده از آن، بتوان تغییرات عملکردی و امتیاز عملکردی نرم‌افزار
(Software performance score)
را به‌طور مطلق سنجید، در اصطلاح به چنین معیاری (که عددی نیز هست) **بنچمارک** 
**(Benchmark)**
گفته می‌شود.

</p>

<div style="text-align:center">
    <img src="https://queue-it.com/media/ubrdvuhb/load-testing-vs-stress-testing.png" alt="Load Test vs. Stress Test" width="500px">
</div>

<p>

این نوع تست همانطور که بالاتر گفته شد می‌تواند شامل موارد زیر باشد:
- **شرایط عادی**: اگر همه چیز طبق برنامه پیش برود، (تعداد داده مورد انتظار، تعداد کاربر مورد انتظار،تعداد درخواست مورد انتظار به سرویس های مشخص) نرم افزار چگونه کار می کند؟
- **شرایط غیرعادی**:مثلا نرم‌افزار شما تا چه حد می‌تواند جلوی حملات DDoS (چیست؟) مقاومت نشان دهد؟
تست بار یک نوع از تست است که در آن، شما می‌سنجید که تحت یک بار مشخص (مثلا حضور n کاربر به طور همزمان در سامانه) محصول شما چگونه کار می‌کند.

در این نوع تست، ما با هدف‌گذاری خاصی، بار را روی محصول زیاد می‌کنیم تا به آستانه عملکرد مطلوب نرم‌افزار برسیم.
ولی در تست استرس، ما نرم‌افزار را در فشار شدید تست می‌کنیم تا متوجه شویم نرم‌افزار چگونه این فشار را مدیریت می‌کند.
</p>

## تست بار

<p>

با شبیه‌سازی فشار در Production، آزمایش بار رفتار محصول را در شرایط اوج، عادی و مورد انتظار نشان می‌دهد. هدف تست این است که مطمئن شویم سیستم، می‌تواند آنچه را که برای آن طراحی شده است انجام دهد. (مثلا یک سایت بتواند در لحظه به 1000 کاربر سرویس دهد)
اهمیت این تست از این جهت است که هنگام توسعه محصول، فقط تعداد کمی از کاربران در استفاده از محصول در نظر گرفته می‌شود. تست بار به شما کمک می‌کند تا برای شرایط حساس در استفاده از نرم‌افزار آماده شوید. (مثلا لود 100000 داده در لحظه)

به طور کلی در تست بار ما اهداف زیر را دنبال می‌کنیم:

- **تعیین حداکثر نیازهای منابع سامانه (سخت افزار، پایگاه داده، شبکه و غیره)**: پس از انجام این تست میتوان تضمین کرد که برنامه، توانایی مدیریت هر باری را که در آینده در معرض آن قرار می‌گیرد دارد.
- **تشخیص عیوب در حالاتی که به سرریز بافر، سوء مدیریت حافظه و نشت حافظه مربوط می‌شود**: آزمایش بار برخی از مسائل از جمله مشکلات پهنای باند، مشکلات تعادل بار و ظرفیت سیستم را آشکار می‌کند.
 
</p>

### تست بار چگونه کار می‌کند؟

<p>

هنگام تست بار، سیستم زیر یک بار در حال افزایش می‌رود تا هنگامی که به آستانه مدنظر بار برسد. این تست به ما کمک می‌کند مشکلاتی از این قبیل را شناسایی کنیم.:
- مشکلات بارگذاری صفحه
- تاخیر در سامانه 
- موضوعات جانبی که هنگام دسترسی تعداد بالای کاربر به سامانه پیش می‌آید
</p>

<div style="text-align:center">
    <img src="https://devopedia.org/images/article/93/7154.1535360355.png" alt="Load Test vs. Stress Test" width="900px">
</div>

### چه زمانی تست فشار انجام دهیم؟

<p>

تست بار هنگامی آغاز می‌شود که در پایان مسیر توسعه محصول باشیم.
از نظر فنی، لازم نیست منتظر بمانیم تا توسعه نرم‌افزار قبل از آزمایش کامل شود. می‌توانیم یک جزء خاص را در هر مرحله از فرآیند توسعه آزمایش کنیم. با این حال، برای آزمایشِ تقاضای صدها هزار کاربر، بهتر است صبر کنیم تا توسعه تقریباً کامل شود. <br>
ابزارهای تست بار معمولاً اقدامات چندین کاربر همزمان را تقلید می‌کنند. این یک روش تکرارشونده است که شامل جمع‌آوری و نظارت بر آمار نرم‌افزاری و سخت‌افزاری است. در گزارش این تست به عملکرد موارد  زیر توجه می‌شود:

- CPU
- دیسک IO
- حافظه سرورهای فیزیکی

این تست زمان پاسخگویی و توان عملیاتی سیستم را به همراه سایر KPIها (چیست؟) نشان می‌دهد. برای شناسایی مشکلات Backend، بررسی این دو فاکتور مهم است: لود ایجاد شده در مدت زمان طولانی و  ورود همزمان کاربران.
پس از تست یک گزارش تولید می‌شود که نتایج این گزارش با اهداف مورد انتظار مقایسه می‌شود.

</p>

## آشنایی و کسب مهارت کارکردن با نرم افزار jmeter

<p>

محصول
[Apache JMeter™](https://jmeter.apache.org/)
یک نرم افزار منبع باز 
(Open-Source)
و بر پایه جاوا است. این نرم‌افزار طراحی شده تا بتواند عملکرد نرم‌افزارها را تست کند. <br>
**با** 
**Apache JMeter**
**چه کارهایی  می‌توان انجام داد؟** <br>
Apache JMeter
می‌تواند برای آزمایش عملکرد برنامه‌های کاربردی داینامیک وب 
(Web dynamic applications)
استفاده شود.
از این نرم‌افزار می‌توان برای شبیه‌سازی یک بار سنگین روی موارد زیر استفاده کرد:
- گروهی از سرورها
- شبکه 
- یا نرم‌افزاری که می‌خواهیم عملکرد کلی آن را تحت بارهای مختلف تحلیل و بررسی کنیم.

ویژگی‌های Apache JMeter عبارت است از:
- قابلیت بارگذاری و تست عملکرد بسیاری از انواع برنامه‌ها/سرور/انواع پروتکل مانند:
  - Web - HTTP, HTTPS (Java, NodeJS, PHP, ASP.NET, …)
  - SOAP / REST Webservices
  - FTP
  - Database via JDBC
  - LDAP
  - Message-oriented middleware (MOM) via JMS
  - Mail - SMTP(S), POP3(S) and IMAP(S)
  - Native commands or shell scripts
  - TCP
  - Java Objects
- [CLI mode](https://www.techtarget.com/searchwindowsserver/definition/command-line-interface-CLI#:~:text=A%20command%2Dline%20interface%20(CLI)%20is%20a%20text%2D,and%20interact%20with%20the%20computer.) 
- یک گزارش 
HTML
پویا، کامل و آماده برای ارائه

از طریق 
[این لینک](https://www.youtube.com/watch?v=SoW2pBak1_Q&t=7110s)
دوره کامل آموزش 
Apache JMeter
را ببینید.

</p>

### تمرین: اجرای مراحل بر روی یک api فرضی و تستی\

<p>

برای تست بار، سناریویی داخل DIA تشکیل داده و با استفاده از api ShortTimeServiceExecute (مستندش) ، به کمک jmeter، دو تست زیر را اجرا کنید:
1. یک threadgroup تشکیل داده که 50 نفر همزمان api را Call کنند.
2. سناریویی تشکیل داده که در ابتدا در هر ثانیه 1 Call صورت بگیرد و در طول یک دقیقه، به 5 کال در ثانیه برسد.

</p>
