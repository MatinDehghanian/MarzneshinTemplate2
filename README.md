<h1 align="center"/>تمپلیت برای پنل  <a href="https://github.com/marzneshin/marzneshin">مرزنشین</a></h1>

# مقدمه
 تمپلیت شخصی سازی شده برای مرزنشین


# نصب
برای نصب تمپلیت دستورات زیر را در ترمینال سرور خود اجرا کنید:
1. دانلود فایل تمپلیت
```sh
sudo wget -N -P /var/lib/marzneshin/templates/subscription/ https://raw.githubusercontent.com/MatinDehghanian/marzneshin-template/master/subscription/index.html
```
2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzneshin/templates/"' | sudo tee -a /etc/opt/marzneshin/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /etc/opt/marzneshin/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/etc/opt/marzneshin` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzneshin/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
```

3. ری استارت مرزنشین
```sh
marzneshin restart
```

## بروزرسانی
برای بروزرسانی تمپلیت ها فقط کافیست مرحله 1 را تکرار کنید.


## حمایت و سفارش
برای سفارش تمپلیت اختصاصی خودتون توی <a href="https://t.me/Mqtin">تلگرام</a> با من در ارتباط باشین.

<a href="https://nowpayments.io/donation?api_key=Z50AKDD-DHSMN86-P0DQ22X-1SQAFCA" target="_blank" rel="noreferrer noopener">
    <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments">
</a>
