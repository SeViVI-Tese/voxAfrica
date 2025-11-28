# African Speech Datasets Catalog

A curated collection of open datasets for **Automatic Speech Recognition (ASR)** and **Text-to-Speech (TTS)** research in African and Bantu languages.

---

## Public Datasets

### Community-Driven Datasets

| Dataset | Languages | Hours | License | Link |
|---------|-----------|-------|---------|------|
| **Mozilla Common Voice** | Swahili, Luganda, Kinyarwanda, +10 | Varies | CC0 | [Common Voice](https://commonvoice.mozilla.org/) |
| **Badrex Shona** | Shona | ~5 hrs | CC-BY-4.0 | [HuggingFace](https://huggingface.co/datasets/badrex/shona-speech) |
| **FLEURS** | 102 languages (incl. African) | ~12 hrs/lang | CC-BY-4.0 | [Google Research](https://huggingface.co/datasets/google/fleurs) |
| **MMS (Meta)** | 1000+ languages | Varies | CC-BY-4.0 | [GitHub](https://github.com/facebookresearch/fairseq/tree/main/examples/mms) |

### Research Collections

| Dataset | Languages | Domain | Link |
|---------|-----------|--------|------|
| **OpenSLR** | Zulu, Xhosa, Sesotho, +5 | General | [OpenSLR](https://www.openslr.org/resources.php) |
| **Masakhane ASR** | Pan-African (20+ langs) | Various | [GitHub](https://github.com/masakhane-io/masakhane-asr) |
| **Niger-Volta LT** | Yoruba, Hausa, Igbo | Mixed | [GitHub](https://github.com/Niger-Volta-LTI) |
| **ALFFA** | Amharic, Hausa, Swahili, Wolof | Broadcast | [GitHub](https://github.com/besacier/ALFFA_PUBLIC) |

### Language-Specific Resources

#### Zimbabwe
- **Shona**: Badrex, Common Voice
- **Ndebele**: Common Voice (limited)

#### Tanzania
- **Swahili**: Common Voice, FLEURS, OpenSLR

#### South Africa
- **Zulu**: NCHLT, OpenSLR
- **Xhosa**: NCHLT, OpenSLR
- **Afrikaans**: NCHLT, Common Voice

#### Nigeria
- **Yoruba**: Common Voice, Niger-Volta
- **Igbo**: Common Voice, Niger-Volta
- **Hausa**: ALFFA, OpenSLR

---

## Dataset Statistics Summary

| Region | Languages Covered | Total Hours | Datasets |
|--------|-------------------|-------------|----------|
| Southern Africa | 8+ | 100+ hrs | 12 |
| East Africa | 6+ | 80+ hrs | 9 |
| West Africa | 10+ | 120+ hrs | 15 |
| North Africa | 4+ | 40+ hrs | 6 |

---

## Upcoming Additions

- [ ] Curated Shona tone-marked corpus
- [ ] Ndebele conversational dataset
- [ ] Code-switched speech data
- [ ] Low-resource language recordings
- [ ] Dialect-specific collections

---

## Contributing New Datasets

Have a dataset to share? Please:

1. Open an issue with tag `dataset-submission`
2. Provide dataset details (see template)
3. Ensure proper licensing
4. Include access instructions

---

## Dataset Quality Guidelines

We prioritize datasets with:

- Clear licensing (preferably open)
- Transcription accuracy > 95%
- Diverse speakers (age, gender, region)
- Metadata documentation
- Audio quality >= 16kHz sampling rate

---

## Citation

When using these datasets, please cite both:
1. The original dataset creators
2. This catalog (if helpful)

```bibtex
@misc{voxafrica_catalog2025,
  title={voxAfrica African Speech Datasets Catalog},
  author={{SeViVI-Tese AI Research}},
  year={2025},
  url={https://github.com/SeViVI-Tese/voxAfrica}
}
```

---

**Last Updated:** 2025-11-13  
**Maintainers:** SeViVI-Tese AI Research Team
