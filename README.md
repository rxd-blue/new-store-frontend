# متجر إلكتروني مع بوت محادثة

متجر إلكتروني بسيط مع واجهة مستخدم عربية وبوت محادثة للمساعدة في تصفية المنتجات.

## 🚀 خطوات النشر

### 1. نشر الواجهة على GitHub Pages

1. قم بإنشاء مستودع جديد على GitHub
2. ارفع الملفات التالية:
   - `index.html`
   - `README.md`
3. فعّل GitHub Pages من إعدادات المستودع
   - اذهب إلى Settings > Pages
   - اختر Branch: `master`
   - اختر Folder: `/root`
   - انتظر حتى يظهر رابط موقعك

### 2. نشر السيرفر على Render.com

1. سجل دخول على [Render.com](https://render.com)
2. اختر New Web Service
3. اربط مع مستودع GitHub
4. اضبط الإعدادات:
   - Build Command: `npm install`
   - Start Command: `npm start`
   - Environment: Node
5. انتظر حتى يكتمل النشر
6. احصل على رابط السيرفر
7. عدّل رابط السيرفر في `index.html`

### 3. إعداد Dialogflow

1. اذهب إلى [Dialogflow Console](https://dialogflow.cloud.google.com/)
2. أنشئ مشروع جديد
3. أضف الـ Intents التالية:
   - تصفية حسب النوع
   - تصفية حسب الماركة
4. اضبط Webhook للتواصل مع السيرفر

## 📦 هيكل المشروع

```
├── index.html      # الواجهة الأمامية
├── server.js       # السيرفر
├── package.json    # تبعيات Node.js
└── README.md       # التوثيق
```

## 🔧 التقنيات المستخدمة

- HTML5 + CSS3 + JavaScript
- Bootstrap 5
- Node.js + Express
- Dialogflow
- GitHub Pages
- Render.com

## 📝 ملاحظات

- تأكد من تحديث رابط السيرفر في `index.html` بعد النشر على Render
- يمكن إضافة المزيد من المنتجات في مصفوفة `products`
- البوت يدعم اللغة العربية للتواصل مع العملاء 