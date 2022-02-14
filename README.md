# Group Project

Supervisor: 郑锋

Team members: 张一弛，杨英特

## Visual Question Answering

VQA is a new dataset containing open-ended questions about images. These questions require an understanding of vision, language and commonsense knowledge to answer

VQA: https://visualqa.org/

## DataSet

#### Download

链接：https://pan.baidu.com/s/1xdo60gx-lIaohkfe-Vfhww 

提取码：stds

#### Introduction

image: image.rar

QA-pair: FM_IQA.json

VGG16: vgg16-20160129.tfmodel

Model of our train: model199.ckpt in Models

## Pretrain, Train and Test

```sh
python data_loader.py
python extract_fc7.py --model_path 'Data/vgg16-20160129.tfmodel' --data_dir 'Data'
python train.py --data_dir 'Data'
python predict.py --model_path 'Data/Models/model199.ckpt' --image_path 'cat.jpeg' --question '这只动物是什么'
```

## Version

#### environment

Python == 3.6.13

cuda == 10.1

#### package

astor == 0.8.1

h5py == 3.1.0

html5lib == 0.9999999

imageio == 2.12.0

jieba == 0.42.1

keras == 2.6.0

numpy == 1.19.5

requests == 2.26.0

scipy == 1.5.4

six == 1.15.0

tensorflow == 1.6.0

tensorflow-gpu == 1.14.0

## report

Report of the DataSet.docx

Report of the VQA Model and Train.docx

## demonstration

PPT of the DataSet.pptx

PPT of the VQA Model and Train.pptx

