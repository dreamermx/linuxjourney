# مجوزهای فایل

## محتویات درس

همانطور که پیشتر یاد گرفتیم، فایل‌ها مجوز و مُدهای مختلفی دارند. بگذارید با یک مثال نگاهی دقیق‌تر به آن بیندازیم:

<pre>$ ls -l Desktop/
drwxr-xr-x 2 pete penguins 4096 Dec 1 11:45 .
</pre>

در قسمت مجوز‌های فایل چهار قسمت وجود دارد. قسمت اول نوع فایل است که  توسط اولین کارکترِ قسمت مجوز‌ها مشخص شده است. در این مثال، ما در حال بررسی یک دایرکتوری یا به عبارت ساده پوشه هستیم و به همین خاطر این کاراکتر حرف <b>d</b> را برای نوع فایل نشان می‌دهد. در اکثر موراد شما با کاراکتر <b>-</b> برای فایل‌های معمولی مواجه خواهید شد.

سه قسمت بعدی در فایل‌مُد ما مجوزهای موجود فایل است. هر مجوز به سه گروه مجزا که هر کدام به سه بیت تقسیم شده‌اند، دسته‌بندی شده‌اند. سه بیت ابتدایی مجوزهای مربوط به کاربر "user" را نشان می‌دهد و سپس مجوزهای مربوط به گروه "group" و بعد از آن  مجوزهای سایر قرار گرفته‌اند. در مثال زیر با توجه به لوله‌های بین آن‌ها می‌توانید تفاوت را به وضوح ببینید.

<pre>d | rwx | r-x | r-x </pre>

هر کاراکتر نشان‌دهنده‌ی مجوزهای متفاوتی است.

<ul>
<li>r: قابل خواندن</li>
<li>w: قابل نوشتن</li>
<li>x: قابل اجرا (در اصل یک برنامه‌ی قابل اجرا)</li>
<li>-: خالی</li>
</ul>

خب در مثال بالا، ما می‌بینیم که کاربر pete تمام مجوزهای مربوط به خواندن، نوشتن و اجرا را دارد. گروه پنگوئن‌ها یا penguins نیز قادر به خواندن و اجرای فایل است. و در نهایت سایر کاربرها (شامل تمام افرادی که فایل در دسترس ایشان است) مجوزهای خواندن و اجرا را دارند.

## تمرین

با استفاده از دستور ls -l بر روی چندین فایل مجوزهای آن‌ها و همچنین گروه و کاربرشان را مشخص کنید.

## سوال آزمون

کدام قسمت مجوز نشان‌دهنده‌ی قابلیت اجرای فایل است؟

## پاسخ آزمون

x
