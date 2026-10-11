# 🤖 Buddy — tumhara 3D AI dost (Android)

3D character jo phone me rehta hai, **Gemini** se Hinglish me baat karta hai, game khelta hai,
aur phone ka kaam karta hai.

## Kya kar sakta hai
- 🗣️ Baat karo (type ya 🎤 voice) — Buddy bolke jawab deta hai, mooh hilta hai
- 🎮 Tic-Tac-Toe aur Patthar-Kagaz-Kainchi
- 📂 Files dekhna (`Download`, `DCIM` ...)
- 🛡️ **Delete se pehle HAMESHA permission popup** — "Haan / Nahi"
- 📱 Apps kholna ("WhatsApp kholo"), battery batana
- 👆 Character par tap karo — kudta hai aur haath hilata hai

## APK banane ka tarika (Android Studio ki zaroorat nahi)
1. GitHub par naya repo banao, ye poora folder push karo.
2. **Actions** tab → "Build Buddy APK" chalne do (ya "Run workflow").
3. Run khatam hone par neeche **Artifacts → Buddy-APK** download karo, zip kholo.
4. `app-debug.apk` phone me install karo ("Unknown sources" allow karna padega).

## Pehli baar chalane par
1. App khulte hi **Gemini API key** maangegi → https://aistudio.google.com/apikey (free). Key sirf phone me save hoti hai, repo me nahi.
2. File ka kaam bolo (jaise "Download me kya hai?") → **All files access** ki settings khulegi → Buddy ko allow karo.

## Offline 3D (optional)
Default me `three.js` internet se aata hai. Offline chahiye to `three.min.js` (r128) download karke
`app/src/main/assets/` me rakh do.

## Limitations (sach baat)
- Buddy sirf wahi kaam karta hai jo `PhoneTools.kt` me tools bane hain. Naye tools wahi add karo.
- Dusre apps ke andar (WhatsApp me msg bhejna etc.) control ke liye Accessibility Service lagti hai — alag phase.
- Home screen ke upar floating character ke liye "draw over other apps" overlay service lagegi — alag phase.
- `MANAGE_EXTERNAL_STORAGE` Play Store par restricted hai; sideload/personal use ke liye theek hai.
