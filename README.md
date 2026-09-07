# תן לי שולחן — ניהול תחרויות טניס שולחן

אפליקציית ווב של מועדון טניס שולחן מבואות החרמון לניהול תחרויות לפי תקנון ITTF.
קובץ אחד (`index.html`), ללא בנייה. משתמשת באותו פרויקט Firebase של אפליקציית הנוכחות (`ttcmh-2a752`):
כניסה עם אותם משתמשים, ייבוא שחקנים מאוסף `players`, ושמירת התחרויות באוסף `tournaments` (מסונכרן בזמן אמת בין מכשירים).

## פריסה
1. ריפו ציבורי `ttc-mvh-tournaments`, הקבצים בשורש, ענף `main`.
2. Settings → Pages → Source: Deploy from a branch → `main` / root.
3. הכתובת: https://shahar1987.github.io/ttc-mvh-tournaments/
4. ב-Firestore → Rules להוסיף את הכלל מ-`firestore.rules.txt` וללחוץ Publish.

## מבנה הנתונים (אוסף tournaments)
`name, date, phase, playersCount, rev, client, state (JSON של כל מצב התחרות), updatedAt, updatedBy, createdBy`
