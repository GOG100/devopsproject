# Smart Parking System 🚗🅿️

מערכת מיקרו-סרביסים לניהול חניון חכם המורכבת משרת Web ושרת Storage.

## 🏗️ ארכיטקטורת המערכת
- **Web Service (Nginx):** מגיש את לוח הבקרה בפורט `8080`.
- **Storage Service (Apache):** מגיש את קבצי המדיה והתמונות בפורט `8081`.
- **Data Volume:** מיפוי מקומי של תיקיית `storage/images/` לתוך שרת ה-Storage.

## 🚀 איך להריץ את המערכת?

1. ודאו ש-Docker Desktop פועל במחשב.
2. הריצו את הפקודה הבאה מתיקיית השרש:
   ```bash
   docker compose up -d
