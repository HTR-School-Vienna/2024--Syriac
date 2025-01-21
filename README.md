# 2024-Syriac

Ground truth of 140 folios of ÖNB Cod. Syr. 1. This ground truth was produced by participants of the Vienna 2024 HTR Winter School, who used Transkribus to manually correct a preliminary automatic transcription that had been generated using Kraken.

**ATTENTION**: To clone this repo you need to have [Git LFS](https://git-lfs.com/) installed and then clone the repository like this:

```
git lfs clone git@github.com:htr-school-vienna/[your_repository_name].git https://github.com/HTR-School-Vienna/2023--carolingian-latin
```

<!-- Continue editing here -->

## Description

- Vienna, Austrian National Library, MS ÖNB Cod. Syr. 1
- Syriac, Serto, 16th century
- Codex dated 1545 AD, scribed by Moses of Mardin in Vienna

### Origin of the data

Source of the images: Österreichische Nationalbibliothek, https://digital.onb.ac.at/RepViewer/viewer.faces?doc=DTL_2933415.

### Segmentation and Transcription guidelines

The segmentation of the folios followed the [SegmOnto](https://segmonto.github.io/) vocabulary for annotation of regions: 

- `MainZone`: the main column of text.
- `MainZone-gold`: any sections of the main column where the text is written in gold block characters, as in the start of the text [here](https://digital.onb.ac.at/RepViewer/viewer.faces?doc=DTL_2933415&order=16). (The `-` character is a substitution for SegmOnto's recommended `:` character for declaring subtypes, since Transkribus did not allow for use of the colon character in the region name.)
- `MarginTextZone`: any marginal words or phrases, including catchwords. Also used for interlinear glosses.
- `NumberingZone`: any page or folio numbers.

The transcription includes spaces, the Syriac letters, some diacritics, punctuation, and no vowel dots or markings.

- Allowed diacritics:
  - Syome
  - Dots over feminine suffix heh
  - Dots in pronouns: above for demonstrative, below for personal
  - Dots in verbs: to distinguish participles and perfects
  - Dots to distinguish homographs
- Excluded diacritics:
  - Vowel dots
  - Dots of hardening and softening (qushoyo and rukokho)
 
Punctuation marks were not normalized, but rather transcribed as they appear in the manuscript (. ܆ ܇ : ܀).

Transkribus's `unclear` tag was used when readings were uncertain or the text was damaged or unclear.

### Data organisation

- `ÖNB_Syr_1`
  - `page`: the XML ground truth
  - `images`: the corresponding image files

## How to cite

This dataset was created by: Ephrem Aboud Ishac, Christine Roughan, Ammar Awad, Carlo Biuzzi Emilio, Saranya Chandran, Jennifer Griggs, Polina Ivanova, Branko Malešević, Stefan Marić, Francesca Nateri, Ivan Petrov, Cristina Tava, and Maria S. Thomas. If you use any item from this corpus as ground truth, cite the dataset using the following information:

```
<!-- Copy citation BibTeX from Zenodo 10.5281/zenodo.10589561 -->
```

## Copyright and licence
This dataset was created as part of the Winter School of Handwritten Text Recognition of Medieval Manuscripts 2024, Vienna at the Österreichische Akademie der Wissenschaften, Institut für Mittelalterforschung, all transcriptions are licensed under the Creative Commons 4 licence. Images were provided by the Austrian National Library (ÖNB) and are licensed under Creative Commons 4 licence.
