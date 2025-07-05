# 🚀 دليل النشر المفصل

## الخطوة 1: تحضير الحساب

### إنشاء حساب Vercel
1. اذهب إلى [vercel.com](https://vercel.com)
2. اضغط "Sign Up"
3. سجل باستخدام GitHub أو Google
4. أكد البريد الإلكتروني

## الخطوة 2: تحميل المشروع

### من v0
1. اضغط "Download Code" في أعلى الصفحة
2. اختر "Download as ZIP"
3. استخرج الملفات في مجلد جديد

### أو من GitHub
\`\`\`bash
git clone [repository-url]
cd wasat-group-website
\`\`\`

## الخطوة 3: النشر

### الطريقة الأولى: من المتصفح
1. اذهب إلى [vercel.com/new](https://vercel.com/new)
2. اسحب مجلد المشروع إلى الصفحة
3. اضغط "Deploy"
4. انتظر انتهاء النشر (2-3 دقائق)

### الطريقة الثانية: من سطر الأوامر
\`\`\`bash
# تثبيت Vercel CLI
npm i -g vercel

# في مجلد المشروع
vercel

# اتبع التعليمات:
# - Set up and deploy? Y
# - Which scope? (اختر حسابك)
# - Link to existing project? N
# - Project name: wasat-group-website
# - Directory: ./
# - Override settings? N

# للنشر للإنتاج
vercel --prod
\`\`\`

## الخطوة 4: ربط الدومين

### الخيار الأول: دومين جديد (الأفضل)
1. اشتر دومين من:
   - [Namecheap](https://namecheap.com)
   - [GoDaddy](https://godaddy.com)
   - [Cloudflare](https://cloudflare.com)

2. في Vercel Dashboard:
   - اذهب إلى Settings > Domains
   - أضف الدومين الجديد
   - اتبع تعليمات DNS

### الخيار الثاني: Subdomain من Odoo
1. في إعدادات DNS لـ Odoo:
\`\`\`
Type: CNAME
Name: website
Value: your-project.vercel.app
\`\`\`

2. في Vercel:
   - أضف `website.wast-group.odoo.com`
   - انتظر التحقق (قد يستغرق 24 ساعة)

## الخطوة 5: التحقق

### اختبار الموقع
- ✅ تحميل الصفحة الرئيسية
- ✅ عمل جميع الروابط
- ✅ عرض الصور
- ✅ عمل النماذج
- ✅ الاستجابة على الهواتف

### اختبار الأداء
- استخدم [PageSpeed Insights](https://pagespeed.web.dev)
- يجب أن يكون النتيجة 90+ للأداء

## 🆘 حل المشاكل الشائعة

### مشكلة: الصور لا تظهر
\`\`\`javascript
// في next.config.mjs
images: {
  unoptimized: true
}
\`\`\`

### مشكلة: الروابط لا تعمل
\`\`\`javascript
// تأكد من trailingSlash
trailingSlash: true
\`\`\`

### مشكلة: خطأ في البناء
\`\`\`bash
# امسح cache وأعد التثبيت
rm -rf .next node_modules
npm install
npm run build
\`\`\`

## 📞 الدعم
- واتساب: +218919835505
- إيميل: info@wasat-group.ly
