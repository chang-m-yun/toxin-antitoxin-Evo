# CS273B_TA_Evo
Designing _de novo_ bacterial toxin-antitoxins using a generative genomic foundation model

**Authors**: Aditi Merchant<sup>1</sup>, Santiago Mille-Fragoso<sup>1</sup>, Samuel King<sup>1</sup>, Chang M. Yun<sup>2</sup> \
<sup>1</sup>Department of Bioengineering, Stanford University, <sup>2</sup>Department of Chemical Engineering, Stanford University

For CS273B Deep Learning in Genomics and Biomedicine, Spring 2024

## Abstract
Toxin-antitoxin (TA) systems are natural kill switches in bacteria that consist of a toxin that inhibits an essential cellular process, and a corresponding antitoxin that counteracts it. TAs are important for bacterial adaptation, persistence, and defense, and have great potential in bioengineering and therapeutic applications, such as for antimicrobials, novel selection markers, and biocontainment. The recent development of genomic large language models (LLMs) promises to enable the generative design of novel TA systems to expand the current toolbox available. Here, we use Evo, a genomic foundation model capable of multi-element generation tasks, to generate _de novo_ TAs by zero-shot prompting and after fine-tuning. We validate the viability of the new TA designs using multiple _in silico_ metrics, including sequence homology and protein structure and interaction prediction, and show that our designs are likely confident candidates ready for experimental validation. Overall, this study demonstrates the first genomic LLM-based design pipeline for TAs and establishes a set of confidence metrics for similar future work.

![Figure: Strategy for de novo design of Type II toxin-antitoxins using a genomic foundation model](/docs/figure_1.png)

**Figure: Strategy for de novo design of Type II toxin-antitoxins using a genomic foundation model.** (a) Mechanism of Type II toxin-antitoxins. (b) High-level overview of the strategy for designing novel Type II toxin-antitoxins to expand the existing repertoire.

## 1. Preprocessing
* Data from TADB 3.0 (https://bioinfo-mml.sjtu.edu.cn/TADB3/browse_tax.php)

## 2. Finetuning
* Base model: Evo (https://github.com/evo-design/evo)
* Finetuning: LoRA (https://github.com/microsoft/LoRA)

## 3-I. Prompting
* Base model: Evo (https://github.com/evo-design/evo)

## 3-II. Evaluation
* Filter 1: Multiple sequence alignment
* Filter 2: Profile Hidden Markov Model (pHMM)
* Filter 3: Basic Local Alignment Search Tool: Protein (BLASTp)
* Protein structure: ESMFold (https://github.com/facebookresearch/esm)

## Acknowledgements
* CS273B Deep Learning in Genomics and Biomedicine, Spring 2024 \
* Laboratory of Evolutionary Design (https://github.com/evo-design) \
* Kundaje Lab (https://github.com/kundajelab) \
* Gao Lab (https://gaolab.bio/)
