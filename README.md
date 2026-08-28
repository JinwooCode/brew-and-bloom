# Brew & Bloom

עמוד תדמית (landing page) יחיד עבור "Brew & Bloom" — קלייה בוטיקית דמיונית של קפה סינגל-אוריג'ין.

## מטרת הפרויקט

להציג נוכחות דיגיטלית קטנה ומקצועית למותג קפה: הצגת המותג, שלושת התערובות המרכזיות, תהליך הקלייה, וקריאה לפעולה להזמנת פולים / מנוי.
הפרויקט נבנה כתרגיל מהיר end-to-end: עיצוב באמצעות Stitch MCP → אתר סטטי → Git → GitHub → תיעוד ב-Obsidian.

## טכנולוגיות

- **HTML5** — עמוד סטטי בודד (`index.html`)
- **CSS3** — עיצוב מוטמע, Flexbox/Grid, responsive
- **Google Fonts** — טיפוגרפיה (serif לכותרות, sans-serif לגוף)
- **Stitch MCP** — יצירת העיצוב והקוד
- **Git / GitHub** — ניהול גרסאות

ללא backend, ללא database, ללא build step.

## איך להריץ

פשוט לפתוח את הקובץ בדפדפן:

```bash
open index.html        # macOS
start index.html       # Windows
```

או להרים שרת סטטי מקומי:

```bash
python -m http.server 8000
# ואז לגלוש אל http://localhost:8000
```
