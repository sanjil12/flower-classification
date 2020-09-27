# flower-classification
flower image classification using CNN on TPUs (tensorflow)
Dataset: 12753 training images, 3712 validation images, 7382 unlabeled test images
dataset stored in tfrecords,i.e tfrecords conatins images with labels in it saved as a record
we need to decode the images with the labels
refrence-https://colab.research.google.com/github/GoogleCloudPlatform/training-data-analyst/blob/master/courses/fast-and-lean-data-science/03_Flower_pictures_to_TFRecords.ipynb#scrollTo=vjw8GURL8wjk
starting with the tpu detection 
Note:tfreacords work with tensorflow(tensorflowrecords)i.e. run only on tpu or gpu
using pre_trained model Xception net with all layers trainable
adam optimizer and sparse categorical entropy
after training model , convert it into tflite model file to get integrated on android
