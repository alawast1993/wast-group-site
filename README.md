# موقع مجموعة وسط للخدمات التسويقية

## 🚀 نشر الموقع

### المتطلبات
- Node.js 18+ 
- npm أو yarn
- حساب Vercel (مجاني)

### خطوات النشر السريع

#### 1. تحضير المشروع
\`\`\`bash
# تثبيت المتطلبات
npm install

# بناء المشروع
npm run build

# اختبار محلي
npm run dev
\`\`\`

#### 2. النشر على Vercel
\`\`\`bash
# تثبيت Vercel CLI
npm i -g vercel

# تسجيل الدخول
vercel login

# نشر المشروع
vercel

# نشر للإنتاج
vercel --prod
\`\`\`

#### 3. ربط الدومين المخصص
1. اذهب إلى [Vercel Dashboard](https://vercel.com/dashboard)
2. اختر المشروع
3. اذهب إلى Settings > Domains
4. أضف الدومين الجديد
5. اتبع تعليمات DNS

### إعدادات DNS المطلوبة

#### للدومين الجديد (wasat-group.ly)
\`\`\`
Type: A
Name: @
Value: 76.76.19.19

Type: CNAME  
Name: www
Value: cname.vercel-dns.com
\`\`\`

#### للـ Subdomain (website.wast-group.odoo.com)
\`\`\`
Type: CNAME
Name: website
Value: your-project.vercel.app
\`\`\`

## 📱 الميزات
- ✅ تصميم متجاوب
- ✅ دعم اللغة العربية (RTL)
- ✅ تحسين محركات البحث (SEO)
- ✅ سرعة تحميل عالية
- ✅ أمان متقدم

## 🔧 التخصيص
- تعديل الألوان في `globals.css`
- تحديث المحتوى في ملفات الصفحات
- إضافة صور جديدة في مجلد `public`

## 📞 الدعم الفني
للمساعدة في النشر: واتساب +218919835505
\`\`\`

سأنشئ ملف GitHub Actions للنشر التلقائي:
