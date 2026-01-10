# From Foreignization to Domestication: Quantifying Syntactic Shift in Beowulf Translations

## Project Overview
This project investigates the evolution of English syntax and translation strategy by analyzing *Beowulf* translations. As English evolved from a synthetic to an analytic language, reliance on fixed SVO word order replaced inflectional morphology. This study quantifies how translation practices have shifted regarding sentence structure and the preservation of historical linguistic features.

Theoretical frameworks by **John D. Niles** suggest that translation oscillates between two poles: "foreignization" (bringing the reader to the text via archaic words) and "domestication" (bringing the text to the reader via fully idiomatic current English). This project uses computational stylometry to measure the translator's "bias" or "spin" regarding these poles.

## Research Question
How do word order (SVO frequency) and dependency parsing accuracy (LAS) vary between translations of *Beowulf* published pre-1900 and post-1900?

## Dataset
The analysis focuses on two verse translations of *Beowulf* retrieved from Project Gutenberg:
*   **Pre-1900:** William Morris and A.J. Wyatt (1895)
*   **Post-1900:** Francis B. Gummere (1909)

To ensure comparability, a parallel sample of "The Watchman’s Challenge" was extracted:
*   Morris: lines 230-300
*   Gummere: lines 229-300

## Methodology
The texts were segmented into sentences to address boundary detection issues common in historical texts. The study utilizes Universal Dependencies to measure "parseability" as a metric for modernity, based on findings by **Martín Arista et al. (2025)** that neural parsers achieve lower accuracy on Old English compared to Modern English.

### Variables
*   **Independent Variable:** Translation Era (Pre-1900 vs. Post-1900)
*   **Dependent Variable 1:** Parseability (LAS Score).
*   **Dependent Variable 2:** Pronominal Usage (Ratio of archaic pronouns).

## Hypotheses
1.  **Morris (1895):** Will exhibit low parseability (LAS scores < 60%) and frequent non-SVO structures. This aligns with the "foreignization" approach, where the syntax attempts to mimic the flexible word order of the source language, often resulting in text deemed "nearly unreadable".
2.  **Gummere (1909):** Will exhibit higher SVO frequency and parseability (LAS 60-80%). While Gummere argued for preserving the "original Anglo-Saxon meter" and its peculiarities, his work represents a "conscientious" middle ground that moves toward domestication and greater narrative flow compared to Morris.

## References

*   Chickering, H. (2002). "Beowulf and 'Heaneywulf'". *The Kenyon Review* 24(1), 160–178.
*   Crane, J. K. (1970). "To Thwack or Be Thwacked: An Evaluation of Available Translations and Editions of Beowulf." *College English* 32(3), 321–340.
*   Gummere, F. B. (1886). "The Translation of Beowulf, and the Relations of Ancient and Modern English Verse." *The American Journal of Philology* 7(1), 46–78.
*   Ingham, R. (2000). "Negation and OV Order in Late Middle English." *Journal of Linguistics* 36(1), 13–38.
*   Martín Arista, J., et al. (2025). "Parsing Old English with Universal Dependencies—The Impacts of Model Architectures and Dataset Sizes." *Big Data and Cognitive Computing* 9(8), 199.
*   Niles, J. D. (1993). "Rewriting Beowulf: The Task of Translation." *College English* 55(8), 858–878.
*   West, F. (1973). "Some Notes on Word Order in Old and Middle English." *Modern Philology* 71(1), 48–53.
*   Yao, X., et al. (2025). "Missing the human touch? A computational stylometry analysis of GPT-4 translations..." *Translation Spaces* 14(2), 303–330.

## Reproducibility
The full code and preprocessed datasets used in this study are available in this repository.
