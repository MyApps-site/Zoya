# Lia AI: pehla version (Parts 1 se 8)

Isme kya hai:
- Hindi / Hinglish / English me **live voice baatcheet** (Gemini Live)
- **Typed chat**
- 10 personalities, naam badalna, bhasha chunna
- **Phone ke kaam:** app kholna, call, message
- `direct` version me **screen padhna, tap, type, scroll** (Accessibility se)
- Do versions: `direct` (poori power) aur `play` (Google Play safe)

Abhi nahi hai (agle round me): 3D orb/splash, Website Forge, Instagram/WhatsApp agent, licensing, saari fancy screens.

## Zaroori baat
Ye code bina compile kiye likha gaya hai (mere paas Android tools nahi the). Pehli build me kuch errors aa sakti hain. Error ka text copy karke mujhe bhej dena, main theek kar dunga.

## Gemini key
1. aistudio.google.com par Google account se login karo.
2. "Get API key" se free key banao.
3. App ke Settings me paste karke Save karo. Key sirf phone me rehti hai.

Voice ka model naam `app/src/main/java/com/Lia/assistant/voice/GeminiLiveClient.kt` me `MODEL` constant me hai. Agar voice connect na ho to Google ke Live API docs se current naam dekhkar wahi ek line badalni hai.

## APK banane ka tareeka (GitHub se, free)

### Tareeka A: PC ya laptop se (sabse aasaan, ek baar ka kaam)
1. github.com par account banao.
2. New repository banao, naam `lia-ai`, **Private** rakho.
3. Is zip ko unzip karo. Andar ke **saare folders aur files** (`app`, `.github`, `settings.gradle.kts` ...) repository ke "uploading an existing file" page par drag karke daalo. `.github` folder zaroor jaye.
4. "Commit changes" dabao.
5. Upar **Actions** tab kholo. "Build APK" chalega (5-10 minute).
6. Hari tick aane par us run ko kholo, neeche **Artifacts** me `lia-ai-apk` download karo.
7. Zip ke andar `direct` aur `play` ki APK milengi. Apne liye `direct` wali use karo.

### Tareeka B: sirf phone se
Phone ke browser me folder upload mushkil hai. Ye karo:
1. Termux install karo (F-Droid se).
2. Termux me: `pkg install git`
3. Zip ko Termux me unzip karo, phir `git init`, `git add .`, `git commit`, aur apne GitHub repo par push karo. (Push ke liye GitHub me Settings > Developer settings > Personal access token banana padega.)
Agar ye bhari lage to kisi dost ka PC ek baar use kar lo (Tareeka A).

## Phone par install
1. APK file phone me kholo. "Install unknown apps" ki ijazat maangega, de do.
2. App kholo. Settings me key daalo.
3. Voice tab me Start dabao. Mic ki ijazat do.
4. Contacts/call ke liye Settings > "Ijazat do".
5. Screen control ke liye (sirf `direct`): Settings > "Accessibility settings kholo" > Lia AI > chalu karo. Ye bahut shakti wali ijazat hai, sirf apne phone par do.

## Suraksha
- Key ya koi secret code me nahi hai.
- Screen control wale kaam me Lia ko hukm hai ki bhejne/post karne se pehle tumse pooche.
- Password aur OTP type nahi karegi.
