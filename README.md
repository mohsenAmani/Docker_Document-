# Docker_Document
Document about Docker learning
 
<p align="center">
 <img alt="Docker-Logo" src="image/docker.png">
</p>
</br>
<p dir=rtl>
  docker info </br>
  docker run hello-world </br>
  docker images </br>
 docker images -a </br>
 docker images -q </br>
 docker image ls </br>
 docker run -it centos:latest </br>
 docker run -it -d centos:latest /bin/bash </br>
 docker ps -a </br>
 docker ps -s </br>
docker ps -q </br>
docker ps -n=3 </br>
docker rm {CONTAINER ID} | {CONTAINER NAME} </br>
docker rm -f {CONTAINER ID} | {CONTAINER NAME} </br>
docker rm -f $(docker ps -aq) </br>
docker rm $(docker ps -a -q -f status=exited) </br>
docker ps --format '{{.Names}}' </br>
docker ps -a --format '{{.Names}}' -f status='exited' </br>
docker ps -a -q -f status='exited' </br>
docker ps -lq </br>
docker rm -f $(docker ps -aq -n=5) </br>
docker rm -f $(docker ps -aq -l) </br>
 docker cp /opt/moh3n.txt 7d3ea77490a6:/home </br>





 cd /var/lib/docker/ </br>
 
 
 
 
</p>
<hr>
<p dir=rtl>
<b>1- Elasticsearch:</b></br> یک موتور متن باز آنالیز و جستجوی Full-Text و مبتنی بر موتور جستجوی Apache Lucene است.
</br></br>
<b>2- Logstash:</b></br> یک جمع کننده لاگ است که داده ها را از منابع مختلف ورودی جمع آوری می‌کند، تغییرات و پیشرفت های مختلف را اجرا می‌کند و سپس داده ها را به مقصد های مختلف خروجی ارسال می‌کند.
</br></br>
<b>3- Kibana:</b></br> یک لایه تجسمی است که در بالای Elasticsearch کار می‌کند، توانایی تجزیه و تحلیل و تجسم داده ها را به کاربران ارائه می‌دهد. 
</br></br>
<b>4- و آخرین مورد Beats:</b></br> در اصل agent های سبکی هستند که روی میزبان‌های edge نصب می‌شوند تا انواع مختلف داده‌ها را برای ارسال به پشته جمع آوری کنند.
</br>
 </p><hr>
 <p dir=rtl>
در کنار هم، Beats و Logstash مسئولیت جمع‌آوری و پردازش داده‌ها را در دست دارند، Elasticsearch داده‌ها را فهرست‌بندی و ذخیره می‌کند و Kibana یک رابط کاربری برای جستجوی داده‌ها و تجسم آنها فراهم می‌کند
  </p>


<h3 dir=rtl>
  اصطلاحات رایج در docker:
</h3>

<table>
  <tr>
    <th><b><i>اصطلاح</i></b></th>
    <th><b><i>توضیحات</i></b></th>
  </tr>
  <tr>
    <td><b>Repo</b></td>
    <td dir=rtl>این اصطلاح برگرفته از واژه Repository به معنی «مخزن» یا «منبع» است</td>
  </tr>
  <tr>
    <td><b>Clone</b></td>
    <td dir=rtl> چنانچه بخواهیم یک ریپازیتوری آنلاین را دریافت نموده و روی سیستم لوکال خود شروع به کار روی آن نماییم، نیاز است تا ابتدا کل پروژه را دانلود نماییم که به این کار کلون کردن گفته می‌شود. </td>
  </tr>
</table>

</br>
<h3 dir=rtl>
  دستورات رایج در Docker:
</h3>

<table>
  <tr>
    <th><b><i>دستورات</i></b></th>
    <th><b><i>توضیحات</i></b></th>
  </tr>
  <tr>
    <td><b>git init</b></td>
    <td dir=rtl> کامند init برگرفته از کلمه Initialize به معنی «شروع کردن» است. پس از اجرای موفقیت‌آمیز این کامند،‌ پوشه‌ای تحت عنوان git. ساخته می‌شود </td>
  </tr>
  <tr>
    <td><b></b></td>
    <td dir=rtl>  </td>
  </tr>
  </table>

</br>
<h3 dir=rtl>
  سایر دستورات در Docker:
</h3>

<table>
  <tr>
    <th><b><i>دستورات</i></b></th>
    <th><b><i>توضیحات</i></b></th>
  </tr>
  <tr>
    <td></br><b>git tag</br>git tag -a V2.0 -m 'کامنت'</br>git tag -l "v*"</br>git show V2.0</br>git push origin V2.0</br>git push origin --tags</br>git checkout V2.0</b></br></td>
    <td dir=rtl>مشاهده تگ ها</br>اضافه کردن تگ با کامنت مناسب</br>دیدن همه تگ ها که با حرف v شروع میشن</br>دیدن جزییات برای لاگی که تگ V2.0 دارد</br>اعمال تغییرات بر روی گیت هاب با تگ بجای شماره کامیت</br>اعمال تگ های ایجاد شده به گیت هاب</br>رفتن به تگ V2.0</td>
  </tr>
  <tr>
    <td><b>git help blame</br>git blame {اسم فایل} -L{شماره خط یا رنجی از خط ها}</b></td>
    <td dir=rtl>برای پیدا کردن آخرین شخصی که خط از فایل رو تغییر داده</td>
  </tr>
  </table>
