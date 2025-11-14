# Sourny - Full SaaS Scaffold (SaaS-like design)

نسخة جاهزة للنشر من مشروع Sourny — تصميم شبيه بمواقع SaaS العالمية.
تحتوي على واجهة Frontend، Backend (Express + JWT + MongoDB)، ونموذج مستخدم مع تشفير كلمات المرور.

## ملاحظات سريعة
- هذه نسخة scaffold جاهزة للتطوير والإطلاق.
- استخدم MongoDB Atlas للبيانات الحقيقية.
- لا تحفظ متغيرات حساسة في المستودع؛ استخدم Environment variables.

## تشغيل محلي
1. فك الضغط عن الحزمة.
2. شغّل Backend:
   ```bash
   cd backend
   npm install
   cp .env.example .env
   # ثم عدل .env بالقيم الحقيقية
   npm start
   ```
3. شغّل الواجهة:
   - افتح `frontend/index.html` في المتصفح
   - أو شغّل سيرفر بسيط: `npx serve frontend`

## نشر سريع (مقترح)
- Frontend: GitHub Pages أو Vercel
- Backend: Render / Railway / Heroku
- Database: MongoDB Atlas (اتبع خطوات إضافة MONGO_URI في متغيرات البيئة)

==== ملفات مهمة ===
- backend/server.js
- backend/routes/auth.js
- backend/models/User.js
- frontend/js/config.js  (ضع رابط API هنا)
