Official code for the paper ["A Little Pretraining Goes a Long Way: A Case Study on Dependency Parsing Task for Low-resource Morphologically Rich Languages"](https://arxiv.org/abs/2102.06551).
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
@misc{sandhan2021little,
      title={A Little Pretraining Goes a Long Way: A Case Study on Dependency Parsing Task for Low-resource Morphologically Rich Languages}, 
      author={Jivnesh Sandhan and Amrith Krishna and Ashim Gupta and Laxmidhar Behera and Pawan Goyal},
      year={2021},
      eprint={2102.06551},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

## Acknowledgements
Much of the base code is from ["DCST Implementation"](https://github.com/rotmanguy/DCST)
