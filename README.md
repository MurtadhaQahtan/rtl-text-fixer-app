# RTL Text Fixer – Arabic, Persian, Urdu and Hebrew text for apps without RTL support (Windows)

[![Get it from Microsoft Store](https://get.microsoft.com/images/en-us%20dark.svg)](https://apps.microsoft.com/detail/9NQC161JJM09)

**RTL Text Fixer** (Microsoft Store ID `9NQC161JJM09`, US$2.99, v1.0) is a Windows 10/11 app
that fixes right-to-left text for programs that don't support it, such as Adobe Premiere Pro, After Effects, Unity,
Blender, many game engines and 3D/video tools. In those programs Arabic letters appear disconnected and RTL text appears
backwards. RTL Text Fixer converts the text so it displays correctly there:

- **Arabic-script languages** — Arabic, Persian, Urdu, Kurdish (Sorani), Pashto, Sindhi, Uyghur: letters are converted to
  connected Unicode presentation forms (isolated / initial / medial / final, lam-alef ligatures) and reordered into visual order.
- **Hebrew and Yiddish**: reordered into visual order (no shaping needed); niqqud can be kept or removed.
- Numbers and English words inside RTL text keep the correct order (Unicode Bidirectional Algorithm, UAX #9); brackets are mirrored.

Type or paste text into the window and copy the live result, or copy text anywhere, press **Ctrl+Shift+R** (configurable)
and paste. Pressing the hotkey again restores the original. An **Unshape** mode turns reshaped text back into normal, editable text.

| Input | Output (visual order — looks reversed in RTL-aware viewers like this one) | Language |
|---|---|---|
| مرحباً بكم في Adobe Premiere Pro 2025 | `Adobe Premiere Pro 2025 ﻲﻓ ﻢﻜﺑ ﺎًﺒﺣﺮﻣ` | Arabic |
| این متن فارسی در After Effects درست است | `ﺖﺳﺍ ﺖﺳﺭﺩ After Effects ﺭﺩ ﯽﺳﺭﺎﻓ ﻦﺘﻣ ﻦﯾﺍ` | Persian |
| اردو متن اب Unity میں درست ہے | `ﮯﮨ ﺖﺳﺭﺩ ﮟﯿﻣ Unity ﺏﺍ ﻦﺘﻣ ﻭﺩﺭﺍ` | Urdu |
| کوردستان و هەولێر | `ﺭێﻝﻭﻪﻫ ﻭ ﻥﺎﺘﺳﺩﺭﻮﮐ` | Kurdish (Sorani) |
| שלום עולם – גרסה 2.0 ב-Blender | `Blender-ב 2.0 הסרג – םלוע םולש` | Hebrew |

- Options: diacritics keep / remove / spacing forms; base direction auto / RTL / LTR; visual order on/off (for apps that
  already order RTL text but don't connect letters); reverse line order; wrap long lines; remove ZWNJ/ZWJ.
- Script and language auto-detection; runs in the system tray; optional start with Windows.
- UI in 12 languages (en, ar, fa, ur, he, tr, ru, es, fr, de, pt-BR, hi) with RTL layout for ar/fa/ur/he.
- Fully offline: no telemetry, ads or accounts ([privacy policy](https://murtadhaqahtan.github.io/rtl-text-fixer-site/privacy.html)).
- Limitations: letters that have no presentation forms in Unicode (e.g. Kurdish ڵ ڕ ێ, Pashto ټ ځ څ ډ ړ ږ ښ ګ ڼ ۍ) cannot
  be connected by any reshaper and are shown unconnected; the target app's font must contain Arabic presentation forms;
  Urdu appears in Naskh style, not Nastaliq; output is per line, so if the target app re-wraps a long line the lines appear
  in the wrong order (use the wrap option); it does not translate. Windows only (10 1809+ / 11, x64 and ARM64).

Website (12 languages, FAQ): https://murtadhaqahtan.github.io/rtl-text-fixer-site/ ·
Store: https://apps.microsoft.com/detail/9NQC161JJM09

The source code is private. This repository only describes the app. Questions: hibari@mail.grokbot.com
