# A Computational Study of Framing Evoked by Presuppositions

## 1. About

This repository contains source code of the paper:

*Qi Yu. 2022. "Again, Dozens of Refugees Drowned": A Computational Study of Political Framing Evoked by Presuppositions. In Proceedings of the 2022 Conference of the North American Chapter of the Association for Computational Linguistics (NAACL): Human Language Technologies: Student Research Workshop*

The paper analyzes a type of political framing strategy which is easy to be neglected, yet powerful: 
framing evoked by [presupposition-triggers](https://plato.stanford.edu/entries/presupposition/). 
Specifically, the usage of iterative adverbs (e.g., *again*) in three different German newspapers is investigated as a study case. 

## 2. Scripts and Model
All results reported in the paper are to be found in the ```.ipynb```-scripts. 

- ```1_finetune_BERT.ipynb```: Fine-tuning [bert-base-german-cased](https://huggingface.co/bert-base-german-cased) to vectorize sentences containing iterative adverbs (iterAdv-S).  
The fine-tuned model is to be found [here](https://drive.google.com/drive/folders/1R9Li24iU_QdV2-0Xm7F1QlXHVbZ1WXuK).
  
- ```2_analyze_iterAdv-S.ipynb```: Analyzing the topic preferences among *iterAdv-S* in different newspapers by 1) clustering the *iterAdv-S* 
  and 2) mining keywords in each cluster using the measure *PMI-freq* (Jin et al., 2020).

For more details, please refer to Section 4 of the paper.


## 3. Cite the Paper
```
@inproceedings{yu-2022-dozens,
    title = "{``}Again, Dozens of Refugees Drowned{''}: A Computational Study of Political Framing Evoked by Presuppositions",
    author = "Yu, Qi",
    booktitle = "Proceedings of the 2022 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies: Student Research Workshop",
    month = jul,
    year = "2022",
    address = "Hybrid: Seattle, Washington + Online",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.naacl-srw.5",
    pages = "31--43",
}
```

## 4. Acknowledgement
This project is funded by the Deutsche Forschungsgemeinschaft (DFG – German Research Foundation) under Germany‘s Excellence Strategy – EXC-2035/1 – 390681379.
