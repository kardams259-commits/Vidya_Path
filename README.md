# VidyaPath — UP Board Smart Study

> **VidyaPath — UP बोर्ड स्मार्ट स्टडी ऐप**
> कक्षा 10, 11 और 12 के विद्यार्थियों के लिए फ्लैशकार्ड, MCQ क्विज़, AI अध्ययन सहायक और वैज्ञानिक कैलकुलेटर — सब एक ही ऐप में। पूरी तरह ऑफ़लाइन चलता है, इंस्टॉल करने योग्य (PWA) है, और आपकी अपनी API key से AI इस्तेमाल करता है।

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PWA](https://img.shields.io/badge/PWA-installable-1A237E)](#-install-as-an-app-pwa)
[![Offline](https://img.shields.io/badge/offline-ready-FF8F00)](#-offline-support)
[![No build step](https://img.shields.io/badge/build-none%20needed-3949AB)](#-run-locally)

A single-file, offline-first study app for **UP Board** students (Hindi medium).
No framework, no bundler, no server — just `index.html`, a manifest, an icon and a service worker.

---

## 📥 Install as an app (PWA)

1. ऐप को GitHub Pages URL पर खोलें (Chrome / Edge / Safari)।
2. **Android Chrome:** ⋮ मेनू → *Add to Home screen* / *Install app*।
3. **iPhone Safari:** Share → *Add to Home Screen*।

इंस्टॉल के बाद यह सामान्य ऐप की तरह फुल-स्क्रीन खुलता है और बिना इंटरनेट भी काम करता है।

---

<!--
## 📸 Screenshots

| Flashcards | Quiz | AI Assistant | Calculator |
|---|---|---|---|
| ![Flashcards](screenshots/1.jpg) | ![Quiz](screenshots/2.jpg) | ![AI](screenshots/3.jpg) | ![Calculator](screenshots/4.jpg) |

> Screenshots add karne ke liye `screenshots/` folder banao aur upar ke naam se images rakho, phir ye comment block hata do.
-->

## ✨ Features / विशेषताएँ

| Feature | क्या करता है | What it does |
|---|---|---|
| 🃏 **Flashcards / फ्लैशकार्ड** | हर अध्याय के प्रश्न-उत्तर कार्ड, उलटकर उत्तर देखें | Chapter-wise Q&A cards, tap to flip |
| 📝 **Quiz / क्विज़** | MCQ अभ्यास, स्कोर और प्रगति ट्रैकिंग | MCQ practice with scoring and progress |
| 🤖 **AI Assistant / AI सहायक** | किसी भी अध्याय पर AI से नए प्रश्न, नोट्स, फॉर्मूले, PYQ बनवाएँ | Generate new questions, notes, formulas and PYQs for any chapter |
| 🧮 **Calculator / कैलकुलेटर** | वैज्ञानिक कैलकुलेटर (sin, cos, log, √, घात) | Scientific calculator |
| 📚 **Study material** | नोट्स, फॉर्मूला सूची, पिछले वर्ष के प्रश्न | Notes, formula list, previous-year questions |
| 🌙 **UI** | डार्क मोड, लिक्विड-ग्लास कार्ड, मोबाइल/डेस्कटॉप व्यू | Dark mode, liquid-glass cards, mobile/desktop view |
| 📴 **Offline** | पहली बार खुलने के बाद इंटरनेट की ज़रूरत नहीं | Works with no internet after first load |

### Subjects & classes / विषय एवं कक्षाएँ

| Subject | Class 10 | Class 11 | Class 12 |
|---|:---:|:---:|:---:|
| भौतिक विज्ञान — Physics | — | ✅ | ✅ |
| रसायन विज्ञान — Chemistry | — | ✅ | ✅ |
| जीव विज्ञान — Biology | — | ✅ | ✅ |
| गणित — Mathematics | ✅ | ✅ | ✅ |
| विज्ञान — Science | ✅ | — | — |
| सामाजिक विज्ञान — Social Science | ✅ | — | — |

---

## 🔑 AI के लिए मुफ़्त Gemini API Key बनाएँ

AI सहायक चलाने के लिए एक API key चाहिए। **Google Gemini की key मुफ़्त मिलती है** और इसमें क्रेडिट कार्ड नहीं लगता।

**👉 मुफ़्त key यहाँ से लें: <https://aistudio.google.com/app/apikey>**

स्टेप-बाय-स्टेप:

1. ऊपर वाला लिंक खोलें (Google अकाउंट से लॉगिन करें)।
2. **Create API key** पर टैप करें → कोई भी project चुनें (नया बनाना हो तो अपने-आप बन जाएगा)।
3. बनने वाली key **`AIza...`** से शुरू होगी — **Copy** कर लें।
4. ऐप खोलें → साइडबार → **AI सहायक** → **🔑 API Key** वाला खाना।
5. Provider में **Google Gemini** चुनें, key पेस्ट करें और **सहेजें (Save)** दबाएँ। बस, AI तैयार है।

> **आपकी key कहाँ जाती है?** सिर्फ़ आपके फ़ोन में (browser `localStorage`) सुरक्षित रहती है और सीधे Google को भेजी जाती है। कोई बीच का सर्वर नहीं, कोई ट्रैकिंग नहीं। इस रेपो में कोई key मौजूद नहीं है।

### Other AI providers (optional)

Gemini के अलावा कोई भी OpenAI-संगत API चलेगा — AI सेटिंग्स में provider चुनकर अपनी key डालें:

| Provider | Key लेने का लिंक | नोट |
|---|---|---|
| Google Gemini | <https://aistudio.google.com/app/apikey> | **मुफ़्त** (recommended) |
| Groq | <https://console.groq.com/keys> | मुफ़्त tier, बहुत तेज़ |
| OpenAI | <https://platform.openai.com/api-keys> | पेड |
| OpenRouter | <https://openrouter.ai/keys> | कई मॉडल, कुछ मुफ़्त |
| DeepSeek | <https://platform.deepseek.com> | पेड, सस्ता |
| Custom | कोई भी endpoint | Base URL + key दोनों भरें |

> API key के बिना भी ऐप पूरा चलता है — फ्लैशकार्ड, क्विज़ और कैलकुलेटर ऑफ़लाइन उपलब्ध रहते हैं। सिर्फ़ AI फ़ीचर key मांगते हैं।

---

## ▶️ Run locally

कोई build step नहीं है। बस फ़ाइलें सर्व करनी हैं (service worker के लिए `file://` नहीं, HTTP चाहिए):

```bash
# इसी फ़ोल्डर में
python3 -m http.server 8080
# फिर browser में खोलें: http://localhost:8080
```

## 🌐 Deploy to GitHub Pages

रेपो में फ़ाइलें डालने के बाद: **Settings → Pages → Source = Deploy from a branch** → Branch = **main**, Folder = **/ (root)** → Save।
एक मिनट में ऐप यहाँ live हो जाएगा: `https://<your-username>.github.io/vidyapath/`

Command line से push करना हो तो:

```bash
git remote add origin https://github.com/<your-username>/vidyapath.git
git branch -M main
git push -u origin main
```

## 📱 Android APK बनाएँ

PWA तैयार है, इसलिए सीधे **[PWABuilder](https://www.pwabuilder.com)** से APK बन जाता है:

1. Pages URL पेस्ट करें → आपका ऐप स्कैन होगा।
2. **Package for stores → Android** चुनें।
3. Package ID, app name, icon भरें → **Download**।
4. मिली `.apk` फ़ाइल फ़ोन में इंस्टॉल करें (Unknown sources allow करना पड़ेगा)।

---

## 🗂 Project structure

```
index.html          # पूरा ऐप — UI, डेटा (फ्लैशकार्ड/क्विज़), AI, कैलकुलेटर
manifest.json       # PWA manifest (installability)
sw.js               # Service worker — offline cache
icon.svg            # App icon
splash.html         # Splash screen (APK/PWA tools के लिए)
```

## 🔒 Privacy

- कोई बैकएंड, कोई अकाउंट, कोई analytics नहीं।
- प्रगति और API key फ़ोन के local storage में रहते हैं — ऐप डेटा बाहर नहीं भेजता।
- AI अनुरोध सीधे आपके चुने हुए provider को जाते हैं।

## 🤝 Contributing

मिले-जुले सुधार (typos, नए अध्याय, नए क्विज़) welcome हैं — issue खोलें या PR भेजें।
`index.html` के `SUBJECTS` array में सीधे नए फ्लैशकार्ड जोड़े जा सकते हैं।

## 📄 License

[MIT](LICENSE)

## ⚠️ Disclaimer

यह एक स्वतंत्र स्टडी टूल है। **UP Board / UPMSP से किसी भी तरह संबद्ध नहीं है।** कंटेंट परीक्षा की तैयारी में मदद के लिए है — आधिकारिक पाठ्यक्रम के लिए board की वेबसाइट देखें।
