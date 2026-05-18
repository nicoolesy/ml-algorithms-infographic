# A Visual Field Guide to Machine Learning
This repository hosts an infographic that classifies ten foundational machine learning algorithms by **learning paradigm** (supervised vs. unsupervised), **application domain** (tabular, computer vision, NLP, generative AI), and **historical lineage**.

🔗 **Live infographic:** [View it here](https://nicoolesy.github.io/ml-algorithms-infographic/index.html)


## The Ten Algorithms
 
| # | Algorithm | Paradigm | Domain(s) |
|---|-----------|----------|-----------|
| 01 | Linear Regression | Supervised | Tabular |
| 02 | Logistic Regression | Supervised | Tabular |
| 03 | Decision Trees | Supervised | Tabular |
| 04 | Random Forest | Supervised | Tabular |
| 05 | Support Vector Machines | Supervised | Tabular, CV |
| 06 | Convolutional Neural Networks | Supervised | Computer Vision |
| 07 | Transformers | Supervised | NLP, Generative AI |
| 08 | K-Means Clustering | Unsupervised | Tabular |
| 09 | Principal Component Analysis | Unsupervised | Tabular |
| 10 | Generative Adversarial Networks | Unsupervised | CV, Generative AI |

## Explanation of the Classification Process
 
I organized this framework along **three axes** because no single dimension captures how these algorithms actually relate to one another in practice.
 
### Axis 1 — Learning Paradigm (Supervised vs. Unsupervised)
 
The first split is the most fundamental in ML: **does the algorithm learn from labeled examples or not?**
 
- **Supervised algorithms** receive `(input, correct output)` pairs and learn to map one to the other. I placed Linear Regression, Logistic Regression, Decision Trees, Random Forest, SVM, CNNs, and Transformers here because each requires labeled training data — predicted prices, class labels, or next tokens.
- **Unsupervised algorithms** are given only inputs and must find structure on their own. K-Means, PCA, and GANs all operate without explicit labels — they cluster, compress, or generate based on the data's intrinsic distribution.
> **Note on GANs (Generative Adversarial Networks):** Some practitioners classify GANs as *self-supervised* because the discriminator generates its own training signal. I classified them as unsupervised because the underlying dataset lacks human-provided labels — the network generates its own supervisory signal internally.

### Axis 2 — Application Domain
 
The second axis maps each algorithm to the data types it natively handles well. An algorithm can appear in multiple domains:
 
- **Tabular** — rows-and-columns data (spreadsheets, databases). Most classical algorithms live here.
- **Computer Vision** — pixel data. CNNs are purpose-built for this; SVMs and GANs also operate here.
- **NLP** — sequences of words/tokens. Transformers dominate this domain today.
- **Generative AI** — algorithms that *create* new content rather than just classifying or predicting. Both Transformers (text/code) and GANs (images) qualify.
I assigned an algorithm to a domain if it's *commonly and effectively* used there in production — not every theoretically possible application.
 
### Axis 3 — Historical Lineage (the "Eras" section)
 
Reading left-to-right in the lineage diagram, the algorithms trace a clear progression:
 
1. **Era 1 — Statistical Foundations.** Interpretable, math-driven models (LR, LogReg, Decision Trees, K-Means, PCA, SVM). These still dominate tabular problems today.
2. **Era 2 — Ensembles & Deep Learning.** Random Forest showed that combining weak learners beats tuning one strong one. CNNs, enabled by GPUs and ImageNet, transformed computer vision around 2012.
3. **Era 3 — The Generative Turn.** GANs (2014) and Transformers (2017) shifted ML from *describing* data to *creating* it — the foundation of the current generative AI moment.
This lineage axis matters because it shows the algorithms aren't isolated; each generation built on the last.

## File Structure
 
```
.
├── index.html      # The infographic (open in browser or via GitHub Pages)
└── README.md       # This file
```
---

## AI Use Disclosure
 
In accordance with academic integrity standards, I want to be transparent about how AI was used in creating this artifact:
 
- **Concept, classification decisions, and reflection:** Authored by me, drawing on my coursework and prior knowledge of machine learning.
- **Visual layout, HTML/CSS formatting, and writing polish:** Created with assistance from **Claude (Anthropic)**. I used Claude to help structure the infographic's visual design, refine the wording of explanations, and produce clean, accessible HTML for hosting on GitHub Pages.
- **Final review and editorial decisions:** All content was reviewed, edited, and approved by me. I take responsibility for the accuracy of every classification and claim made in this artifact.
This use of AI is consistent with how professionals in the field increasingly use these tools — as collaborators for drafting, formatting, and polish — while the substantive thinking and final judgment remain my own.


## Author
 
[Nicole Chen] · Indiana Wesleyan University
