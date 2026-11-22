# arabic-calligraphy-ornament-multimodal-dataset
---
license: cc-by-4.0
language:
  - ar
  - en
task_categories:
  - question-answering
  - text-generation
  - image-to-text
  - text-to-image
pretty_name: Arabic Calligraphy & Islamic Ornament Dataset (2M Records)
tags:
  - arabic-calligraphy
  - islamic-art
  - arabesque
  - geometric-patterns
  - svg
  - color-palettes
  - image-generation-prompts
  - cultural-heritage
  - nlp
  - multimodal
size_categories:
  - 1M<n<10M
---

# مجموعة بيانات الخط العربي والفنون والزخارف الإسلامية
### (Arabic Calligraphy & Islamic Art Dataset)

## نظرة عامة (Overview)

تُقدّم هذه المجموعة بنية بيانات غنية ومُهيكلة بصيغة **JSONL** تضم **2,000,000 سجل** (بواقع **250,000 سجل** في كل ملف من **8 ملفات متخصصة**) وحجم إجمالي **1,466.83 MB**، لتغطية أبعاد الخط العربي، الزخرفة الإسلامية، المدارس الخطية، لوحات الألوان، أوصاف اللوحات، الأسئلة المعرفية، وتوليد الأنماط الهندسية بلغة **SVG**.

تم توليد هذه البيانات عبر محرك توليد برمجي متخصص يجمع بين المفاهيم الأصيلة لفنون الخط والزخرفة الإسلامية وبين متطلبات أنظمة الذكاء الاصطناعي الحديثة، مما يجعلها مورداً عملياً لتدريب وتقييم نماذج اللغة (**LLMs**)، والنماذج متعددة الوسائط (**Multimodal & Diffusion / Image Generation Workflows**)، وأنظمة التصميم والرسوم المتجهة (**SVG & UI/Generative Design**).

---

## ملخص إحصاءات المجموعة (Dataset Statistics)

- **إجمالي السجلات:** `2,000,000` سجل
- **الحجم الإجمالي للملفات:** `1,466.83 MB`
- **عدد الملفات:** `8` ملفات (`JSONL`، ترميز `UTF-8`)
- **الترخيص:** `CC BY 4.0`

| # | الملف | المحور الفني / المعرفي | عدد السجلات | الحجم |
| :---: | :--- | :--- | :---: | :---: |
| 1 | `islamic_art_calligraphy_rules.jsonl` | قواعد الخط والنسب (Calligraphy Rules) | 250,000 | 126.88 MB |
| 2 | `islamic_art_image_prompts.jsonl` | أوامر توليد الصور (Image Prompts - AR/EN) | 250,000 | 339.65 MB |
| 3 | `islamic_art_descriptions.jsonl` | أوصاف اللوحات والعناصر البصرية (Artwork Descriptions) | 250,000 | 292.35 MB |
| 4 | `islamic_art_qa.jsonl` | أسئلة وأجوبة معرفية (Islamic Art QA) | 250,000 | 138.87 MB |
| 5 | `islamic_art_color_palettes.jsonl` | لوحات الألوان وقيم HEX (Color Palettes) | 250,000 | 163.53 MB |
| 6 | `islamic_art_ornament_patterns.jsonl` | الأنماط الزخرفية والهندسية (Ornament Patterns) | 250,000 | 226.58 MB |
| 7 | `islamic_art_schools.jsonl` | المدارس الخطية وأعلامها (Calligraphy Schools) | 250,000 | 109.45 MB |
| 8 | `islamic_art_svg_patterns.jsonl` | أنماط زخرفية برمجية SVG (SVG Patterns) | 250,000 | 169.51 MB |

---

## توافر البيانات (Data Availability)

المجموعة متاحة مجاناً على المنصتين التاليتين:

| المنصة | الرابط |
| :--- | :--- |
| 🤗 **Hugging Face** | [Abdulrhman472001/arabic-calligraphy-ornament-multimodal-dataset](https://huggingface.co/datasets/Abdulrhman472001/arabic-calligraphy-ornament-multimodal-dataset) |
| 📊 **Kaggle** | [abdulrhmanamr47/arabic-calligraphy-ornament-multimodal-dataset](https://www.kaggle.com/datasets/abdulrhmanamr47/arabic-calligraphy-ornament-multimodal-dataset) |

- **Hugging Face:** https://huggingface.co/datasets/Abdulrhman472001/arabic-calligraphy-ornament-multimodal-dataset
- **Kaggle:** https://www.kaggle.com/datasets/abdulrhmanamr47/arabic-calligraphy-ornament-multimodal-dataset

---

## القيمة العلمية والفنية والتقنية (Why This Dataset Matters)

1. **جسر بين التراث الفني الأصيل والذكاء الاصطناعي التوليدي:** توثّق المجموعة معارف دقيقة مثل نسب الحروف بالنقاط (`5-7 نقاط` في الثلث)، أنواع الخط الكوفي، المقرنصات، المدارس الخطية، والأرابيسك والزخارف الهندسية، مع ربطها بأوامر توليد صور ثنائية اللغة (`prompt_ar` و `prompt_en` و `negative_prompt`) وأكواد `SVG` جاهزة للتنفيذ.
2. **تنوع المخرجات من النصوص إلى الكود البصري:** لا تقتصر المجموعة على النصوص الوصفية، بل تضم أكواد `SVG` هندسية صالحة للاستخدام المباشر في الويب أو التحويل إلى رسوم، بالإضافة إلى لوحات ألوان مزودة بقيم `HEX` ووظائف الاستخدام والسمات المزاجية (`mood`).
3. **إثراء الوصف الفني والتحليل البصري:** يجمع ملف `descriptions` بين الوصف السردي الكامل (`full_description`) والعناصر البصرية المهيكلة (`visual_elements`: التكوين، التناغم اللوني، والإضاءة) والأبعاد والأدوات الخطية مثل قلم الخيزران.
4. **بنية موحدة ومتوافقة مع أدوات التدريب الحديثة:** تأتي جميع الملفات بصيغة `JSONL` نظيفة بترميز `UTF-8` (`ensure_ascii=False`) ومفاتيح إنجليزية واضحة تسهل قراءتها وتحميلها عبر `datasets` و `trl` وأطر العمل المختلفة.

---

## هيكل الملفات الثمانية وتفاصيلها (Dataset Structure)

### 1. قواعد الخط والنسب (`islamic_art_calligraphy_rules.jsonl`)

- **الهدف:** تمثيل قواعد الخطوط العربية، نسب الحروف، الخصائص البصرية، مجالات الاستخدام، والخطاطين أو الأنواع الفرعية.
- **الحقول الأساسية:** `id`, `type`, `script`, `letter`, `proportion`, `description`, `characteristics`, `uses`, `famous_calligraphers` (مع دعم حقول إضافية مثل `sub_types` عند توفرها).

### 2. أوامر توليد الصور (`islamic_art_image_prompts.jsonl`)

- **الهدف:** توفير أوامر تفصيلية عربية وإنجليزية وسلبية (`negative_prompt`) لتوليد لوحات الخط والزخرفة الإسلامية مع تحديد الخط، الزخرفة، الألوان، الخلفية، والإطار.
- **الحقول الأساسية:** `id`, `type`, `script`, `content`, `ornament_style`, `primary_color`, `secondary_color`, `background`, `frame`, `prompt_ar`, `prompt_en`, `negative_prompt`, `tags`.

### 3. أوصاف اللوحات (`islamic_art_descriptions.jsonl`)

- **الهدف:** وصف الأعمال الخطية والزخرفية من حيث الخط، الزخرفة، الاتجاه، المقاس، الأداة، الألوان، والعناصر البصرية المنظمة.
- **الحقول الأساسية:** `id`, `type`, `script`, `ornament`, `content`, `orientation`, `size`, `tool`, `primary_color`, `background`, `full_description`, `visual_elements`.

### 4. أسئلة وأجوبة معرفية (`islamic_art_qa.jsonl`)

- **الهدف:** دعم مهام الإجابة عن الأسئلة وبناء المساعدين المعرفيين المتخصصين في الخط العربي والعمارة والفنون الإسلامية.
- **الحقول الأساسية:** `id`, `type`, `question`, `answer`, `category`, `tags`.

### 5. لوحات الألوان (`islamic_art_color_palettes.jsonl`)

- **الهدف:** تقديم لوحات لونية مستوحاة من العمارة والزخارف الإسلامية مع أكواد `HEX`، واستخدامات كل لون، والمصدر الإلهامي والطابع المزاجي.
- **الحقول الأساسية:** `id`, `type`, `palette_name`, `colors`, `inspiration`, `mood`.

### 6. الأنماط الزخرفية (`islamic_art_ornament_patterns.jsonl`)

- **الهدف:** تحليل الأنماط الزخرفية (مثل الأرابيسك والأنماط الهندسية) حسب درجة التعقيد، التناظر، العناصر المكوّنة، الخصائص، والاستخدامات المقترحة.
- **الحقول الأساسية:** `id`, `type`, `pattern_name`, `complexity`, `symmetry`, `description`, `elements`, `characteristics`, `full_description`, `suggested_uses`.

### 7. المدارس الخطية (`islamic_art_schools.jsonl`)

- **الهدف:** توثيق المدارس الخطية التاريخية، فتراتها الزمنية، خصائصها، أعلامها، مناطق انتشارها، وأثرها الفني.
- **الحقول الأساسية:** `id`, `type`, `school_name`, `era`, `characteristics`, `pioneers`, `region`, `legacy`.

### 8. أنماط SVG (`islamic_art_svg_patterns.jsonl`)

- **الهدف:** توفير أنماط زخرفية وهندسية مكتوبة بصيغة `SVG` قابلة للتضمين المباشر أو التصدير والتطوير البرمجي.
- **الحقول الأساسية:** `id`, `type`, `pattern_type`, `description`, `svg_code`, `tags`, `usage`.

---

## أمثلة من السجلات (Data Samples)

**مثال من قواعد الخط والنسب (Calligraphy Rules):**

```json
{
  "id": 1,
  "type": "calligraphy_rule",
  "script": "الثلث",
  "letter": "الألف",
  "proportion": "5-7 نقاط",
  "description": "أم الخطوط وأصعبها، يتميز بالحروف الممتدة والتشكيلات الدقيقة",
  "characteristics": ["حروف ممتدة", "تشكيل كامل", "انسيابية عالية", "تداخل الحروف"],
  "uses": ["العناوين الرئيسية", "اللوحات الجدارية", "المصاحف", "القباب"],
  "famous_calligraphers": ["الشيخ حامد الآمدي", "حافظ عثمان", "محمد شوقي"]
}
```

**مثال من أوامر توليد الصور (Image Prompts):**

```json
{
  "id": 1,
  "type": "image_generation_prompt",
  "script": "الثلث",
  "content": "بسم الله الرحمن الرحيم",
  "ornament_style": "الأرابيسك",
  "primary_color": "الذهبي",
  "secondary_color": "الأزرق_اللازوردي",
  "background": "خلفية بيضاء ناصعة",
  "frame": "إطار ذهبي مزخرف",
  "prompt_ar": "لوحة فنية بخط الثلث يحمل نص 'بسم الله الرحمن الرحيم'، مع زخارف الأرابيسك متقنة، باللون الذهبي والأزرق_اللازوردي، خلفية بيضاء ناصعة، إطار ذهبي مزخرف. أسلوب فني كلاسيكي، دقة عالية، إضاءة متحفية.",
  "prompt_en": "Artistic الثلث calligraphy artwork with text 'بسم الله الرحمن الرحيم', intricate الأرابيسك patterns, الذهبي and الأزرق_اللازوردي color palette, خلفية بيضاء ناصعة, إطار ذهبي مزخرف. Classical Islamic art style, high detail, museum lighting, 8k resolution.",
  "negative_prompt": "أخطاء إملائية، تشويه في الحروف، زخارف غير متماثلة، ألوان فاقعة، نص غير واضح، جودة منخفضة",
  "tags": ["الثلث", "الأرابيسك", "الذهبي", "فن_إسلامي", "خط_عربي"]
}
```

**مثال من أنماط SVG (SVG Patterns):**

```json
{
  "id": 1,
  "type": "svg_pattern",
  "pattern_type": "نجمة_8",
  "description": "نجمة ثمانية بسيطة تتكون من مربعين متداخلين ودائرة محيطة",
  "svg_code": "<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 200 200\">  <g fill=\"none\" stroke=\"#D4AF37\" stroke-width=\"2\">    <rect x=\"50\" y=\"50\" width=\"100\" height=\"100\" transform=\"rotate(45 100 100)\"/>    <rect x=\"50\" y=\"50\" width=\"100\" height=\"100\"/>    <circle cx=\"100\" cy=\"100\" r=\"70\"/>  </g></svg>",
  "tags": ["زخرفة_هندسية", "فن_إسلامي", "SVG", "نمط_متكرر"],
  "usage": "يمكن استخدام هذا الكود مباشرة في تطبيقات الويب أو تحويله إلى صور"
}
```

---

## استخدامات مقترحة (Use Cases)

- **تدريب النماذج اللغوية ومتعددة الوسائط (SFT & Multimodal Training):** بناء مساعدين ومولدات تفهم مصطلحات الخط العربي والزخرفة الإسلامية وتصيغ أوامر فنية دقيقة.
- **تطبيقات التصميم والرسوم المتجهة (Generative Design & SVG Tools):** استلهام لوحات ألوان متناسقة وأنماط هندسية قابلة للتوليد أو المعاينة البرمجية.
- **التعليم والتوثيق الثقافي (EdTech & Digital Heritage):** إثراء المنصات التعليمية والموسوعات الرقمية بأسئلة وأجوبة ومعلومات منظمة حول الخطوط والمدارس الفنية.
- **التقييم والمعايير (Benchmarking):** اختبار قدرة النماذج على التمييز بين الخطوط والأنماط الزخرفية وتقديم شروح دقيقة.

---

## الترخيص (License)

هذه البيانات متاحة للعموم بموجب ترخيص المشاع الإبداعي نَسب المُصنَّف 4.0 دولي (CC BY 4.0). يُسمح بالمشاركة والتعديل والاستخدام التجاري والبحثي بشرط الإشارة إلى المصدر الأصلي.

---

## الاستشهاد (Citation)

إذا استخدمت هذه البيانات في أبحاثك أو نماذجك، يرجى الاستشهاد بها على النحو التالي:

```bibtex
@dataset{arabic_calligraphy_islamic_art_2026,
  author       = {Abd El Rahman Amr},
  title        = {Arabic Calligraphy & Islamic Art Dataset},
  year         = {2026},
  publisher    = {Hugging Face / Kaggle},
  license      = {CC-BY-4.0}
}
```

---

## تحميل البيانات وقراءتها عبر Python

> **ملاحظة:** الحجم الإجمالي يتجاوز **1.4 GB**؛ يُنصح بتحميل الملفات التي تحتاجها فقط، أو استخدام وضع البث (`streaming=True`) عند العمل عبر `datasets`.

### 1. التحميل من Hugging Face

تنزيل المجموعة كاملة إلى مجلد محلي عبر `huggingface_hub`:

```python
from pathlib import Path
from huggingface_hub import snapshot_download

local_dir = snapshot_download(
    repo_id="Abdulrhman472001/arabic-calligraphy-ornament-multimodal-dataset",
    repo_type="dataset",
    local_dir="./data_hf",
)
print("تم التنزيل إلى:", Path(local_dir).resolve())
```

أو تنزيل ملفات محددة فقط:

```python
from huggingface_hub import snapshot_download

snapshot_download(
    repo_id="Abdulrhman472001/arabic-calligraphy-ornament-multimodal-dataset",
    repo_type="dataset",
    local_dir="./data_hf",
    allow_patterns=["*islamic_art_qa.jsonl", "*islamic_art_svg_patterns.jsonl"],
)
```

أو التحميل المباشر عبر مكتبة `datasets` (لكل ملف حقول مختلفة، لذا يُحمَّل كل ملف على حدة):

```python
from datasets import load_dataset

REPO = "Abdulrhman472001/arabic-calligraphy-ornament-multimodal-dataset"

qa  = load_dataset(REPO, data_files="**/islamic_art_qa.jsonl", split="train")
svg = load_dataset(REPO, data_files="**/islamic_art_svg_patterns.jsonl", split="train")

print(qa)
print(qa[0])

# وضع البث للملفات الكبيرة دون تنزيلها كاملة
prompts = load_dataset(
    REPO,
    data_files="**/islamic_art_image_prompts.jsonl",
    split="train",
    streaming=True,
)
print(next(iter(prompts)))
```

### 2. التحميل من Kaggle

عبر مكتبة `kagglehub`:

```python
import kagglehub

dataset_path = kagglehub.dataset_download(
    "abdulrhmanamr47/arabic-calligraphy-ornament-multimodal-dataset"
)
print("مسار البيانات على الجهاز:", dataset_path)
```

أو عبر سطر الأوامر (Kaggle CLI):

```bash
kaggle datasets download -d abdulrhmanamr47/arabic-calligraphy-ornament-multimodal-dataset -p ./data_kaggle --unzip
```

### 3. قراءة ومعاينة أي ملف `.jsonl` محلياً

```python
import json
from pathlib import Path

# يبحث عن الملف داخل المجلد مهما كان مساره الفرعي
file_path = next(Path("./data_hf").rglob("islamic_art_qa.jsonl"))

records = []
with file_path.open("r", encoding="utf-8") as f:
    for i, line in enumerate(f):
        if line.strip():
            records.append(json.loads(line))
        if i >= 999:  # اقرأ أول 1000 سجل فقط للمعاينة السريعة
            break

print("عدد السجلات المقروءة:", len(records))
print("أول سجل:", records[0])
```

### 4. القراءة عبر pandas

```python
import pandas as pd
from pathlib import Path

path = next(Path("./data_hf").rglob("islamic_art_color_palettes.jsonl"))

# قراءة أول 10,000 سجل على دفعات لتوفير الذاكرة
chunks = pd.read_json(path, lines=True, chunksize=10_000)
df = next(chunks)

print(df.head())
print(df["mood"].value_counts().head(10))
```

### 5. معاينة نمط SVG وحفظه كصورة

```python
import json
from pathlib import Path

path = next(Path("./data_hf").rglob("islamic_art_svg_patterns.jsonl"))

with path.open("r", encoding="utf-8") as f:
    record = json.loads(next(f))

print(record["pattern_type"], "-", record["description"])

# حفظ الكود كملف SVG يمكن فتحه في أي متصفح
Path("pattern_1.svg").write_text(record["svg_code"], encoding="utf-8")

# عرض النمط داخل Jupyter Notebook
# from IPython.display import SVG, display
# display(SVG(data=record["svg_code"]))
```

### 6. تحويل أوامر توليد الصور إلى قوالب تعليمات (SFT)

```python
import json
from pathlib import Path

path = next(Path("./data_hf").rglob("islamic_art_image_prompts.jsonl"))
out = Path("sft_image_prompts.jsonl")

with path.open("r", encoding="utf-8") as src, out.open("w", encoding="utf-8") as dst:
    for i, line in enumerate(src):
        if i >= 1000:  # عيّنة تجريبية
            break
        r = json.loads(line)
        sample = {
            "instruction": f"اكتب أمر توليد صورة للوحة بخط {r['script']} بزخرفة {r['ornament_style']}.",
            "input": r["content"],
            "output": r["prompt_ar"],
        }
        dst.write(json.dumps(sample, ensure_ascii=False) + "\n")

print("تم الحفظ في:", out.resolve())
```
