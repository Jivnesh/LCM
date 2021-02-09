Official code for the paper ["A Little Pretraining Goes a Long Way: A Case Study on Dependency Parsing Task for Low-resource Morphologically Rich Languages"]().
If you use this code please cite our paper.

## Requirements

* Python 3.7 
* Pytorch 1.1.0 
* Cuda 9.0 
* Gensim 3.8.1

We assume that you have installed conda beforehand. 

```
conda install pytorch==1.1.0 torchvision==0.3.0 cudatoolkit=9.0 -c pytorch
pip install gensim==3.8.1
```
## Data
* Pretrained FastText embeddings for Sanskrit can be obtained from [here](https://drive.google.com/drive/folders/1JJMBjUZdqUY7WLYefBbA2zKaMHH3Mm18?usp=sharing). Make sure that `.vec` file is placed at approprite position.
* For Multilingual experiments, we use [UD treebanks](https://universaldependencies.org/) and [Pretrained FastText embeddings](https://fasttext.cc/docs/en/crawl-vectors.html)


## How to train model
If you want to run complete model pipeline: (1) Pretraining (2) Integration, then simply run bash script `run_san_LCM.sh`.

```bash
bash run_san_LCM.sh

```


## Citation

If you use our tool, we'd appreciate if you cite the following paper:

```
@inproceedings{sandhan-etal-2021-little,
    title = "A Little Pretraining Goes a Long Way: A Case Study on Dependency Parsing Task for Low-resource Morphologically Rich Languages",
    author = "Sandhan, Jivnesh and Krishna, Amrith and Gupta, Ashim and Behera, Laxmidhar and Goyal, Pawan", 
    booktitle = "Proceedings of the Student Research Workshop at the 16th Conference of the {E}uropean Chapter of the Association for Computational Linguistics",
    month = apr,
    year = "2021",
    address = "Kyiv, Ukraine",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/",
    pages = "--",
    abstract = "Neural dependency parsing has achieved remarkable performance for many domains and languages. The bottleneck of massive labeled data limits the effectiveness of these approaches for low resource languages. In this work, we focus on dependency parsing for morphological rich languages (MRLs) in a low-resource setting. Although morphological information is essential for the dependency parsing task, the morphological disambiguation and lack of powerful analyzers pose challenges to get this information for MRLs. To address these challenges, we propose simple auxiliary tasks for pretraining. We perform experiments on 10 MRLs in low-resource settings to measure the efficacy of our proposed pretraining method and observe an average absolute gain of 2 points (UAS) and 3.6 points (LAS).",
}
```

## Acknowledgements
Much of the base code is from ["DCST Implementation"](https://github.com/rotmanguy/DCST)
