# دليل الزوار - ساك الدولية
## SAAK International Visitor Guide

---

## 📁 هيكل الملفات

```
visitor-guide/
├── index.html              ← الملف الرئيسي (55 KB فقط)
├── images/
│   ├── logo-white.png      ← الشعار الأبيض (للهيدر)
│   ├── logo-color.png      ← الشعار الملون (للمحتوى)
│   ├── facility.jpg        ← صورة المبنى الخارجي
│   ├── manufacturing1.jpg  ← صورة منطقة التصنيع
│   └── manufacturing2.jpg  ← صورة قريبة من الإنتاج
├── icons/
│   ├── icon-camera.png     ← ممنوع التصوير
│   ├── icon-smoking.png    ← ممنوع التدخين
│   ├── icon-hazard.png     ← مواد خطرة
│   ├── icon-drinks.png     ← ممنوع المشروبات
│   ├── icon-weapons.png    ← ممنوع الأسلحة
│   └── icon-food.png       ← ممنوع الطعام
├── AppScript.js            ← كود Google Apps Script
└── README.md               ← هذا الملف

```

---

## 🔧 خطوات ربط نموذج الآراء بـ Google Sheets

### الخطوة 1: إعداد Apps Script

1. افتحي [Google Sheet](https://docs.google.com/spreadsheets/d/1BaLek2MK6Mw9YJz5rMW5azYWpxY4D4nCIhZ-Bf6xybw)
2. من القائمة: **Extensions → Apps Script**
3. احذفي كل الكود الموجود
4. افتحي ملف `AppScript.js` وانسخي محتواه كاملاً
5. الصقيه في محرر Apps Script
6. اضغطي **Save** (Ctrl+S)

### الخطوة 2: النشر (Deploy)

1. اضغطي **Deploy → New deployment**
2. اختاري **Type: Web app**
3. **Execute as:** Me
4. **Who has access:** Anyone
5. اضغطي **Deploy**
6. وافقي على الصلاحيات
7. **انسخي رابط الـ Web App**

### الخطوة 3: ربط الرابط بـ index.html

1. افتحي `index.html`
2. ابحثي عن: `SCRIPT_PLACEHOLDER`
3. استبدليه برابط الـ Web App

**مثال:**
```
قبل: var SCRIPT_URL = 'https://script.google.com/macros/s/SCRIPT_PLACEHOLDER/exec';
بعد: var SCRIPT_URL = 'https://script.google.com/macros/s/AKfycbx.../exec';
```

---

## 🚀 رفع على GitHub

1. أنشئي Repository جديد: `visitor-guide`
2. ارفعي **كل الملفات والمجلدات** معاً
3. فعّلي GitHub Pages من Settings → Pages → main branch
4. الرابط: `https://saak-sa.github.io/visitor-guide/`

## 🌐 رفع على Netlify

1. اسحبي **مجلد `visitor-guide`** كاملاً على [netlify.com/drop](https://app.netlify.com/drop)
2. الرابط يظهر فوراً

---

## ✏️ تعديل الصور

استبدلي أي صورة بنفس الاسم في نفس المجلد:
- `images/facility.jpg` ← صورة المبنى
- `images/manufacturing1.jpg` ← صورة التصنيع الأولى
- `images/manufacturing2.jpg` ← صورة التصنيع الثانية
