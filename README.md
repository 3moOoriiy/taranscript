# 🎬 أداة تحويل الفيديو إلى نص
## Video Transcription Tool

أداة ويب قوية لاستخراج النص من ملفات الفيديو باستخدام تقنية التعرف على الكلام. مبنية بـ Streamlit وتدعم عدة لغات وصيغ فيديو.

A powerful web-based tool for extracting text from video files using speech recognition technology. Built with Streamlit and supports multiple languages and video formats.

![Python](https://img.shields.io/badge/python-v3.7+-blue.svg)
![Streamlit](https://img.shields.io/badge/streamlit-v1.28+-red.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## ✨ المميزات | Features

- 🎥 **صيغ فيديو متعددة** | Multiple Video Formats: MP4, AVI, MOV, MKV, WebM, FLV, M4V
- 🌍 **دعم عدة لغات** | Multi-language Support: العربية، الإنجليزية، الفرنسية، الألمانية، الإسبانية، وأكثر
- 🚀 **معالجة سريعة** | Fast Processing: تقسيم ذكي للصوت للمعالجة الفعالة
- 💾 **خيارات تصدير متعددة** | Multiple Export Options: تحميل كملف نصي أو ملف ترجمة SRT
- 📱 **تصميم متجاوب** | Responsive Design: يعمل على الحاسوب والهاتف
- 🎛️ **إعدادات قابلة للتخصيص** | Customizable Settings: مدة قابلة للتعديل للحصول على أفضل النتائج
- 📊 **تتبع المعالجة** | Real-time Progress: شريط تقدم مرئي أثناء المعالجة

## 🔧 المتطلبات | Requirements

- Python 3.7 أو أحدث | Python 3.7+
- اتصال بالإنترنت للتعرف على الكلام | Internet connection for speech recognition
- مساحة تخزين كافية (1-2 GB) | Sufficient storage space (1-2 GB)
- FFmpeg (للمعالجة المتقدمة) | FFmpeg (for advanced processing)

## 🚀 التثبيت السريع | Quick Installation

### الطريقة الأولى: التثبيت التلقائي | Method 1: Automatic Installation

```bash
# تحميل المشروع | Download project
git clone https://github.com/your-username/video-transcription-tool.git
cd video-transcription-tool

# تشغيل التثبيت التلقائي | Run automatic installer
python install.py

# تشغيل التطبيق | Run application
python run.py
```

### الطريقة الثانية: التثبيت اليدوي | Method 2: Manual Installation

```bash
# إنشاء بيئة افتراضية (اختياري) | Create virtual environment (optional)
python -m venv venv
source venv/bin/activate  # Linux/Mac
# أو | or
venv\Scripts\activate     # Windows

# تثبيت المكتبات | Install packages
pip install -r requirements.txt

# تشغيل التطبيق | Run application
streamlit run app.py
```

## 📖 كيفية الاستخدام | How to Use

1. **فتح التطبيق** | Open the application
   ```bash
   python run.py
   ```

2. **اختيار الإعدادات** | Choose settings:
   - اختر لغة الفيديو | Select video language
   - حدد مدة كل جزء | Set chunk duration

3. **رفع الفيديو** | Upload video:
   - اسحب وأسقط الملف | Drag and drop file
   - أو اضغط لاختيار الملف | Or click to select

4. **بدء المعالجة** | Start processing:
   - اضغط "بدء استخراج النص" | Click "Start Text Extraction"
   - انتظر انتهاء المعالجة | Wait for processing to complete

5. **تحميل النتيجة** | Download results:
   - حمل كملف نصي | Download as text file
   - أو كملف ترجمة SRT | Or as SRT subtitle file

## 🎯 نصائح للحصول على أفضل النتائج | Tips for Best Results

### 🎤 جودة الصوت | Audio Quality
- استخدم فيديوهات بصوت واضح | Use videos with clear audio
- تجنب الضوضاء الخلفية | Avoid background noise
- تأكد من جودة الصوت العالية | Ensure high audio quality

### 🗣️ طريقة الكلام | Speaking Style
- كلام واضح ومفهوم | Clear and understandable speech
- سرعة مناسبة (ليس سريع جداً) | Appropriate speed (not too fast)
- فترات صمت قصيرة بين الجمل | Short pauses between sentences

### ⚙️ الإعدادات | Settings
- اختر اللغة الصحيحة | Select the correct language
- قلل مدة الأجزاء للكلام السريع | Reduce chunk duration for fast speech
- زد المدة للمحادثات الهادئة | Increase duration for quiet conversations

## 📁 هيكل المشروع | Project Structure

```
video-transcription-tool/
├── app.py              # الملف الرئيسي | Main application
├── install.py          # سكريپت التثبيت | Installation script
├── run.py              # ملف التشغيل | Run script
├── requirements.txt    # المكتبات المطلوبة | Required packages
└── README.md          # هذا الملف | This file
```

## 🛠️ استكشاف الأخطاء | Troubleshooting

### خطأ في تثبيت PyAudio | PyAudio Installation Error

**Windows:**
```bash
pip install pipwin
pipwin install pyaudio
```

**Linux/Ubuntu:**
```bash
sudo apt-get install portaudio19-dev python3-pyaudio
pip install pyaudio
```

**macOS:**
```bash
brew install portaudio
pip install pyaudio
```

### خطأ في معالجة الفيديو | Video Processing Error

- تأكد من صيغة الفيديو المدعومة | Ensure supported video format
- تحقق من وجود صوت في الفيديو | Check audio track exists
- جرب تقليل مدة الأجزاء | Try reducing chunk duration
- تأكد من تثبيت FFmpeg | Ensure FFmpeg is installed

### مشاكل في التعرف على الكلام | Speech Recognition Issues

- تحقق من اتصال الإنترنت | Check internet connection
- جرب لغة مختلفة | Try different language
- تحسين جودة الصوت | Improve audio quality
- تقليل الضوضاء الخلفية | Reduce background noise

## 📚 المكتبات المستخدمة | Libraries Used

- **Streamlit**: واجهة الويب | Web interface
- **SpeechRecognition**: التعرف على الكلام | Speech recognition
- **pydub**: معالجة الصوت | Audio processing
- **moviepy**: معالجة الفيديو | Video processing
- **requests**: طلبات HTTP | HTTP requests

## 🤝 المساهمة | Contributing

نرحب بالمساهمات! | Contributions are welcome!

1. Fork المشروع | Fork the project
2. إنشاء فرع للميزة | Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit التغييرات | Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push للفرع | Push to branch (`git push origin feature/AmazingFeature`)
5. فتح Pull Request | Open Pull Request

## 📜 الترخيص | License

هذا المشروع مرخص تحت رخصة MIT - انظر ملف [LICENSE](LICENSE) للتفاصيل.

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 المطور | Developer

**Your Name**
- GitHub: [@your-username](https://github.com/your-username)
- Email: your.email@example.com

## 🙏 شكر وتقدير | Acknowledgments

- Google Speech Recognition API
- Streamlit Community
- MoviePy Contributors
- pydub Developers

---

**ملاحظة**: هذا المشروع يستخدم Google Speech Recognition API المجاني والذي له حدود استخدام. للاستخدام التجاري المكثف، يُنصح بالترقية إلى خدمة مدفوعة.

**Note**: This project uses the free Google Speech Recognition API which has usage limits. For intensive commercial use, upgrading to a paid service is recommended.
