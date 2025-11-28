# 🇿🇼 Shona Language Resources

<div align="center">

![Shona Language](https://via.placeholder.com/1000x200/E65100/FFFFFF?text=Shona+Language+Datasets+%26+Resources)

**Comprehensive collection of Shona speech and text datasets for NLP research**

</div>

---

## 📊 Overview

Shona is a Bantu language spoken by approximately **14+ million people**, primarily in Zimbabwe. This page catalogs available datasets for:

- 🎙️ **Automatic Speech Recognition (ASR)**
- 🗣️ **Text-to-Speech (TTS)**
- 💬 **Question Answering (QA)**
- 🔤 **Language Modeling**
- 🗨️ **Conversational AI**

---

## 🎤 Speech Datasets

### 1. Mozilla Common Voice - Shona
**Status:** ✅ Publicly Available

- **Description:** Community-contributed voice recordings
- **Size:** Varies (updated regularly)
- **License:** CC0 1.0 (Public Domain)
- **Quality:** Crowdsourced, variable quality
- **Use Cases:** ASR training, speaker verification
- **Link:** [Common Voice Shona](https://commonvoice.mozilla.org/sn)

**Access:**
```bash
# Download via datasets library
from datasets import load_dataset
dataset = load_dataset("mozilla-foundation/common_voice_11_0", "sn")
```

---

### 2. Badrex Shona Speech Dataset
**Status:** ✅ Publicly Available

- **Description:** Curated Shona audio recordings with transcriptions
- **Size:** ~5 hours
- **Format:** Audio + transcriptions
- **License:** CC-BY-4.0
- **Quality:** High-quality, verified transcriptions
- **Use Cases:** ASR fine-tuning, baseline models
- **Link:** [HuggingFace - Badrex](https://huggingface.co/datasets/badrex/shona-speech)

**Access:**
```python
from datasets import load_dataset
dataset = load_dataset("badrex/shona-speech")
```

---

### 3. Shekharmeena Shona Male Audio Dataset
**Status:** ✅ Publicly Available | 🆕 **NEW**

- **Description:** Small Shona audio collection with transcribed text
- **Speaker Type:** Male voices
- **Size:** Limited (ideal for experiments)
- **Format:** Audio files + text transcriptions
- **Quality:** Clean recordings, transcribed
- **Use Cases:** ASR fine-tuning, proof-of-concept projects
- **Link:** [HuggingFace - Shekharmeena](https://huggingface.co/datasets/Shekharmeena/Shona-Male-Audio-Dataset)

**Access:**
```python
from datasets import load_dataset
dataset = load_dataset("Shekharmeena/Shona-Male-Audio-Dataset")
```

**⚠️ Note:** Small dataset size - best used as supplementary data or for initial experiments.

---

## 📝 Text Corpora

### 4. Leipzig Corpora Collection - Shona
**Status:** ✅ Publicly Available

- **Description:** Multiple Shona web corpora scraped from various sources
- **Years Available:** 2016, 2018, 2019, and more
- **Size:** Varies by version (10K - 1M+ sentences)
- **Format:** Sentence-level text files
- **License:** Free for non-commercial use
- **Use Cases:** 
  - Language modeling
  - QA context generation
  - TTS text sources
  - Synthetic QA dataset creation
- **Link:** [Leipzig Corpora - Shona](https://wortschatz.uni-leipzig.de/en/download/Shona)

**Available Versions:**
| Year | Sentences | Size |
|------|-----------|------|
| 2016 | 100K | ~5 MB |
| 2018 | 300K | ~15 MB |
| 2019 | 1M | ~50 MB |

**Access:**
```bash
# Download from Leipzig website
wget https://downloads.wortschatz-leipzig.de/corpora/sna_web_2019_1M.tar.gz
tar -xzf sna_web_2019_1M.tar.gz
```

---

## 💬 Conversational & Slang Datasets

### 5. Shona-English Slang Dataset
**Status:** ✅ Publicly Available | 🆕 **NEW** | 🔥 **HOT**

- **Paper:** "Advancing Conversational AI with Shona Slang" (2025)
- **Description:** Annotated Shona-English slang dataset with:
  - Intent labels
  - Sentiment annotations
  - Dialogue acts
  - Code-mixing tags
- **Size:** Dataset size in paper/repository
- **Format:** CSV with multiple annotation layers
- **Use Cases:**
  - Conversational AI / Chatbots
  - Code-switching research
  - Sentiment analysis
  - Intent recognition
  - Dialogue systems
- **Links:** 
  - [GitHub Dataset](https://github.com/HappymoreMasoka/Working_with_shona-slang/blob/main/slang_dataset_with_contexts_and_intent.csv)
  - [Research Paper](https://arxiv.org/search/?query=Advancing+Conversational+AI+with+Shona+Slang) *(if available)*

**Dataset Features:**
```python
# Expected columns
- text: Shona/English mixed text
- intent: User intent classification
- sentiment: Positive/Negative/Neutral
- dialogue_act: Question/Statement/Command
- code_mixing: Language tags
- context: Conversational context
```

**Access:**
```bash
# Clone repository
git clone https://github.com/HappymoreMasoka/Working_with_shona-slang.git
cd Working_with_shona-slang

# Or download directly
wget https://raw.githubusercontent.com/HappymoreMasoka/Working_with_shona-slang/main/slang_dataset_with_contexts_and_intent.csv
```

**Research Citation:**
```bibtex
@article{masoka2025shona,
  title={Advancing Conversational AI with Shona Slang},
  author={Masoka, Happymore and colleagues},
  year={2025},
  note={Dataset available at GitHub}
}
```

---

## 📈 Dataset Comparison

<div align="center">

| Dataset | Type | Size | Quality | Best For |
|---------|------|------|---------|----------|
| **Common Voice** | Speech | Variable | Mixed | Large-scale ASR |
| **Badrex** | Speech | ~5 hrs | High | ASR fine-tuning |
| **Shekharmeena** | Speech | Small | Good | Experiments |
| **Leipzig** | Text | 1M+ sent | High | Language models |
| **Slang Dataset** | Text | Variable | High | Conversational AI |

</div>

---

## 🎯 Recommended Use Cases

### ASR Model Training
```
Primary: Mozilla Common Voice + Badrex
Supplementary: Shekharmeena dataset
```

### TTS System Development
```
Text Source: Leipzig Corpora (2019 version)
Validation: Badrex transcriptions
```

### Conversational AI / QA Systems
```
Primary: Shona-English Slang Dataset
Context: Leipzig Corpora
Validation: Common Voice (for voice interface)
```

### Language Modeling
```
Training: Leipzig Corpora (all versions)
Fine-tuning: Slang Dataset
Evaluation: Badrex transcriptions
```

---

## ⚠️ Important Caveats

### Data Scarcity
- **Large, high-quality Shona ASR corpora remain scarce**
- Most pan-African projects focus on accented English rather than native Shona
- Example: [AfriSpeech-200](https://huggingface.co/datasets/intronhealth/afrispeech-200) is useful for methodology but contains limited Shona audio

### Data Quality Considerations
- **Common Voice:** Community-contributed, requires quality filtering
- **Leipzig Corpora:** Web-scraped, may contain noise/encoding issues
- **Slang Dataset:** Reflects informal language, may not suit formal applications

### License Compliance
Always check and comply with dataset licenses:
- ✅ CC0 / CC-BY: Permissive for commercial use
- ⚠️ Non-commercial: Academic use only
- ⚠️ Custom licenses: Read terms carefully

---

## 🔮 Future Additions

We're working on:

- [ ] Tone-marked Shona corpus (linguistic analysis)
- [ ] Dialect-specific collections (Zezuru, Karanga, Manyika, Korekore)
- [ ] Code-switched Shona-English speech data
- [ ] Low-resource dialect recordings
- [ ] Shona sign language integration

**Want to contribute?** See our [Contributing Guidelines](../CONTRIBUTING.md)

---

## 📚 Research Papers

### Key Publications on Shona NLP

1. **"Advancing Conversational AI with Shona Slang"** (2025)
   - Introduces slang dataset with multi-layer annotations
   - [GitHub](https://github.com/HappymoreMasoka/Working_with_shona-slang)

2. **"Low-Resource ASR for Bantu Languages"** (Various)
   - Check Masakhane publications
   - [Masakhane.io](https://www.masakhane.io/)

3. **"Mozilla Common Voice: Massively Multilingual ASR"**
   - Includes Shona as one of 100+ languages
   - [Paper](https://commonvoice.mozilla.org/en/datasets)

---

## 🛠️ Tools & Libraries

### Recommended Processing Tools

```python
# Audio processing
import librosa
import torchaudio

# Text processing
from datasets import load_dataset
import pandas as pd

# ASR frameworks
from transformers import Wav2Vec2ForCTC
import nemo.collections.asr as nemo_asr
```

---

## 📞 Contact & Contributions

Found a new Shona dataset? Have quality improvements?

1. 📝 [Open an Issue](https://github.com/SeViVI-Tese/voxAfrica/issues) with tag `shona-dataset`
2. 📧 Email: nashaa182@gmail.com
3. 💬 [Start a Discussion](https://github.com/SeViVI-Tese/voxAfrica/discussions)

---

<div align="center">

**🌟 This page is actively maintained**

*Last updated: November 2025*

[![Contributions](https://img.shields.io/badge/contributions-welcome-brightgreen)](../CONTRIBUTING.md)
[![License](https://img.shields.io/badge/license-MIT-blue)](../LICENSE)

</div>
