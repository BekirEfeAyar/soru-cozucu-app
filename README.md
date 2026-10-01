# SoruÇöz 📷✨

Fotoğrafını çek, yapay zeka çözsün, sana Türkçe anlatsın. %100 ücretsiz (kendi ücretsiz API anahtarınla).

## Özellikler
- 📷 Kamera / 🖼️ Galeri ile soru fotoğrafı
- 📚 Ders + seviye seçimi (ortaokul/lise/üniversite)
- 🤖 3 ücretsiz servis: Google Gemini (önerilen), Pollinations, OpenRouter
- 🇹🇷 Adım adım Türkçe anlatım + CEVAP + Kısa Özet
- 🔊 Sesli anlat (cihaz TTS, ücretsiz), 📋 kopyala, 📤 paylaş
- 📚 Geçmiş telefonda saklanır

## Ücretsiz API anahtarı (1 dk, bir kez)
1. **Gemini (önerilen):** https://aistudio.google.com/apikey → giriş yap → Create API key → uygulamaya yapıştır
2. **Pollinations:** https://enter.pollinations.ai/keys → hesap → key oluştur
3. **OpenRouter:** https://openrouter.ai/keys → hesap → key al, model: `google/gemini-2.0-flash-exp:free`

Uygulamada ⚙️ → servis seç → anahtarı yapıştır → Kaydet → Bağlantıyı Test Et.

## Web olarak çalıştır
`index.html` dosyasını tarayıcıda aç (internet gerekli).

## Android APK derleme (ücretsiz)
Gerekenler: Node.js, JDK 17, Android SDK.

```bash
npm install
npx cap add android
npx cap sync android
cd android
gradlew.bat assembleDebug
```

APK: `android/app/build/outputs/apk/debug/app-debug.apk`

## Proje yapısı
```
soru-cozucu-app/
├── index.html
├── www/
├── capacitor.config.json
├── package.json
└── android/
```
