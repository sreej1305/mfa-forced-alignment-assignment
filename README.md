# mfa-forced-alignment-assignment
Forced alignment using Montreal Forced Aligner (MFA)
Assignment 1: Forced Alignment using Montreal Forced Aligner (MFA)

Objective
To set up and execute a forced alignment pipeline using Montreal Forced Aligner (MFA) and analyze word and phoneme alignment between speech audio and text transcripts.
---
Tools Used
- Montreal Forced Aligner (MFA) v3.3.9
- Praat
- Ubuntu (WSL on Windows)
---
Dataset Structure

data/
├── wav/ # Audio files (.wav)
└── transcripts/ # Corresponding transcripts (.txt)
Each transcript file corresponds to one audio file with the same filename.

---

Installation
MFA was installed using micromamba.

```bash
micromamba create -n mfa -c conda-forge montreal-forced-aligner
micromamba activate mfa
Running Forced Alignment
The following command was used:
mfa align data english_us_arpa english_us_arpa output
Acoustic model: english_us_arpa
Dictionary: english_us_arpa

Output
The alignment results are stored in the output/ directory as Praat TextGrid files.
These TextGrid files contain:
Word-level alignment
Phoneme-level alignment

Analysis
The TextGrid files were inspected using Praat.
Screenshots showing word and phoneme boundaries are provided in the screenshots/ folder.

Observations include:
Correct alignment for most words and phonemes
Minor timing offsets in some phoneme boundaries
No major alignment failures observed

Conclusion
This assignment demonstrates successful forced alignment using MFA and analysis using Praat.
