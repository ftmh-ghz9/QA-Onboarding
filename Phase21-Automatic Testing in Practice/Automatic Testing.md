## تست خودکار (اتوماتیک)

<p>

تست خودکار یک تکنیک تست است که در آن، فرآیند ارزیابی کارکرد نرم‌افزار قبل از تحویل، به طور خودکار انجام می‌شود. با استفاده از تست خودکار، می‌توان تست‌هایی که اجرای آن به صورت دستی بوده را با سرعت خیلی بیشتری انجام داد. تست خودکار برای اجرای تست‌های بسیار بزرگ (تست کلی محصول) یا تست‌هایی با اجرای مداوم است (مانند 
Smoke Test
([چیست؟](https://www.techtarget.com/searchsoftwarequality/definition/smoke-testing#:~:text=Smoke%20testing%2C%20also%20called%20build,not%20delve%20into%20finer%20details.)) ). <br>
بزرگترین مزیت تست خودکار، این است که مقادیر زیادی از تست‌های دستی را به یک ریپازیتوری کد تبدیل و ساده‌سازی می‌کند. تست‌های خودکار می‌توانند به طور مکرر در هر زمانی از روز اجرا شوند و بخش بسیار مهمی از Continuous Integration و Continuous Delivery در رویه‌های توسعه نرم‌افزار هستند.

</p>

<p>

مراحل تست خودکار:
1. **یک ابزار تست را انتخاب کنید**. ابزار انتخاب شده بستگی به نوع تست دارد و  این ابزار باید از پلتفرمی که نرم‌افزار بر روی آن در حال توسعه است، پشتیبانی کند.
2. **محدوده اتوماسیون را تعریف کنید**. این بدان معناست که چه مقدار از تست‌های انجام شده روی نرم‌افزار، خودکار است.
3. **برنامه‌ریزی، طراحی و توسعه**: این مرحله شامل برنامه‌ریزی و توسعه کدهای تست است.
4. **اجرای تست**: در این مرحله، نرم‌افزار با استفاده از کدهای اتوماتیک تست می‌شود. ابزار تست همچنین باید داده‌ها را جمع‌آوری کرده و گزارش‌های دقیق تست را ارائه دهد.
5. **نگهداری کدها**: اسکریپت‌های تست خودکار در صورت نیاز با نسخه‌های جدیدتر اصلاح و به‌روز می‌شوند.

</p>

<p>

انواع تست‌های خودکار شامل موارد زیر است:
- [Acceptance tests](https://www.techtarget.com/searchsoftwarequality/definition/acceptance-test#:~:text=Acceptance%20testing%20is%20a%20quality,testing%20or%20end%2Duser%20testing.)
- [API tests](https://www.techtarget.com/searchapparchitecture/definition/API-testing)
- [Integration tests](https://www.techtarget.com/searchsoftwarequality/definition/integration-testing)
- [Regression tests](https://www.browserstack.com/guide/regression-testing#:~:text=Regression%20Testing%20is%20a%20type,the%20introduction%20of%20new%20changes.)
- [Smoke tests](https://www.techtarget.com/searchsoftwarequality/definition/smoke-testing#:~:text=Smoke%20testing%2C%20also%20called%20build,not%20delve%20into%20finer%20details.)
- [System tests](https://www.techtarget.com/searchsoftwarequality/definition/system-testing#:~:text=System%20testing%2C%20also%20referred%20to,full%2C%20integrated%20system%20or%20application.)
- [Unit tests](https://en.wikipedia.org/wiki/Unit_testing)
- [User interface (UI) tests](https://www.browserstack.com/guide/ui-testing-guide)

</p>

<div style="text-align:center">
    <img src="https://cdn.ttgtmedia.com/rms/onlineimages/software_quality-test_types-f.png" alt="Load Test vs. Stress Test" width="700px">
</div>

<p>

فریمورک ([چیست؟](https://www.codecademy.com/resources/blog/what-is-a-framework/))های مرسوم تست خودکار به شرح زیر هستند:
- [Data-Driven Frameworks](https://testsigma.com/data-driven-testing)
- [Keyword-driven Frameworks](https://www.guru99.com/keyword-driven-testing.html) 
- [linear scripting framework](https://www.softwaretestingmaterial.com/types-test-automation-frameworks/#Linear-Scripting-Framework)
- [modular testing framework](https://www.softwaretestingmaterial.com/types-test-automation-frameworks/#Modular-Testing-Framework)

فریمورک اسکریپت خطی برای برنامه‌های کاربردی کوچک مناسب است، زیرا استفاده از یک اسکریپت آزمایشی را با برنامه‌ریزی کمتر امکان پذیر می‌کند. اما این اسکریپت‌ها قابل استفاده مجدد نیست. فریمورک تست ماژولار، اسکریپت‌هایی را به‌عنوان تست‌های کوچک و مستقل ایجاد می‌کند تا افزونگی را کاهش دهد، اما این فرآیند معمولاً زمان بیشتری نیاز دارد.
با فریمورک‌های مبتنی بر داده 
(Data-Driven)
، می‌توان اسکریپت‌هایی نوشت که برای مجموعه‌های داده‌های متعدد کار کند. این نوع فریمورک‌ها پوشش گسترده‌تری را با آزمایش‌های کمتر، نسبت به فریمورک‌های ماژولار، ارائه می‌دهند. <br>
ابزارها و فریمورک‌های تست خودکار شامل 
Selenium،
Robot Framework
و 
Cypress
هستند.
[Robot Framework](https://robotframework.org/)
به تسترها کمک می‌کند تا تست‌های 
User acceptance،
Performance,
System acceptance
را برای دستگاه‌های 
Android
توسعه دهند.
Cypress
تست‌های 
end-to-end،
Integration
و 
Unit
را در یک مرورگر پوشش می‌دهد.

</p>

### Xray

<p>

Xray
یک ابزار مدیریت تست کامل برای 
Jira
است. این یک برنامه با امکانات کامل است که برای اجرا به نرم افزار دیگری نیاز ندارد.
از کل چرخه عمر تست پشتیبانی می‌کند:
-  برنامه ریزی تست
- طراحی تست
- اجرای تست 
- گزارش تست

Xray
این کار را با استفاده از ایشو تایپ‌های 
Jira
انجام می‌دهد، بنابراین می‌توانید از تمام مزایای 
Jira
که استفاده کنید.
هدف 
Xray
کمک به شرکت‌ها در بهبود کیفیت سیستم‌های خود از طریق تست موثر و کارآمد است. به همین دلیل است که 
Xray
در حال حاضر از تست‌های دستی و خودکار، از جمله 
BDD
(مانند: 
Cucumber،
SpecFlow،
Serenity BDD)
پشتیبانی می‌کند.

</p>