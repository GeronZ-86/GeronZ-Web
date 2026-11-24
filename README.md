<div align="center">

# GeronZ-Web

### 🌐 [geronz.me](https://geronz-86.github.io/GeronZ-Web/)

**پورتفولیوی شخصی — توسعه‌دهنده فرانت‌اند، بازی و طراح دوبعدی/سه‌بعدی**

[🌐 مشاهده سایت](https://geronz-86.github.io/GeronZ-Web/) · [🐛 گزارش مشکل](https://github.com/GeronZ-86/GeronZ-Web/issues) · [💬 تماس](https://t.me/GeronZ_DeV)

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![Languages](https://img.shields.io/badge/lang-FA%20%7C%20EN%20%7C%20RU-D9B45F?style=flat-square)
![No Framework](https://img.shields.io/badge/framework-none-black?style=flat-square)

</div>

---

## 📸 پیش‌نمایش

<div align="center">

![پیش‌نمایش سایت](./img/og-cover.jpg)

</div>

---

<div dir="rtl">

## ✨ ویژگی‌ها

- 🎨 **تم تاریک/طلایی** با طراحی مدرن و ظریف
- 🌐 **سه‌زبانه کامل** (فارسی، انگلیسی، روسی) با حفظ انتخاب کاربر در `localStorage`
- 📱 **کاملاً واکنش‌گرا** — بهینه‌شده برای موبایل، تبلت و دسکتاپ (بدون اسکرول افقی)
- ✉️ **فرم تماس فعال** — متصل به Formspree با اعتبارسنجی کامل و حالت لودینگ
- 🚫 **صفحه ۴۰۴ سفارشی** — سه‌زبانه و هماهنگ با تم سایت
- ♿ **دسترس‌پذیر** — ARIA، `focus-visible`، `prefers-reduced-motion`
- ⚡ **بدون فریم‌ورک** — HTML/CSS/JS خالص، سریع و سبک
- 🔒 **امن** — مخفی‌سازی ایمیل با Base64، `noopener noreferrer`، referrer policy
- 🤖 **آماده برای SEO** — دارای `robots.txt` و `sitemap.xml`
- 🎭 **انیمیشن‌های ظریف** در هاور
- 🎯 **متغیرهای CSS** برای شخصی‌سازی آسان

---

## 🛠 تکنولوژی‌ها

<table>
  <thead>
    <tr>
      <th>فناوری</th>
      <th>کاربرد</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><b>HTML5</b></td><td>ساختار معنایی و دسترس‌پذیر</td></tr>
    <tr><td><b>CSS3</b></td><td>Grid، Flexbox، متغیرها، Media Queries</td></tr>
    <tr><td><b>JavaScript (Vanilla)</b></td><td>تعویض زبان، منوی موبایل، مخفی‌سازی ایمیل، ارسال فرم</td></tr>
    <tr><td><b>Formspree</b></td><td>دریافت پیام‌های فرم تماس بدون نیاز به بک‌اند</td></tr>
    <tr><td><b>Vazirmatn</b></td><td>فونت فارسی (Google Fonts)</td></tr>
    <tr><td><b>SVG</b></td><td>آیکن‌های درون‌خطی برندها</td></tr>
  </tbody>
</table>

---

## 📁 ساختار پروژه

<table>
  <thead>
    <tr>
      <th>فایل / پوشه</th>
      <th>توضیح</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><code>index.html</code></td><td>کل سایت (HTML + CSS + JS)</td></tr>
    <tr><td><code>404.html</code></td><td>صفحه خطای سفارشی سه‌زبانه</td></tr>
    <tr><td><code>robots.txt</code></td><td>راهنمای ربات‌های جستجو</td></tr>
    <tr><td><code>sitemap.xml</code></td><td>نقشه سایت برای گوگل</td></tr>
    <tr><td><code>README.md</code></td><td>همین فایل</td></tr>
    <tr><td><code>img/</code></td><td>پوشه‌ی تصاویر</td></tr>
    <tr><td><code>img/G.jpg</code></td><td>تصویر پروفایل</td></tr>
    <tr><td><code>img/favicon.svg</code></td><td>آیکن تب مرورگر</td></tr>
    <tr><td><code>img/og-cover.jpg</code></td><td>تصویر پیش‌نمایش شبکه‌های اجتماعی</td></tr>
    <tr><td><code>img/warBorn.jpg</code></td><td>تصویر پروژه</td></tr>
    <tr><td><code>img/Jojaa.jpg</code></td><td>تصویر پروژه</td></tr>
    <tr><td><code>img/shepherd.jpg</code></td><td>تصویر پروژه</td></tr>
    <tr><td><code>img/BWR.jpg</code></td><td>تصویر پروژه</td></tr>
    <tr><td><code>img/IslandMen.jpg</code></td><td>تصویر پروژه</td></tr>
  </tbody>
</table>

---

## 🚀 اجرای محلی

### روش ۱ — بدون سرور (ساده‌ترین)

</div>

```bash
git clone https://github.com/GeronZ-86/GeronZ-Web.git
cd GeronZ-Web
```

<div dir="rtl">

سپس فایل `index.html` را در مرورگر باز کن. تمام.

### روش ۲ — با سرور محلی (توصیه‌شده برای تست کامل)

</div>

```bash
# با Python
python -m http.server 8000

# یا با Node.js
npx serve .

# یا با PHP
php -S localhost:8000
```

<div dir="rtl">

سپس `http://localhost:8000` را باز کن.

> **چرا سرور محلی؟** چون بعضی رفتارها (مثل `localStorage` و مسیرهای نسبی) ممکن است در حالت `file://` متفاوت باشند.

---

## 🌐 تعویض زبان

سه زبان پشتیبانی می‌شود: **فارسی (`fa`)**، **انگلیسی (`en`)**، **روسی (`ru`)**

### نحوه‌ی کار

1. کاربر روی دکمه‌ی زبان در هدر کلیک می‌کند.
2. تابع `applyLang()` تمام عناصر دارای `data-i18n`، `data-i18n-html` و `data-i18n-placeholder` را جایگزین می‌کند.
3. انتخاب در `localStorage` با کلید `geronz-lang` ذخیره می‌شود.
4. جهت صفحه خودکار بین `rtl` و `ltr` تغییر می‌کند.

### افزودن زبان جدید

در انتهای `index.html`، آبجکت `i18n` را گسترش بده:

</div>

```js
i18n.de = {
  'nav.home': 'Startseite',
  'nav.about': 'Über mich',
  // ... بقیه کلیدها
};
```

<div dir="rtl">

و یک دکمه به `.lang-switcher` اضافه کن:

</div>

```html
<button type="button" data-set-lang="de" aria-pressed="false">DE</button>
```

<div dir="rtl">

---

## ✉️ فرم تماس (Formspree)

فرم تماس سایت به سرویس **Formspree** متصل است تا بدون نیاز به سرور یا بک‌اند، پیام‌ها مستقیم به ایمیل شما ارسال شوند.

برای تغییر ایمیل دریافت‌کننده، کافیست در کد JavaScript (بخش `initContactForm`) مقدار `FORM_ENDPOINT` را با لینک جدید خود در Formspree جایگزین کنید.

---

## 🚢 استقرار روی GitHub Pages

1. به **Settings → Pages** برو
2. **Source** را روی `Deploy from a branch` بگذار
3. **Branch** را `main` و پوشه را `/ (root)` انتخاب کن
4. **Save** کن
5. بعد از ۱–۲ دقیقه، سایت در `https://GeronZ-86.github.io/GeronZ-Web/` در دسترس است
6. 🔒 **حتماً گزینه‌ی `Enforce HTTPS` را فعال کن**
7. ⚠️ **نکته مهم:** حتماً فایل `.nojekyll` در ریشه پروژه وجود داشته باشد تا GitHub Pages فایل‌های شما را بدون پردازش Jekyll سرو کند (مخصوصاً برای صفحه ۴۰۴).

### دامنه‌ی اختصاصی (اختیاری)

اگر دامنه‌ای مثل `geronz.me` داری:

1. یک فایل `CNAME` در ریشه بساز و فقط دامنه را داخلش بنویس: `geronz.me`
2. در پنل DNS دامنه، رکوردهای `A` و `CNAME` را طبق [مستندات GitHub](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) تنظیم کن.

---

## 🔒 نکات امنیتی

<table>
  <thead>
    <tr>
      <th>مورد</th>
      <th>پیاده‌سازی</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><b>مخفی‌سازی ایمیل</b></td><td>ایمیل به Base64 تبدیل شده و فقط با JS دیکد می‌شود</td></tr>
    <tr><td><b>فرم تماس</b></td><td>ارسال امن از طریق API سرویس Formspree (بدون دخالت بک‌اند شخصی)</td></tr>
    <tr><td><b>هانی‌پات (Honeypot)</b></td><td>فیلد مخفی <code>_gotcha</code> برای جلوگیری از ارسال پیام‌های اسپم ربات‌ها</td></tr>
    <tr><td><b>لینک‌های خارجی</b></td><td>همه دارای <code>rel="noopener noreferrer"</code></td></tr>
    <tr><td><b>Referrer</b></td><td><code>&lt;meta name="referrer" content="strict-origin-when-cross-origin"&gt;</code></td></tr>
    <tr><td><b>HTTPS</b></td><td>فعال از GitHub Pages</td></tr>
    <tr><td><b>اسکریپت‌های شخص ثالث</b></td><td>فقط Google Fonts (معتبر) و Formspree (برای فرم)</td></tr>
  </tbody>
</table>

---

## 🎨 شخصی‌سازی

### تغییر رنگ‌ها

در `index.html`، ابتدای `<style>`، متغیرها را تغییر بده:

</div>

```css
:root {
  --gold: #D9B45F;        /* رنگ اصلی */
  --gold-light: #F0D48A;  /* رنگ روشن‌تر (تیترها) */
  --bg: #0a0a0a;          /* پس‌زمینه */
  --item-bg: #232323;     /* پس‌زمینه کارت‌ها */
  --border: #2a2a2a;      /* رنگ حاشیه */
  --header-h: 64px;       /* ارتفاع هدر */
}
```

<div dir="rtl">

---

## 🧪 چک‌لیست قبل از انتشار

- [ ] همه‌ی تصاویر در `img/` موجودند و مسیرها دقیقاً با کد HTML مطابقت دارند.
- [ ] `Enforce HTTPS` در تنظیمات Pages فعال است.
- [ ] فایل `.nojekyll` در ریشه وجود دارد.
- [ ] فایل‌های `404.html`، `robots.txt` و `sitemap.xml` آپلود شده‌اند.
- [ ] لینک‌های شبکه‌های اجتماعی به پروفایل‌های واقعی اشاره می‌کنند.
- [ ] متای `og:image` به یک فایل واقعی اشاره می‌کند.
- [ ] سایت در حالت موبایل (بدون اسکرول افقی) و دسکتاپ تست شده است.
- [ ] فرم تماس پیام را با موفقیت به ایمیل شما ارسال می‌کند.
- [ ] تعویض زبان در هر سه زبان و در صفحه ۴۰۴ کار می‌کند.

---

## 📮 ارتباط

<table>
  <thead>
    <tr>
      <th>پلتفرم</th>
      <th>لینک</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>🌐 وب‌سایت</td><td><a href="https://geronz-86.github.io/GeronZ-Web/">geronz-86.github.io/GeronZ-Web</a></td></tr>
    <tr><td>💬 تلگرام</td><td><a href="https://t.me/GeronZ8">@GeronZ_DeV</a></td></tr>
    <tr><td>🐙 گیت‌هاب</td><td><a href="https://github.com/GeronZ-86">@GeronZ-86</a></td></tr>
    <tr><td>💼 لینکدین</td><td><a href="https://www.linkedin.com/in/sobhan-hosseini-a57991384">sobhan-hosseini</a></td></tr>
    <tr><td>🐦 X (توییتر)</td><td><a href="https://x.com/sobh_n86">@sobh_n86</a></td></tr>
    <tr><td>📷 اینستاگرام</td><td><a href="https://instagram.com/sobha.n8668">@sobha.n8668</a></td></tr>
    <tr><td>📺 یوتیوب</td><td><a href="https://youtube.com/@GeronZ-86">@GeronZ-86</a></td></tr>
    <tr><td>📌 پینترست</td><td><a href="https://pinterest.com/hsbhan6366">hsbhan6366</a></td></tr>
  </tbody>
</table>

---

## 📄 مجوز

این پروژه تحت مجوز **MIT** منتشر شده است — استفاده، تغییر و توزیع آزاد است. لطفاً attribution را حفظ کن.

</div>

---

<div align="center" dir="rtl">

**ساخته شده با ☕ و 🖤 توسط GeronZ**

اگر این پروژه برایت الهام‌بخش بود، یک ⭐ به ریپازیتوری بده

</div>