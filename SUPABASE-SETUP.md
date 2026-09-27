# ربط حسابات الطلاب بـ Supabase

1. أنشئ حسابًا في [Supabase](https://supabase.com/dashboard/sign-up)، ثم أنشئ مشروعًا جديدًا.
2. من إعدادات المشروع، انسخ **Project URL** و**Publishable key** إلى `supabase-config.js`.
3. من **Authentication → URL Configuration**، اضبط **Site URL** على `https://modern-commerce-unit-yh4fbp3jzlf.qoder.website/`، وأضف الرابطين التاليين إلى **Redirect URLs**:
   - `https://modern-commerce-unit-yh4fbp3jzlf.qoder.website/login.html`
   - `https://modern-commerce-unit-yh4fbp3jzlf.qoder.website/reset-password.html`
4. التسجيل بالبريد مفعّل افتراضيًا. سيحتاج الطالب إلى تأكيد بريده الإلكتروني إذا بقي تأكيد البريد مفعّلًا.

المفتاح المسموح به في الواجهة هو **Publishable key** فقط. لا تضع `service_role` أو أي secret key في ملفات الموقع. الخطة المجانية تشمل حتى 50,000 مستخدم نشط شهريًا، لكن المشاريع المجانية قد تتوقف مؤقتًا بعد أسبوع من عدم النشاط. خدمة البريد الافتراضية محدودة للاختبار؛ للاستخدام المنتظم قد تحتاج إلى إعداد SMTP خاص.
