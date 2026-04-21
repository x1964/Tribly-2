Tribly 🌿
منصة التواصل الاجتماعي التي تجمعك بأصحابك بطريقة مختلفة

The next-generation social platform connecting communities

📍 Alexandria, Egypt 🇪🇬 · 🏙️ 4 Cities · 👥 638+ Users

📖 نبذة عن المشروع | About
Tribly هي منصة تواصل اجتماعي جديدة بالكامل، مصممة لربط المجتمعات المحلية بطريقة مبتكرة ومختلفة. نعمل حالياً على تطوير المنصة لتقديم تجربة فريدة تجمع بين البساطة والقوة.

Tribly is a next-generation social platform designed to connect local communities in innovative ways. Currently under active development to deliver a unique experience that combines simplicity with power.

✅ قائمة فحص SEO | SEO Checklist
#	العنصر	الحالة	Description
1	Meta Title	✅	مُحسّن بأقل من 60 حرفاً
2	Meta Description	✅	مُحسّن بأقل من 160 حرفاً
3	Canonical URL	✅	محدد بشكل صحيح
4	Open Graph Tags	✅	og:title, og:description, og:image, og:url
5	Twitter Cards	✅	twitter:card, twitter:title, twitter:image
6	hreflang Tags	✅	ar + en بدائل اللغات
7	Structured Data	✅	JSON-LD (WebSite + Organization)
8	Sitemap.xml	✅	يتضمن صور وفيديو وبدائل لغات
9	Robots.txt	✅	مسموح للجميع مع Sitemap
10	Semantic HTML	✅	header, main, section, footer
11	Alt Text Images	✅	نصوص بديلة لجميع الصور
12	Mobile Responsive	✅	تصميم متجاوب بالكامل
13	Core Web Vitals	✅	LCP, FID, CLS ضمن المعايير
14	HTTPS	✅	شهادة SSL نشطة عبر Cloudflare
15	PWA Manifest	✅	manifest.json مع جميع الأيقونات
16	Security.txt	✅	ملف الأمان متاح عند المسار المعتمد
17	Favicon Set	✅	جميع الأحجام متوفرة
18	Theme Color	✅	لون الثيمة محدد
19	Language Attribute	✅	lang="ar" dir="rtl"
20	Preconnect Hints	✅	DNS prefetch للـ CDN
📊 نتائج Lighthouse | Lighthouse Scores
الفحص	النتيجة	الحالة
Performance	100	🟢
Accessibility	100	🟢
Best Practices	100	🟢
SEO	100	🟢
PWA	100	🟢
جميع النتائج مقاسة على اتصال 4G محاكى مع تقليل السرعة 4x (Mobile)

🛠️ التقنيات المستخدمة | Tech Stack
Frontend
HTML5
CSS3
JavaScript
PWA
Backend
PHP
MySQL
Hosting & CDN
GitHub Pages
InfinityFree
Cloudflare
📁 هيكل الملفات | File Structure
tribly.online/
├── index.html # PWA + SSR Coming Soon Page
├── sitemap.xml # Sitemap with images, video, hreflang
├── robots.txt # Crawl directives + sitemap reference
├── manifest.json # PWA manifest (icons, theme, display)
├── security.txt # Security contact & policy
├── README.md # Project documentation
└── img/
├── maskable_icon.png # 512×512 Maskable PWA icon
├── og-image.png # 1200×630 Open Graph image
├── favicon-32x32.png # Standard favicon
└── apple-touch-icon.png # 180×180 Apple touch icon

text


---

## 🚀 خطوات النشر | Deployment

### المتطلبات المسبقة | Prerequisites

- حساب GitHub
- حساب Cloudflare (خطة مجانية)
- حساب InfinityFree (خطة مجانية)
- نطاق مخصص (tribly.online)

### الخطوة 1: إعداد المستودع

```bash
git clone https://github.com/tribly/tribly.online.git
cd tribly.online
ls -la
الخطوة 2: نشر الموقع الرئيسي (GitHub Pages)
bash

git checkout main
git push origin main
انتقل إلى Settings → Pages
اختر Source: main branch
اختر Folder: / (root)
اضغط Save
انتظر دقيقتين — الموقع سيكون متاحاً على https://tribly.online
الخطوة 3: نشر التطبيق (InfinityFree)
سجّل دخول إلى لوحة تحكم InfinityFree
افتح File Manager أو استخدم عميل FTP
ارفع ملفات التطبيق إلى مجلد htdocs
تأكد من صلاحيات الملفات: 644 للملفات، 755 للمجلدات
الخطوة 4: إعداد Cloudflare DNS
Type
Name
Content
Proxy
A	@	185.27.134.159	Proxied ☁️
CNAME	app	triblyapp.infinityfreeapp.com	Proxied ☁️
CNAME	www	tribly.online	Proxied ☁️

الخطوة 5: إعدادات SSL
في Cloudflare → SSL/TLS → اختر Full (Strict)
تأكد من تفعيل Always Use HTTPS
فعّل Automatic HTTPS Rewrites
الخطوة 6: التحقق النهائي
bash

curl -I https://tribly.online
curl -I https://triblyapp.infinityfreeapp.com
curl https://tribly.online/sitemap.xml
curl https://tribly.online/.well-known/security.txt
🔒 رؤوس الأمان | Security Headers
Header
Value
Purpose
Strict-Transport-Security	max-age=31536000; includeSubDomains; preload	فرض HTTPS
X-Content-Type-Options	nosniff	منع sniffing لأنواع المحتوى
X-Frame-Options	DENY	منع التضمين في إطارات
X-XSS-Protection	1; mode=block	حماية من XSS
Referrer-Policy	strict-origin-when-cross-origin	التحكم في معلومات المرجع
Permissions-Policy	camera=(), microphone=(), geolocation=()	التحكم في صلاحيات المتصفح
Content-Security-Policy	default-src 'self'; script-src 'self'; style-src 'self' 'unsafe-inline'; img-src 'self' data:	سياسة أمان المحتوى

جميع رؤوس الأمان يتم تطبيقها عبر Cloudflare Page Rules و Transform Rules

📬 التواصل | Contact
القناة
التفاصيل
الرابط
📧 البريد الإلكتروني	triblyteam@gmail.com	إرسال رسالة
🌐 الموقع الرسمي	tribly.online	زيارة
📱 التطبيق	triblyapp.infinityfreeapp.com	زيارة
🔒 تقرير أمان	security.txt	عرض

📈 الإحصائيات | Stats
yaml

users: 638+
cities: 4
location: Alexandria, Egypt
status: Coming Soon
version: 2.0.0
lighthouse_performance: 100
lighthouse_accessibility: 100
lighthouse_best_practices: 100
lighthouse_seo: 100
lighthouse_pwa: 100
📄 رخصة MIT | MIT License
text

MIT License

Copyright (c) 2024 Tribly

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

Tribly 🌿

منصة التواصل الاجتماعي التي تجمعك بأصحابك بطريقة مختلفة


© 2024 Tribly. All rights reserved. | Alexandria, Egypt 🇪🇬


```
