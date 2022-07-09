Annotations for the Meta-Evaluation of Machine Translation Research
=============

The annotations are available [here](https://docs.google.com/spreadsheets/d/1l9OL1HbUfZ6woawTAapqe-ASEn2DWw8FB64o1NO-K_U).

**Last update July 9th 2022**: 2021 *ACL conferences + various charts added.  


The original version published at ACL 2021 is still available [here](https://docs.google.com/spreadsheets/d/1C4kYnnKbIn2U_zEWsLGkReUzb-HqGxN4cQqje4uojmE).

These annotations were used to conduct a meta-evaluation of machine translation publications published from 2010 to 2020 at conferences organized by the ACL. The analysis of this meta-evaluation, including pitfalls and concerning trends, is presented in the following publication: "Scientific Credibility of Machine Translation Research: A Meta-Evaluation of 769 Papers" by Benjamin Marie, Atsushi Fujita, and Raphael Rubino (ACL2021).

The annotations will be updated to include upcoming conferences and keep track of the evolution of the machine translation evaluation.


Guideline for Machine Translation Evaluation
=============
Given the pitfalls and concerning trends observed in our annotations, we propose the following guideline for machine translation (MT) papers that rely on automatic metric scores for evaluating translation quality.

 * An MT evaluation may not exclusively rely on BLEU. Other automatic metrics that better correlate with human judgments, or a human evaluation, may be used in addition or in lieu of BLEU.
* Statistical significance testing may be performed on automatic metric scores to ensure that the difference between two scores, whatever its amplitude, is not coincidental.
* Automatic metric scores copied from previous work may not be compared. If inevitable, copied scores may only be compared with scores computed in exactly the same way, through tools guaranteeing this comparability, while providing all the necessary information to reproduce them.  
* Comparisons between MT systems through their metric scores may be performed to demonstrate the superiority of a method or an algorithm only if the systems have been trained, validated, and tested with exactly the same pre-processed data, unless the proposed method or algorithm is indeed dependent on a particular dataset or pre-processing. 

Following this guideline is as simple as writing the following text in your paper:

*For evaluation, we use BLEU (Papineni et al., 2002) and chrF (Popović, 2015) computed with SacreBLEU (Post, 2018). We perform statistical significance testing using bootstrap resampling (Koehn, 2004). All the MT systems compared in this paper are trained, validated and tested on the exact same pre-processed data.*

It does not mean that the evaluation is perfect but that it is more credible than almost all the MT evaluations performed in previous work and give it the maximum meta-evaluation score of 4 (see the following section). However, note that it does not fully apply to a paper proposing new datasets and/or pre-processing methods for MT.
In this example, *chrF* and *bootstrap resampling* are only examples: other and better metrics and statistical significance testing methods may be used.

Meta-Evaluation Score
=============
The purpose of the following scoring method is to assess the trustworthiness of an automatic evaluation performed in a machine translation paper. Ultimately, it can be used for authors' self-assessment or by machine translation program committees to identify trustworthy papers.

Each "yes" answer to the following questions brings 1 point to the paper for a maximum of 4 points.

* Is a metric that better correlates with human judgment than BLEU used or is a human evaluation performed? 
* Is statistical significance testing performed?
* Are the automatic metric scores computed for the paper and not copied from other work?
  * If copied, are all the copied and compared scores computed through tools that guarantee their comparability (e.g., SacreBLEU)?
* If comparisons between machine translation systems are performed to demonstrate the superiority of a method or an algorithm that is independent from the datasets exploited and their pre-processing, are all the compared machine translation systems exploiting exactly the same pre-processed data for training, validating, and testing? (if not applicable, give 1 point by default)



Paper
-----
Bibtex:
```
@inproceedings{marie21ACL,
  author={Marie, Benjamin and Fujita, Atsushi and Rubino, Raphael},
  title={Scientific Credibility of Machine Translation Research: A Meta-Evaluation of 769 Papers},
  year={2021},
  booktitle={Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics}
}
```

Contact
---
For questions, please contact the first author of the paper. 

License
---

![Creative Commons License](http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)

Use and/or redistribution of this dataset is permitted under the conditions of [Creative Commons Attribution-NonCommercial-ShareAlike License 4.0](http://creativecommons.org/licenses/by-nc-sa/4.0/>).
