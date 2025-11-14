# Sourny- V2 (Gradient design) — Starter (2026-ready)

نسخة مبدئية من مشروع Sourny- V2 بتصميم **Gradient ملون** (Purple → Blue → Cyan).
النسخة مناسبة للنشر السريع: واجهة حديثة + API بسيط مع JWT لاختبار التسجيل وتسجيل الدخول.

## المحتويات
- `frontend/` — واجهة ثابتة مع صفحات: Landing, Login, Dashboard.
- `backend/` — خادوم Node.js + Express مع JWT (in-memory for demo).
- `README.md` — هذا الملف.
- `LICENSE` — MIT.

## تشغيل محلي (Frontend)
1. افتح `frontend/index.html` أو استعمل سيرفر ثابت بسيط:
   ```bash
   npx serve frontend
   ```
   أو افتح الملف مباشرة في المتصفح.

## تشغيل الخادوم (Backend)
```bash
cd backend
npm install
npm start
```
الخادوم يعمل محليًا على `http://localhost:4000`

## ملاحظات فنية
- JWT مستخدم فقط للعرض: مفاتيح سرية في `.env` عند الإنتاج.
- قاعدة بيانات غير متضمنة — يتم حفظ البيانات في الذاكرة (للتجربة). للانتاج ربط بMongo/Postgres.
- خطوات النشر:
  - ارفع `frontend/` إلى GitHub Pages أو Vercel.
  - ارفع `backend/` إلى Render / Railway / Heroku.

## ميزات V2 (الموجودة الآن)
- تصميم Gradient عصري (2026)
- صفحات: Landing, Login, Register, Dashboard
- API: /api/register, /api/login, /api/orders (CRUD بسيطة)
- حماية JWT على endpoints المحمية

---

إن احتجت أعدتلك نسخة مع MongoDB + persistent users أو دمجت OAuth (Google/Meta) نعّمها لك.
