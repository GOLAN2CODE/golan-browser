# Third-party source and notices / المصادر والتراخيص الخارجية

## English

This is an inventory of preserved local material and known source references, not a completed redistribution/license audit. No new license is assigned to application code: the original browser root had no project-wide LICENSE file.

| Component | Preserved source / reference |
|---|---|
| Compact Whisper runtime | `third_party/compact-asr/whisper-d1be6fde.tar.gz`, pinned commit `d1be6fde11ac6e0407606b4e42fe72d34add8037`, MIT notices, build script and four ABI payloads |
| Whisper tiny Q5_1 model | `app/src/main/assets/golan-asr/ggml-tiny-q5_1.bin`, model provenance/card, original OpenAI model and engine MIT notices |
| QuickJS | Complete `third_party/quickjs/quickjs-2026-06-04/` source tree and LICENSE, build script, provenance and ABI binaries |
| WebP runtime correction | `third_party/ffmpeg16k/source/libwebp-v1.6.0.tar.gz`, `licenses/` terms/patent notices, build/repack scripts |
| yt-dlp | Existing source-containing executable ZIP at `app/src/main/res/raw/ytdlp`; exact release version `2026.10.26`, URL and digest recorded in `third_party/yt-dlp/provenance.json` |
| youtube-dl-android / FFmpeg / Python | Pinned `io.github.junkfood02.youtubedl-android:library:0.18.1` and `:ffmpeg:0.18.1` Maven dependencies, retained modified delivery payloads, original AAR digests and transformation scripts |
| Other Android dependencies | Exact coordinates remain in `app/build.gradle`; these retain their own licenses |

Exact upstream references retained by the original project:

- [Whisper source commit](https://github.com/ggml-org/whisper.cpp/tree/d1be6fde11ac6e0407606b4e42fe72d34add8037)
- [Pinned Whisper model repository revision](https://huggingface.co/ggerganov/whisper.cpp/tree/5359861c739e955e79d9a303bcbc70fb988958b1)
- [yt-dlp release](https://github.com/yt-dlp/yt-dlp/releases/tag/2026.10.26)
- [youtube-dl-android 0.18.1](https://github.com/yausername/youtubedl-android/tree/0.18.1)
- [Original FFmpeg dependency AAR](https://repo.maven.apache.org/maven2/io/github/junkfood02/youtubedl-android/ffmpeg/0.18.1/ffmpeg-0.18.1.aar)
- [Original library AAR](https://repo.maven.apache.org/maven2/io/github/junkfood02/youtubedl-android/library/0.18.1/library-0.18.1.aar)
- [WebP1.6.0 source](https://github.com/webmproject/libwebp/archive/refs/tags/v1.6.0.tar.gz)

Unresolved review items: a complete per-member license/source/notice review of the bundled FFmpeg/Python runtimes and yt-dlp distribution has not been completed. The retained WebP source is not the full corresponding source of the FFmpeg runtime archive. The raw FFmpeg and yt-dlp ZIP inventories did not expose entries named LICENSE/COPYING/NOTICE; this bounded check is not a complete license determination. Preserve and review applicable upstream terms and any corresponding-source obligations. Compilation inputs and preserved local source are provided without claiming all dependency licensing obligations are cleared.

## العربية

هذا جرد لما حُفظ محليًا وروابط المصدر المعروفة، وليس شهادة اكتمال تدقيق الترخيص أو إعادة التوزيع. لم نضف ترخيصًا لكود المتصفح؛ الجذر الأصلي لم يتضمن ملف LICENSE شاملًا.

- مصدر Whisper المثبت ونموذجه وتراخيص MIT محفوظة في `third_party/compact-asr/` وأصول التطبيق؛ المصادر والنسخ التنفيذية للمعماريات الأربع موجودة.
- مصدر QuickJS الكامل وترخيصه وسكربت بنائه محفوظة في `third_party/quickjs/`.
- أرشيف WebP1.6.0 وتراخيصه وإشعارات البراءات وسكربتات إعادة بنائه محفوظة في `third_party/ffmpeg16k/`.
- محرك yt-dlp موجود كملف ZIP تنفيذي يتضمن كود Python في `app/src/main/res/raw/ytdlp`، وإصداره2026.10.26 ورابطه وبصمته في ملف provenance الخاص به.
- إصدارات اعتماديات youtube-dl-android وFFmpeg وPython وتحويلات حمولاتها مثبتة في Gradle وملفات provenance. بقية اعتماديات أندرويد تحتفظ بتراخيصها المستقلة.

الروابط أعلاه هي مراجع المصدر الدقيقة الموجودة في المشروع. يبقى تدقيق ترخيص ومصدر وإشعارات كل عضو من حمولات FFmpeg وPython وyt-dlp غير مكتمل. أرشيف WebP ليس المصدر المقابل الكامل لحمولة FFmpeg. لم يظهر في جرد ZIP المحدود لـFFmpeg وyt-dlp عضو باسم LICENSE أوCOPYING أوNOTICE؛ هذا لا يكفي لحكم ترخيص شامل. يجب الحفاظ على شروط الموردين ومراجعة التزامات المصدر عند تطبيقها؛ وجود ملفات البناء والمصادر المحفوظة لا يعني اعتماد امتثال جميع الاعتماديات.
