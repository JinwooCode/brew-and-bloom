# Brew & Bloom

עמוד תדמית (landing page) יחיד עבור "Brew & Bloom" — קלייה בוטיקית דמיונית של קפה סינגל-אוריג'ין.
האתר בעברית, בפריסת RTL מלאה.

## מטרת הפרויקט

להציג נוכחות דיגיטלית קטנה ומקצועית למותג קפה: הצגת המותג, שלוש הקליות המרכזיות, תהליך הקלייה, וקריאה לפעולה להזמנת פולים / מנוי.
הפרויקט נבנה כתרגיל מהיר end-to-end: עיצוב → אתר סטטי → Git → GitHub → תיעוד ב-Obsidian.

## טכנולוגיות

- **HTML5** — עמוד סטטי בודד (`index.html`), `lang="he"` + `dir="rtl"`
- **CSS3** — עיצוב מוטמע, Flexbox/Grid, custom properties, היסטים לוגיים (`inset-inline-start`), responsive
- **Google Fonts** — Frank Ruhl Libre (כותרות) + Heebo (גוף)
- **Stitch MCP** — הפיק את ה-design system של הפרויקט (פלטת צבעים, סקאלת טיפוגרפיה ו-spacing, כללי elevation ו-components). ה-HTML עצמו נכתב ידנית לפי אותו design system, מכיוון שיצירת ה-screen ב-Stitch לא הושלמה — ראו הערה למטה.
- **Git / GitHub** — ניהול גרסאות

ללא backend, ללא database, ללא build step.

### הערה על Stitch

`generate_screen_from_text` הסתיים ב-timeout בכל ארבעת הניסיונות, ו-`list_screens` נשאר ריק. מה ש-Stitch כן הפיק ונשמר — ה-design system וה-assets — שימש כבסיס לעיצוב: Frank Ruhl Libre הוא התחליף העברי ל-Playfair Display שנבחר שם, וכן אומצו הצל האמביינטי (`0 4px 20px rgba(44,29,20,.04)`), רדיוס 8px לכפתורים ו-min-height 48px.

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
