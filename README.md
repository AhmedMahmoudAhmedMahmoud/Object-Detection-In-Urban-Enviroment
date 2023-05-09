# Object-Detection-in-Urban-Enviroment-1

Train an object detection model using the Notebook Tensorflow Object Detection API and Colab.

## Classes:
Vehicles, Pedestrians, Cyclists

## Models:

1- EfficientDet D1 640x640 

pipline.config changes :

num_classes: 3

batch_size: 4

fine_tune_checkpoint_type: "detection"

fine_tune_checkpoint: "/content/gdrive/MyDrive/Project/customTF2/data/efficientdet_d1_coco17_tpu-32/checkpoint/ckpt-0"

train_input_reader: {

  label_map_path: "/content/gdrive/MyDrive/Project/customTF2/data/train/label_map.pbtxt"
  
  tf_record_input_reader {
  
    input_path: "/content/gdrive/MyDrive/Project/customTF2/data/train/*.tfrecord"
    
  }
  
eval_input_reader: {

  label_map_path: "/content/gdrive/MyDrive/Project/customTF2/data/val/label_map.pbtxt"
  
  shuffle: false
  
  num_epochs: 1
  
  tf_record_input_reader {
  
    input_path: "/content/gdrive/MyDrive/Project/customTF2/data/val/*.tfrecord"
    
  }
  
Loss
![Loss](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/be05f666-5d8b-4549-9b4f-387f38f40837)
Precision
![Prec](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/c07e586c-f3f7-4b57-b616-b57123ede1ba)
Recall
![Recall](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/518864d5-b683-4ffe-9056-b3e80710af2b)

Learning Rate
![Learning_Rate](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/47cae0a3-e47c-41a8-86f3-5e96e8b13c83)

![Efficientdet1](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/8a6d07c9-b3d1-4bd5-932e-52c1c3125b63)




2- SSD ResNet50 V1 FPN 640x640 (RetinaNet50)

pipline.config changes :

num_classes: 3

batch_size: 4

fine_tune_checkpoint_type: "detection"

fine_tune_checkpoint: "/content/gdrive/MyDrive/Project/customTF2/data/efficientdet_d1_coco17_tpu-32/checkpoint/ckpt-0"

train_input_reader: {

  label_map_path: "/content/gdrive/MyDrive/Project/customTF2/data/train/label_map.pbtxt"
  
  tf_record_input_reader {
  
    input_path: "/content/gdrive/MyDrive/Project/customTF2/data/train/*.tfrecord"
    
  }
  
eval_input_reader: {

  label_map_path: "/content/gdrive/MyDrive/Project/customTF2/data/val/label_map.pbtxt"
  
  shuffle: false
  
  num_epochs: 1
  
  tf_record_input_reader {
  
    input_path: "/content/gdrive/MyDrive/Project/customTF2/data/val/*.tfrecord"
    
  }
 Loss 
![Loss](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/82a61ea5-4dd0-49ca-8d80-39a44fa25ef5)
Precision
![Pre](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/1e44d474-ce77-4961-87de-52661eff2636)
Recall
![Recall](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/5bfd87c1-a57a-40e8-bf09-2400ff183fe6)
Learning Rate
![LR](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/da3862af-ec3b-49d5-b2a6-78b2b7a08b19)


![Resnet](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/15267bf8-127d-4408-b132-3f7a9457fbe4)


3- SSD MobileNet V1 FPN 640x640

pipline.config changes :

num_classes: 3

batch_size: 8

fine_tune_checkpoint_type: "detection"

fine_tune_checkpoint: "/content/gdrive/MyDrive/Project/customTF2/data/efficientdet_d1_coco17_tpu-32/checkpoint/ckpt-0"

train_input_reader: {

  label_map_path: "/content/gdrive/MyDrive/Project/customTF2/data/train/label_map.pbtxt"
  
  tf_record_input_reader {
  
    input_path: "/content/gdrive/MyDrive/Project/customTF2/data/train/*.tfrecord"
    
  }
  
eval_input_reader: {

  label_map_path: "/content/gdrive/MyDrive/Project/customTF2/data/val/label_map.pbtxt"
  
  shuffle: false
  
  num_epochs: 1
  
  tf_record_input_reader {
  
    input_path: "/content/gdrive/MyDrive/Project/customTF2/data/val/*.tfrecord"
    
  }
  
 Loss
![Loss](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/8185634a-b20d-423a-aa3f-80d2aa5ba29a)
Precision
![Prec](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/0be78866-f106-4826-89f1-cb94b12d4877)
Recall
![Recall](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/c1f3f9de-ef81-4c49-9602-95947cbcc7d8)
Learning Rate
![LR](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/b6b3eb3e-28a4-47bf-944e-06643a5b610c)


![MobileNet](https://github.com/AhmedMahmoudAhmedMahmoud/Object-Detection-In-Urban-Enviroment/assets/130584964/610ac98d-3792-40b0-a80a-d381e8fcbcb2)

Resnet50 achieved lower loss values earlier than both EfficientNet and MobileNet models, as evident from the results obtained. EfficientNet took comparatively more steps to minimize the loss than MobileNet.And MobileNet could not detect the pedestrian while the EfficientDet was able to detect it.

The provided testing frames were all successfully analyzed by the three models in terms of vehicle detection. However, upon closer examination, it was found that MobileNet detected vehicles with some additional noise, which was not present in the results of the EfficientNet and ResNet50 models.

For the most part, ResNet50 and MobileNet models were able to detect pedestrians, although MobileNet struggled with critical cases. On the other hand, EfficientNet consistently detected pedestrians with minimal noise throughout the entire testing phase.

Due to a low number of training and validation steps, none of the three models were able to detect the presence of cyclists.

After analyzing the training results through TensorBoard, along with the detection outcomes on test samples, it was determined that the pre-trained EfficientNet D1 model was the optimal choice for deployment out of the three tested models, based on its total loss and mAP values.

We can improve the performance of the tested models by Increasing the amount of training data, Fine-tuning the pre-trained models, Tuning the hyperparameters, Using data augmentation.
