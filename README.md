# VoiceDraw 🎙️ > 📝 > 🖼️

VoiceDraw, sesli komutlarınızı yazıya döküp, bu metinlerden yapay zeka ile görsel üreten ve görsel çıktıları arayüzde gösteren bir Streamlit uygulamasıdır.

## Özellikler
- **Ses Kaydı:** Mikrofonunuzdan ses kaydedin.
- **Transkripsiyon:** Kaydedilen sesi yazıya dökün (OpenAI Whisper veya alternatif transkriptör ile).
- **Görsel Üretimi:** Yazıya dökülen metni kullanarak DALL-E veya Google Gemini ile görsel oluşturun.
- **Arayüz:** Streamlit tabanlı, kolay ve etkileşimli kullanıcı arayüzü.

## 💻 Kurulum
1. Gerekli kütüphaneleri yükleyin:
   ```zsh
   pip install -r requirements.txt
   ```
2. `.env` dosyasına API anahtarlarınızı ekleyin:
   ```env
   openai_apikey="YOUR_OPENAI_API_KEY"
   google_apikey="YOUR_GOOGLE_API_KEY"
   ```

## 🔓 Kullanım
1. Uygulamayı başlatın:
   ```zsh
   streamlit run app.py
   ```
2. Arayüzde "Başlat" ile ses kaydını başlatın, "Durdur" ile kaydı bitirin.
3. Kaydınız otomatik olarak yazıya dökülür ve görsel üretilir.
4. Üretilen görsel ve transkript arayüzde görüntülenir.

## 📂 Dosya Yapısı
- `app.py` : Ana Streamlit uygulaması
- `recorder.py` : Ses kaydı modülü
- `transcriptor.py` : Ses-metin dönüştürücü modül
- `painter.py` : Görsel üretim modülü
- `icons/` : Uygulama ikonları ve görselleri

## 🖋️ Notlar
- OpenAI API anahtarınızın aktif ve yeterli kotaya sahip olduğundan emin olun.
- macOS'ta mikrofon erişimi için uygulamaya izin verin.
- Eğer OpenAI Whisper API kotanız yoksa, yerel transkriptör kullanabilirsiniz.

## Lisans
Bu proje eğitim ve kişisel kullanım amaçlıdır. 🧘🏼‍♀️
