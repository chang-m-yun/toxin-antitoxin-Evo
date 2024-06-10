# CS273B_TA_Evo
CS273B Final Project: Designing de novo bacterial toxin-antitoxins uisng a generative genomic foundation model

Authors: Aditi Merchant, Santiago Mille-Fragoso, Samuel King, Chang M. Yun
Stanford University
CS273B Deep Learning in Genomics and Biomedicine, Spring 2024

## 1. Preprocessing
* Data from TADB 3.0 (https://bioinfo-mml.sjtu.edu.cn/TADB3/browse_tax.php)

## 2. Finetuning
* Base model: Evo (https://github.com/evo-design/evo)
* Finetuning: LoRA (https://github.com/microsoft/LoRA)

## 3. Prompting
* Base model: Evo (https://github.com/evo-design/evo)

## 4. Evaluation
* Filter 1: Multiple sequence alignment
* Filter 2: Profile Hidden Markov Model (pHMM)
* Filter 3: Basic Local Alignment Search Tool: Protein (BLASTp)
* Protein structure: ESMFold (https://github.com/facebookresearch/esm)
