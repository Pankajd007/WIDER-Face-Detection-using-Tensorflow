# WIDER-Face-Detection-using-Tensorflow
## Introduction


In this notebook, we implement [The TensorFlow 2 Object Detection Library](https://blog.tensorflow.org/2020/07/tensorflow-2-meets-object-detection-api.html) for training on our own dataset.



We will take the following steps to implement EfficientDet D0 on our custom data:
* Install TensorFlow2 Object Detection Dependencies
* Download Custom TensorFlow2 Object Detection Dataset
* Write Custom TensorFlow2 Object Detection Training Configuation
* Train Custom TensorFlow2 Object Detection Model
* Export Custom TensorFlow2 Object Detection Weights
* Use Trained TensorFlow2 Object Detection For Inference on Test Images



## Install TensorFlow2 Object Detection Dependencies
```
  !git clone --depth 1 https://github.com/tensorflow/models
  ```

## Install the Object Detection API
```
%%bash
cd models/research/
protoc object_detection/protos/*.proto --python_out=.
cp object_detection/packages/tf2/setup.py .
python -m pip install .
```
``
## run model builder test
!python model_builder_tf2_test.py
``



## Reslut
![download](https://user-images.githubusercontent.com/57318222/115399440-d8287b80-a205-11eb-8719-35d2db66ee53.png)

