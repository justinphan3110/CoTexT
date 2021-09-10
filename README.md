# CoTexT
Code implementation for [CoTexT: Multi-task Learning with Code-Text Transformer](https://arxiv.org/abs/2105.08645)

# Google Cloud Storage 

Our base Google Cloud Storage URI is at [gs://scifive]()


As described in our [paper](https://arxiv.org/abs/2105.08645), we make public 3 version of CoTexT, each one has been benchmarked to achieve state-of-the-art on different code - natural language generation task. They are all available on our [Google Cloud bucket](https://console.cloud.google.com/storage/browser/cotext), we are working on release the models on HuggingFace also.

Instruction on access Cloud Storage from the command line with python library gsutil is described [here](https://cloud.google.com/storage/docs/gsutil)

### gsutil URI for 6 SciFive models:

Description of each model is descriped in our [paper](https://arxiv.org/abs/2105.08645)

* **CoTexT 1-CC**: [gs://cotext/cc_pl]() 
* **CoTexT 2-CC**: [gs://cotext/cc]() 
* **CoTexT 1-CCG**: [gs://cotext/ccg]() 




## Citations
If you use CoTexT model or our code for publications, please cite: 
```
@article{DBLP:journals/corr/abs-2105-08645,
  author    = {Long Phan and
               Hieu Tran and
               Daniel Le and
               Hieu Nguyen and
               James Anibal and
               Alec Peltekian and
               Yanfang Ye},
  title     = {CoTexT: Multi-task Learning with Code-Text Transformer},
  journal   = {CoRR},
  volume    = {abs/2105.08645},
  year      = {2021},
  url       = {https://arxiv.org/abs/2105.08645},
  archivePrefix = {arXiv},
  eprint    = {2105.08645},
  timestamp = {Mon, 31 May 2021 16:16:57 +0200},
  biburl    = {https://dblp.org/rec/journals/corr/abs-2105-08645.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

