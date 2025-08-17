
تعليمات سريعة للنشر على GitHub Pages + Search Console

1) بدّل كل ظهور لـ BASE_URL بالمشروع بعنوان موقعك الحقيقي، مثال:
   https://example.github.io/demo-site  ->  https://YOUR-USER.github.io/REPO-NAME
   ملاحظة: في مواقع المستخدم (user site) بيكون الرابط: https://YOUR-USER.github.io/
   أما مواقع المشاريع (project site) بيكون: https://YOUR-USER.github.io/REPO-NAME

2) تحقق من الروابط داخل:
   - index.html وملفات الصفحات
   - robots.txt (سطر Sitemap)
   - sitemap.xml (كل <loc>)

3) تحقّق من أن الصفحات تُفتح صح بعد الرفع.

4) تفعيل GitHub Pages:
   - Settings > Pages > Source: deploy from a branch
   - اختار الفرع main والمجلد / (root)
   - احفظ، وبعدين افتح الرابط اللي بيعطيك GitHub

5) Google Search Console:
   - أضف خاصية جديدة (URL prefix) بعنوان موقعك بالضبط.
   - للتحقق يا إمّا:
     أ) ترفع ملف HTML اللي بيعطيك إيّاه جوجل على جذر الموقع (نفس مستوى index.html)، أو
     ب) تفعل الوسم <meta name="google-site-verification"...> داخل <head> بملف index.html
   - قدّم خريطة الموقع من المسار: /sitemap.xml
   - استخدم URL Inspection > Test live > Request indexing.

6) شائعة المشاكل:
   - خريطة الموقع تعطي خطأ: تأكّد الرابط صحيح، والملف مُتاح علناً وما في أخطاء صياغة.
   - robots.txt يمنع الزحف؟ عندنا Allow: /؛ لا تغيّرها لمنع الفهرسة.
   - العناوين الكانونيكل canonical لازم تطابق الروابط العلنية لموقعك.

بالتوفيق! :)
