# VocalClear - AI Audio Isolation

VocalClear is a locally hosted, AI-powered desktop utility engineered for precise, high-fidelity audio track isolation. **Simply put: it completely removes background music and instruments, leaving you with crystal-clear human vocals.**

*Note: VocalClear is a closed-source application. This repository serves strictly as the official release host, technical documentation center, and issue tracker.*

## 📥 Releases & Installation
The latest standalone Windows executable is available directly via GitHub Releases:
**[Download Latest Release (v1.0.1)](https://github.com/HashTheDev-hub/VocalClear-Updates/releases/latest/download/VocalClear-Setup-v1.0.1.zip)**

---

## ⚙️ Technical Architecture
VocalClear is built to maximize local hardware efficiency and prevent data loss during heavy batch operations:

*   **Adaptive ETA Algorithm:** Features a custom time-estimation algorithm with a self-healing threshold that tracks multi-stage processing and adapts to hardware capabilities in real-time.
*   **Optimized Memory Allocation:** Dynamically manages PyTorch VRAM allocation to prevent memory fragmentation and system crashes during the processing of massive media files.
*   **Context Menu Integration:** Hooks directly into the Windows Registry, allowing users to send media files or entire directories to the inference pipeline directly from Windows Explorer.
*   **Dynamic FFmpeg Pipeline:** Natively parses multi-track MKV/MP4 files. It allows for targeted audio stream extraction and rebuilds media with strict packet interleaving synchronization.
*   **Lossless Output:** Processes audio at full native resolution without applying secondary compression algorithms.
*   **Inference Behavior:** Deep learning isolation relies on overlapping frequency complexity. While highly accurate, the AI may occasionally filter non-musical environmental noise, identifying it as an artifact meant for removal.

## 💻 System Requirements
*   **OS:** Windows 10 / Windows 11 (64-bit).
*   **GPU:** CUDA-enabled NVIDIA GPU is highly recommended for accelerated inference, though CPU fallback is supported.
*   **Storage:** 6 GB minimum free disk space.
*   **Network:** Required only once for initial license verification.

## 🐛 Issue Tracking
Please use the **[Issues](../../issues)** tab to report bugs, crashes, or request features. Include steps to reproduce and any relevant system specs when opening a ticket.

## 💖 Support
If you find this utility valuable for your workflow, consider supporting its continued development by obtaining a Pro license:
**[Get License on Gumroad](https://hashthedev.gumroad.com/l/VocalClear-Pro)**

---
---

# المستودع الرسمي | VocalClear - AI

يعد VocalClear أداة مكتبية محلية مدعومة بالذكاء الاصطناعي، تمت هندستها لعزل المسارات الصوتية بدقة وجودة عالية. **بمعنى أوضح: التطبيق يقوم بإزالة الموسيقى والخلفيات الصوتية تماماً، ليترك لك الصوت البشري بنقاء تام.**

*ملاحظة: هذا التطبيق مغلق المصدر. يُستخدم هذا المستودع حصرياً لاستضافة الإصدارات، التوثيق التقني، وتتبع الأخطاء البرمجية (Issue Tracker).*

## 📥 التحميل
الإصدار الأخير لنظام ويندوز متاح للتحميل المباشر:
**[تحميل أحدث إصدار (v1.0.1)](https://github.com/HashTheDev-hub/VocalClear-Updates/releases/latest/download/VocalClear-Setup-v1.0.1.zip)**

---

## ⚙️ البنية التقنية
تم بناء البرنامج لاستغلال كفاءة العتاد المحلي ومنع فقدان البيانات أثناء معالجة الملفات الضخمة:

*   **خوارزمية وقت التقدير (ETA):** خوارزمية مخصصة تتتبع مراحل المعالجة وتصحح نفسها ذاتياً بناءً على قدرات العتاد في الوقت الفعلي.
*   **إدارة الذاكرة (VRAM):** إدارة ديناميكية لذاكرة PyTorch لتجنب تجزئة الذاكرة ومنع الانهيار أثناء جلسات المعالجة الطويلة.
*   **تكامل مع سجل نظام ويندوز (Registry):** يتيح إرسال الملفات أو المجلدات مباشرة لمعالج الذكاء الاصطناعي عبر النقر بزر الفأرة الأيمن (Context Menu).
*   **مسار FFmpeg ديناميكي:** تحليل ذكي للفيديوهات متعددة المسارات (MKV/MP4) مع القدرة على تحديد مسارات معينة وإعادة بناء الملف بتزامن دقيق.
*   **مخرجات أصلية (Lossless):** معالجة الصوت بكامل الجودة دون أي خوارزميات ضغط ثانوية.
*   **سلوك نموذج الذكاء الاصطناعي:** تعتمد دقة العزل على تداخل الترددات. قد يقوم النموذج أحياناً بحذف المؤثرات البيئية غير الموسيقية ظناً منه أنها عناصر تتطلب الإزالة.

## 💻 متطلبات النظام
*   **نظام التشغيل:** ويندوز 10 / ويندوز 11 (64-بت).
*   **معالج الرسومات (GPU):** يُنصح بشدة باستخدام كرت شاشة NVIDIA (مدعوم بـ CUDA) لتسريع المعالجة، مع توفر دعم المعالجة عبر المعالج المركزي (CPU).
*   **مساحة التخزين:** 6 جيجابايت كحد أدنى.
*   **الشبكة:** اتصال بالإنترنت مطلوب لمرة واحدة فقط للتحقق من الترخيص.

## 🐛 تتبع الأخطاء (Issues)
يرجى استخدام قسم **[Issues](../../issues)** للإبلاغ عن أي خطأ برمجي (Bug) أو كراش.

## 💖 دعم التطوير
لدعم استمرارية تطوير هذه الأداة، يمكنك الحصول على الترخيص الاحترافي عبر:
**[شراء الترخيص من Gumroad](https://hashthedev.gumroad.com/l/VocalClear-Pro)**

---
### 🌍 Supported Languages - اللغات المدعومة
*   **English:** (English - Full support)
*   **Arabic:** (العربية - دعم كامل باستثناء السجل (اللوق))
*   **Spanish:** (Español - Mayormente compatible - Traducido por IA)
*   **Portuguese (BR):** (Português BR - Principalmente compatível - Traduzido por IA)
*   **Turkish:** (Türkçe - Büyük ölçüde uyumlu - Yapay zeka tarafından çevrildi)
*   **Russian:** (Русский - В основном поддерживается - Переведено ИИ)
*   **Chinese (Simplified):** (简体中文 - 主要支持 - 由 AI 翻译)
*   **Japanese:** (日本語 - 大部分対応 - AIによる翻訳)
*   **Korean:** (한국어 - 대부분 지원 - AI 번역)
