# African Speech Datasets Catalog

<div align="center">

![African Languages](https://via.placeholder.com/1000x200/1976D2/FFFFFF?text=Pan-African+Speech+Datasets+Catalog)

**Curated collection of open datasets for ASR and TTS research in African and Bantu languages**

</div>

---

## 🌍 Public Datasets

### 🤝 Community-Driven Datasets

| Dataset | Languages | Hours | License | Link |
|---------|-----------|-------|---------|------|
| **Mozilla Common Voice** | Swahili, Luganda, Kinyarwanda +15 | Varies | CC0 | [Common Voice](https://commonvoice.mozilla.org/) |
| **Badrex Shona** | Shona | ~5 hrs | CC-BY-4.0 | [HuggingFace](https://huggingface.co/datasets/badrex/shona-speech) |
| **Shekharmeena Shona** 🆕 | Shona (Male) | Small | Check License | [HuggingFace](https://huggingface.co/datasets/Shekharmeena/Shona-Male-Audio-Dataset) |
| **FLEURS** | 102 languages (incl. African) | ~12 hrs/lang | CC-BY-4.0 | [Google Research](https://huggingface.co/datasets/google/fleurs) |
| **MMS (Meta)** | 1000+ languages | Varies | CC-BY-4.0 | [GitHub](https://github.com/facebookresearch/fairseq/tree/main/examples/mms) |

### 🔬 Research Collections

| Dataset | Languages | Domain | Link |
|---------|-----------|--------|------|
| **OpenSLR** | Zulu, Xhosa, Sesotho, +5 | General | [OpenSLR](https://www.openslr.org/resources.php) |
| **Masakhane ASR** | Pan-African (20+ langs) | Various | [GitHub](https://github.com/masakhane-io/masakhane-asr) |
| **Niger-Volta LT** | Yoruba, Hausa, Igbo | Mixed | [GitHub](https://github.com/Niger-Volta-LTI) |
| **ALFFA** | Amharic, Hausa, Swahili, Wolof | Broadcast | [GitHub](https://github.com/besacier/ALFFA_PUBLIC) |

### 📝 Text Corpora

| Dataset | Languages | Type | Link |
|---------|-----------|------|------|
| **Leipzig Corpora** 🆕 | Shona (multiple years) | Web text | [Leipzig](https://wortschatz.uni-leipzig.de/en/download/Shona) |
| **Shona Slang Dataset** 🆕 🔥 | Shona-English | Conversational | [GitHub](https://github.com/HappymoreMasoka/Working_with_shona-slang) |

---

## 🗺️ Language-Specific Resources

### 🇿🇼 Zimbabwe
- **Shona**: [Detailed Resources](shona_resources.md) | Common Voice, Badrex, Shekharmeena, Leipzig, Slang Dataset
- **Ndebele**: Common Voice (limited)

### 🇹🇿 Tanzania
- **Swahili**: Common Voice, FLEURS, OpenSLR

### 🇿🇦 South Africa
- **Zulu**: NCHLT, OpenSLR
- **Xhosa**: NCHLT, OpenSLR
- **Afrikaans**: NCHLT, Common Voice

### 🇳🇬 Nigeria
- **Yoruba**: Common Voice, Niger-Volta
- **Igbo**: Common Voice, Niger-Volta
- **Hausa**: ALFFA, OpenSLR

---

## 📊 Dataset Statistics Summary

| Region | Languages Covered | Total Hours | Datasets |
|--------|-------------------|-------------|----------|
| Southern Africa | 8+ | 100+ hrs | 15 |
| East Africa | 6+ | 80+ hrs | 12 |
| West Africa | 10+ | 120+ hrs | 18 |
| North Africa | 4+ | 40+ hrs | 6 |

---

## 🆕 Recent Additions (2025)

- ✅ **Shekharmeena Shona Male Audio Dataset** - Small but clean Shona speech corpus
- ✅ **Leipzig Shona Corpora** (2016-2019) - Large web-scraped text collections
- ✅ **Shona-English Slang Dataset** - Annotated conversational data with intent/sentiment labels

---

## 🎯 Recommended Starting Points

### For ASR Research
1. **Mozilla Common Voice** - Large-scale, multi-language
2. **Badrex Shona** - High-quality Shona baseline
3. **FLEURS** - Multilingual benchmark

### For TTS Development
1. **Leipzig Corpora** - Large text sources
2. **Common Voice** - Voice recordings for reference
3. **Badrex** - Quality transcriptions

### For Conversational AI
1. **Shona Slang Dataset** - Code-switching & intent
2. **Leipzig Corpora** - Context generation
3. **Common Voice** - Voice interface validation

---

## 📥 Quick Access Commands

```bash


# Badrex Shona
badrex = load_dataset("badrex/shona-speech")

# Shekharmeena Shona
shekhar = load_dataset("Shekharmeena/Shona-Male-Audio-Dataset")

# Leipzig Corpora (manual download)
wget https://downloads.wortschatz-leipzig.de/corpora/sna_web_2019_1M.tar.gz

# Slang Dataset
git clone https://github.com/HappymoreMasoka/Working_with_shona-slang.git
```

---

## 🚀 Upcoming Additions

- [ ] Tone-marked Shona corpus
- [ ] Ndebele conversational dataset
- [ ] Multi-dialect speech collections
- [ ] Low-resource language recordings
- [ ] Code-switched speech data

---

## 🤝 Contributing New Datasets

Have a dataset to share?

1. 📝 [Open an issue](https://github.com/SeViVI-Tese/voxAfrica/issues) with tag `dataset-submission`
2. Provide: Name, language(s), size, license, link, description
3. Ensure proper licensing documentation
4. Include access instructions

---

## ✅ Dataset Quality Guidelines

We prioritize datasets with:

- ✅ Clear licensing (preferably open/CC licenses)
- ✅ Transcription accuracy > 95%
- ✅ Diverse speakers (age, gender, region)
- ✅ Comprehensive metadata
- ✅ Audio quality >= 16kHz sampling rate
- ✅ Reproducible access methods

---

## 📚 Citation

When using these datasets, please cite:

1. **Original dataset creators** (check individual licenses)
2. **This catalog** (if helpful):

```bibtex
@misc{voxafrica_catalog2025,
  title={voxAfrica African Speech Datasets Catalog},
  author={{SeViVI-Tese AI Research}},
  year={2025},
  url={https://github.com/SeViVI-Tese/voxAfrica}
}
```

---

<div align="center">

**Last Updated:** November 25, 2025  
**Maintainers:** SeViVI-Tese AI Research Team

[![Star this repo](https://img.shields.io/github/stars/SeViVI-Tese/voxAfrica?style=social)](https://github.com/SeViVI-Tese/voxAfrica)

</div>
