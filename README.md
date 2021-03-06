# Efficient-Det
物体検出モデルefficient-detを改良したもの

# install requirements
```
python
pip install pycocotools numpy opencv-python tqdm tensorboard tensorboardX pyyaml webcolors
pip install torch==1.4.0
pip install torchvision==0.5.0
```
 
# run the simple inference script
```python
python efficientdet_test.py
```

# datasets
Efficient-det-dataset　に用意する。　　
train-valにデータを分ける方法はフォルダ内のRead Meファイルに記載されている。

# your dataset structure should be like this
```python
datasets/
    -your_project_name/
        -train_set_name/
            -*.jpg
        -val_set_name/
            -*.jpg
        -annotations
            -instances_{train_set_name}.json
            -instances_{val_set_name}.json
```

# for example, coco2017
```python
datasets/
    -coco2017/
        -train2017/
            -000000000001.jpg
            -000000000002.jpg
            -000000000003.jpg
        -val2017/
            -000000000004.jpg
            -000000000005.jpg
            -000000000006.jpg
        -annotations
            -instances_train2017.json
            -instances_val2017.json
```
## 参照
https://github.com/zylo117/Yet-Another-EfficientDet-Pytorch
