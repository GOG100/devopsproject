---

### 📄 `AI_USAGE.md`
```markdown
# תיעוד שימוש ב-AI 🤖

במהלך הפיתוח נעזרנו בכלי AI לקבלת הנחיות, פתרון שגיאות ובניית אוטומציות.

## 💬 פרומפטים מרכזיים שנעשה בהם שימוש
- *"איך להגדיר Docker Compose עם שני שרשים (Nginx ו-Apache) ומיפוי Volume?"*
- *"בניית קובץ GitHub Actions Workflow לבדיקת Build והעלאת Images ל-GHCR."*

## 🛠️ שגיאה מרכזית שטופלה בעזרת ה-AI
- **הבעיה:** דחיפת קובץ ה-Workflow ל-GitHub נכשלה עם שגיאת הרשאות Token:
  `refusing to allow a Personal Access Token to create or update workflow... without workflow scope`
- **הפתרון:** ה-AI זיהה שחסרה הרשאת `workflow` ב-Personal Access Token (PAT). יצרנו Token חדש ב-GitHub עם הרשאות `repo` ו-`workflow`, וה-Push עבר בהצלחה.
