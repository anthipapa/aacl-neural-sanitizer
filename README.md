Code associated with the following citation can be found [here](https://github.com/NorskRegnesentral/NeuralTextSanitizer).

A novel approach for text sanitization, which is the task of editing a document to mask all (direct and indirect) personal identifiers and thereby conceal the identity of the individuals(s) mentioned in the text. The approach proceeds in three steps:
1. A neural, privacy-enhanced entity recognizer is first employed to detect and classify potential personal identifiers
2. We then determine which entities, or combination of entities, are likely to pose a re-identification risk through a range of privacy risk assessment measures
   - span probabilities derived from a BERT language model
   - web search queries
   - a classifier trained on labelled data
3. Finally, a linear optimization solver decides which entities to mask to minimize the semantic loss while simultaneously ensuring that the estimated privacy risk remains under a given threshold

## Citation

Anthi Papadopoulou, Yunhao Yu, Pierre Lison, and Lilja Øvrelid. 2022. "[Neural Text Sanitization with Explicit Measures of Privacy Risk](https://aclanthology.org/2022.aacl-main.18/)". *In Proceedings of the 2nd Conference of the Asia-Pacific Chapter of the Association for Computational Linguistics and the 12th International Joint Conference on Natural Language Processing (Volume 1: Long Papers), pages 217–229, Online only. Association for Computational Linguistics.*

```bibtex
@inproceedings{papadopoulou-etal-2022-neural,
    title = "Neural Text Sanitization with Explicit Measures of Privacy Risk",
    author = "Papadopoulou, Anthi  and
      Yu, Yunhao  and
      Lison, Pierre  and
      {\O}vrelid, Lilja",
    booktitle = "Proceedings of the 2nd Conference of the Asia-Pacific Chapter of the Association for Computational Linguistics and the 12th International Joint Conference on Natural Language Processing (Volume 1: Long Papers)",
    month = nov,
    year = "2022",
    address = "Online only",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.aacl-main.18",
    pages = "217--229",
    abstract = "We present a novel approach for text sanitization, which is the task of editing a document to mask all (direct and indirect) personal identifiers and thereby conceal the identity of the individuals(s) mentioned in the text. In contrast to previous work, the approach relies on explicit measures of privacy risk, making it possible to explicitly control the trade-off between privacy protection and data utility. The approach proceeds in three steps. A neural, privacy-enhanced entity recognizer is first employed to detect and classify potential personal identifiers. We then determine which entities, or combination of entities, are likely to pose a re-identification risk through a range of privacy risk assessment measures. We present three such measures of privacy risk, respectively based on (1) span probabilities derived from a BERT language model, (2) web search queries and (3) a classifier trained on labelled data. Finally, a linear optimization solver decides which entities to mask to minimize the semantic loss while simultaneously ensuring that the estimated privacy risk remains under a given threshold. We evaluate the approach both in the absence and presence of manually annotated data. Our results highlight the potential of the approach, as well as issues specific types of personal data can introduce to the process.",
}
```
