# SoruÇöz 📷✨

Fotoğrafını çek, yapay zeka çözsün, sana Türkçe anlatsın. İki yol var: API anahtarsız **Web'de Sor** veya anahtarlı otomatik çözüm.

## Özellikler
- 📷 Kamera / 🖼️ Galeri ile soru fotoğrafı (fotoğraf sonrası sınıf + ders ekranı açılır)
- 📚 Sınıf (1-12, Üniversite, KPSS/DGS) + ders + seviye seçimi
- 🌐 Web'de Sor: soru metni hazırlanır, kopyalanır/paylaşılır, Gemini/ChatGPT/Copilot sitesinde cevap alınır, cevap yapıştırılıp kaydedilir (API anahtarı gerekmez, manuel adımdır)
- 🤖 API ile otomatik çözüm (isteğe bağlı): Google Gemini, Pollinations, OpenRouter
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
