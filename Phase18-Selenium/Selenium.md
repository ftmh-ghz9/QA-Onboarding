## Selenium

<p>

سلنیوم یا
[Selenium](https://www.selenium.dev/)
یک ابزار بسیار مفید برای تست اتوماتیک سرویس‌های تحت وب است. 
Selenium
به صورت شبیه‌سازی شده، یک مرورگر را در سیستم‌عامل باز می‌کند و دستورات (کدهای) نوشته شده را توسط مرورگر، خط به خط اجرا می‌کند و بعد از انجام دستورات، بسته می‌شود.<br>
سلنیوم را می‌توان به صورت یک کتابخانه در 
python
استفاده کرد ولی قبل از آن نیاز است که 
WebDriver
آن را نصب کرده باشید. از طریق [این لینک](https://www.selenium.dev/downloads/) می‌توانید 
WebDriver
مربوط به سلنیوم را دانلود کنید.
ویدیوی آموزش نحوه نوشتن کد پایتون سلنیوم و اجرای آن را از طریق [این لینک](https://drive.google.com/file/d/1NnVwLjBs3fQ2uXCYpCwfKvETyrYWSkSR/view) ببینید.

</p>

<div style="text-align:center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Selenium_Logo.png/1200px-Selenium_Logo.png" alt="Selenium" width="300px">
</div>

### تمرین: پیاده‌سازی یک سناریوی تست شبه‌واقعی روی Booking.com

<p>

پس از آموزش کامل دوره سلنیوم، در این پروژه شما قرار است یک سناریوی تست را در یک سایت معروف (Booking.com) انجام دهید. لازم به ذكر است برای انجام این روال شما مجاز به استفاده از تمام كتابخانه‌های مرسوم selenium خواهید بود و محدودیت خاصی در این بخش نخواهید داشت. <br>
شما بایستی سناریوی زیر را با استفاده از سلنیوم در پایتون اجرا کنید و کد نهایی را برای mentor خود ارسال کنید. همچنین یک بار نیز کد را برای mentor خود اجرا کنید.

</p>

<p>

**سناریوی تست:**

1. اول سایت 
Booking.com
را باز کند و ارز را به 
USD
تغییر دهد. (مانند تصاویر)

<div style="text-align:center">
    <img src="FirstStep.png" alt="First Step" width="900px">
</div>
<div style="text-align:center">
    <img src="FirstStep1.png" alt="First Step" width="900px">
</div>

2. سپس فیلد شهر مقصد را با شهر دلخواه (مثلا 
Paris)
پر کند و شهر مدنظر را انتخاب کند. (مشابه عکس) 
<div style="text-align:center">
    <img src="SecondStep.png" alt="Second Step" width="900px">
</div>

3. سپس تاریخی دلخواه را انتخاب کند. (کد نوشته شده باید قادر باشد در صورت انتخاب ماه‌های آینده با ورق زدن صفحه تاریخ ماه مدنظر را پیدا کند، همچنین باید تمامی حالات انتخاب ماه در کد در نظر گرفته شود -مانند انتخاب روزهایِ ماه ورودی و خروجی در آن‌ها متفاوت است.-)
<div style="text-align:center">
    <img src="ThirdStep.png" alt="Third Step" width="900px">
</div>

4. سپس تعداد 
Adult
را به تعداد دلخواه تغییر دهد.
<div style="text-align:center">
    <img src="FourthStep.png" alt="Fourth Step" width="900px">
</div>

5. بعد انجام جستجو تا پایین صفحه 
Scroll
کند و وارد صفحه بعد شود.
<div style="text-align:center">
    <img src="FifthStep.png" alt="Fifth Step" width="900px">
</div>
<div style="text-align:center">
    <img src="FifthStep1.png" alt="Fifth Step" width="900px">
</div>

</p>