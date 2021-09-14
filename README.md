# CoTexT
Code implementation for [CoTexT: Multi-task Learning with Code-Text Transformer](https://arxiv.org/abs/2105.08645)

# Google Cloud Storage 

Our base Google Cloud Storage URI is at [gs://scifive]()


As described in our [paper](https://arxiv.org/abs/2105.08645), we make public 3 version of CoTexT, each one has been benchmarked to achieve state-of-the-art on different code - natural language generation task. They are all available on our [Google Cloud bucket](https://console.cloud.google.com/storage/browser/cotext), we are working on release the models on HuggingFace also.

Instruction on access Cloud Storage from the command line with python library gsutil is described [here](https://cloud.google.com/storage/docs/gsutil)

### gsutil URI for pre-trained data:

* **CodeSearchNet**: [gs://cotext/data/pretrain]() 
* **Github Repos**: [gs://cotext/data/github_repos/sample_content/cleaned]() 



### gsutil URI for 3 CoTexT models:

Description of each model is descriped in our [paper](https://arxiv.org/abs/2105.08645)

* **CoTexT 1-CC**: [gs://cotext/cc_pl]() 
* **CoTexT 2-CC**: [gs://cotext/cc]() 
* **CoTexT 1-CCG**: [gs://cotext/ccg]() 




## Citations
If you use CoTexT model or our code for publications, please cite: 
```
@inproceedings{phan-etal-2021-cotext,
    title = "{C}o{T}ex{T}: Multi-task Learning with Code-Text Transformer",
    author = "Phan, Long  and
      Tran, Hieu  and
      Le, Daniel  and
      Nguyen, Hieu  and
      Annibal, James  and
      Peltekian, Alec  and
      Ye, Yanfang",
    booktitle = "Proceedings of the 1st Workshop on Natural Language Processing for Programming (NLP4Prog 2021)",
    month = aug,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2021.nlp4prog-1.5",
    doi = "10.18653/v1/2021.nlp4prog-1.5",
    pages = "40--47",
    abstract = "We present CoTexT, a pre-trained, transformer-based encoder-decoder model that learns the representative context between natural language (NL) and programming language (PL). Using self-supervision, CoTexT is pre-trained on large programming language corpora to learn a general understanding of language and code. CoTexT supports downstream NL-PL tasks such as code summarizing/documentation, code generation, defect detection, and code debugging. We train CoTexT on different combinations of available PL corpus including both {``}bimodal{''} and {``}unimodal{''} data. Here, bimodal data is the combination of text and corresponding code snippets, whereas unimodal data is merely code snippets. We first evaluate CoTexT with multi-task learning: we perform Code Summarization on 6 different programming languages and Code Refinement on both small and medium size featured in the CodeXGLUE dataset. We further conduct extensive experiments to investigate CoTexT on other tasks within the CodeXGlue dataset, including Code Generation and Defect Detection. We consistently achieve SOTA results in these tasks, demonstrating the versatility of our models.",
}

```

