```markdown
# GeronZ-Web

<div align="center">

# GeronZ.me

پورتفولیوی شخصی — توسعه‌دهنده فرانت‌اند، بازی و طراح دوبعدی/سه‌بعدی

[🌐 مشاهده سایت](https://geronz-86.github.io/GeronZ-Web/) · [🐛 گزارش مشکل](https://github.com/GeronZ-86/GeronZ-Web/issues) · [💬 تماس](https://t.me/GeronZ8)

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![Languages](https://img.shields.io/badge/lang-FA%20%7C%20EN%20%7C%20RU-D9B45F?style=flat-square)
![No Framework](https://img.shields.io/badge/framework-none-black?style=flat-square)

</div>

---

## 📸 پیش‌نمایش

![پیش‌نمایش سایت](./preview.jpg)

---

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

| فناوری | کاربرد |
|---|---|
| **HTML5** | ساختار معنایی و دسترس‌پذیر |
| **CSS3** | Grid، Flexbox، متغیرها، Media Queries |
| **JavaScript (Vanilla)** | تعویض زبان، منوی موبایل، مخفی‌سازی ایمیل، ارسال فرم |
| **Formspree** | دریافت پیام‌های فرم تماس بدون نیاز به بک‌اند |
| **Vazirmatn** | فونت فارسی (Google Fonts) |
| **SVG** | آیکن‌های درون‌خطی برندها |

---

## 📁 ساختار پروژه

```text
GeronZ-Web/
├── index.html              # کل سایت (HTML + CSS + JS)
├── 404.html                # صفحه خطای سفارشی سه‌زبانه
├── robots.txt              # راهنمای ربات‌های جستجو
├── sitemap.xml             # نقشه سایت برای گوگل
├── README.md
└── img/
    ├── G.jpg               # تصویر پروفایل
    ├── favicon.svg         # آیکن تب مرورگر
    ├── og-cover.jpg        # تصویر پیش‌نمایش شبکه‌های اجتماعی
    ├── warBorn.jpg
    ├── Jojaa.jpg
    ├── shepherd.jpg
    ├── BWR.jpg
    └── IslandMen.jpg
```

---

## 🚀 اجرای محلی

### روش ۱ — بدون سرور (ساده‌ترین)

```bash
git clone https://github.com/GeronZ-86/GeronZ-Web.git
cd GeronZ-Web
```

سپس فایل `index.html` را در مرورگر باز کن. تمام.

### روش ۲ — با سرور محلی (توصیه‌شده برای تست کامل)

```bash
# با Python
python -m http.server 8000

# یا با Node.js
npx serve .

# یا با PHP
php -S localhost:8000
```

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

```js
i18n.de = {
  'nav.home': 'Startseite',
  'nav.about': 'Über mich',
  // ... بقیه کلیدها
};
```

و یک دکمه به `.lang-switcher` اضافه کن:

```html
<button type="button" data-set-lang="de" aria-pressed="false">DE</button>
```

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

| مورد | پیاده‌سازی |
|---|---|
| **مخفی‌سازی ایمیل** | ایمیل به Base64 تبدیل شده و فقط با JS دیکد می‌شود |
| **فرم تماس** | ارسال امن از طریق API سرویس Formspree (بدون دخالت بک‌اند شخصی) |
| **هانی‌پات (Honeypot)** | فیلد مخفی `_gotcha` برای جلوگیری از ارسال پیام‌های اسپم ربات‌ها |
| **لینک‌های خارجی** | همه دارای `rel="noopener noreferrer"` |
| **Referrer** | `<meta name="referrer" content="strict-origin-when-cross-origin">` |
| **HTTPS** | فعال از GitHub Pages |
| **اسکریپت‌های شخص ثالث** | فقط Google Fonts (معتبر) و Formspree (برای فرم) |

---

## 🎨 شخصی‌سازی

### تغییر رنگ‌ها

در `index.html`، ابتدای `<style>`، متغیرها را تغییر بده:

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

<div align="center">

| پلتفرم | لینک |
|---|---|
| 🌐 وب‌سایت | [geronz-86.github.io/GeronZ-Web](https://geronz-86.github.io/GeronZ-Web/) |
| 💬 تلگرام | [@GeronZ8](https://t.me/GeronZ8) |
| 🐙 گیت‌هاب | [@GeronZ-86](https://github.com/GeronZ-86) |
| 💼 لینکدین | [sobhan-hosseini](https://www.linkedin.com/in/sobhan-hosseini-a57991384) |
| 🐦 X | [@sobh_n86](https://x.com/sobh_n86) |
| 📷 اینستاگرام | [@sobha.n8668](https://instagram.com/sobha.n8668) |
| 📺 یوتیوب | [@GeronZ-86](https://youtube.com/@GeronZ-86) |
| 📌 پینترست | [hsbhan6366](https://pinterest.com/hsbhan6366) |

</div>

---

## 📄 مجوز

این پروژه تحت مجوز **MIT** منتشر شده است — استفاده، تغییر و توزیع آزاد است. لطفاً attribution را حفظ کن.

---

<div align="center">

**ساخته شده با ☕ و 🖤 توسط GeronZ**

اگر این پروژه برایت الهام‌بخش بود، یک ⭐ به ریپازیتوری بده

</div>
```
