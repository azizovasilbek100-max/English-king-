# 👑 English King — O'rnatish Qo'llanmasi

## 📱 Android APK qilish — 2 ta usul

---

## USUL 1: PWA (Eng oson — hech qanday dastur kerak emas)

1. Barcha 3 faylni bir joyga saqlang:
   - index.html
   - manifest.json
   - sw.js

2. **GitHub Pages orqali (BEPUL hosting):**
   - github.com ga kiring → New Repository yarating
   - 3 faylni upload qiling
   - Settings → Pages → Branch: main → Save
   - Havola: `https://username.github.io/english-king`

3. Android telefoningizda:
   - Chrome brauzerida havolani oching
   - O'ng yuqori burchak: ⋮ → "Add to Home screen"
   - "Install" tugmasini bosing
   - **Ilova ikonkasi ekranga qo'shiladi!**
   - Offline ham ishlaydi! ✅

---

## USUL 2: Haqiqiy APK (Android Studio kerak)

### Talab qilinadigan dasturlar:
- Node.js (nodejs.org)
- Android Studio (developer.android.com)
- Capacitor (`npm install @capacitor/core @capacitor/cli`)

### Buyruqlar:
```bash
# 1. Papka yarating
mkdir english-king-app && cd english-king-app

# 2. index.html, manifest.json, sw.js fayllarini papkaga ko'chiring

# 3. package.json yarating
npm init -y

# 4. Capacitor o'rnating
npm install @capacitor/core @capacitor/cli @capacitor/android

# 5. Capacitor sozlang
npx cap init "English King" com.englishking.app --web-dir .

# 6. Android platformasini qo'shing
npx cap add android

# 7. Sync qiling
npx cap sync android

# 8. Android Studio'da oching
npx cap open android

# 9. Android Studio'da: Build → Generate Signed APK
```

---

## USUL 3: Online APK Builder (Eng tez)

1. **PWABuilder.com** ga kiring (Microsoft's tool)
2. GitHub Pages havolangizni kiriting
3. "Build APK" tugmasini bosing
4. APK yuklab oling va o'rnating!

---

## 📊 Ilova tarkibi

- **800+ so'z** — 16 kategoriya
- **Kartochkalar** — yashil/qizil ranglar
- **Lug'at** — qidirish va filtr
- **Test** — 10/20/30 savol
- **So'z Yasash** — harflar o'yini
- **Ball tizimi** — localStorage'da saqlanadi
- **Offline** — internetsiZ ishlaydi

---

Muammo bo'lsa: English King ilovasi haqida so'rang!
