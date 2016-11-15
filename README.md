# Multi-class GAN

### Citation
If you use this work in your research, please cite:

    @article{Mao2016,
      author = {Xudong Mao, Qing Li, Haoran Xie, Raymond Y.K. Lau and Zhen Wang},
      title = {Multi-class Generative Adversarial Networks with the L2 Loss Function},
      journal = {arXiv preprint arXiv:1611.04076},
      year = {2016}
    }

### Prerequisites
- Tensorflow
- SciPy

### Usage
1.Download datasets

  - [HWDB1.0 (Handwritten Chinese characters)](http://www.nlpr.ia.ac.cn/databases/handwriting/Download.html)
  - [LSUN-bedroom](http://lsun.cs.princeton.edu/2016/)

2.Convert data

```
  $ python convert_icdar.py --source_dir $SOURCE_PATH --target_dir $TARGET_PATH
  $ python convert_lsun.py --source_dir $SOURCE_PATH --target_dir $TARGET_PATH
```

3.Train model

```
  $ python train_chn.py --data_dir $DATA_DIR
  $ python train_lsun.py --data_path $DATA_PATH
```
