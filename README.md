# Build-Your Own Transfer Learning Neural Network
---
This is project code for Udacity's Intro to Machine Learning Nanodegree program. In this project, code developed for an image classifier built with PyTorch, then converted into a command line applications: train.py, predict.py, load_model.py, and data_processing.py.

The image classifier to recognize different species of flowers. Dataset contains 102 flower categories. However, any dataset can be used to create a Convolutional Neural Network using train.py. More details on how the Image Classifier works in the PyTorch Transfer Learning.ipynb.

If you want access to the flowers data and my model checkpoint, they're in my Google Drive [here](https://drive.google.com/open?id=1weQumRkbqBua8cT2oau6Bg5Hjuz6kUPJ). I trained this model on the [Caltech 101 Images](http://www.vision.caltech.edu/Image_Datasets/Caltech101/) dataset, and it worked as well.

### Command line applications train.py & predict.py (leverage code from load_model.py, and data_processing.py)
---
### train.py arguments...

Use train.py to train your own neural network! Tip: train this on a GPU, or you'll *never* finish.

---
1.  'data_directory'. 'Provide data directory on which to train the model. Mandatory argument', type = str
2.  '-a' or '--arch'. 'All VGG models can be used. Otherwise, VGG16 will be used', type = str
3.  '-hid or '--hidden_units'. 'Hidden units in Classifier. Default value is 4096', type = int
4.  '-o' or '--output_units. Output units in Classifier. Default value is 102', type = int
5.  '-lr' or '--learning_rate'. 'Learning rate, default value 0.001', type = float
6.  '-e or '--epochs'. 'Number of epochs, default value is 5', type = int
7.  '-p' or '--p' 'Number of batches to train model on before printing validation testing results, default value is 5', type = int
8. '-g' or '--GPU'. "Option to use GPU", type = str
9. '-sd' or '--save_dir'. 'Provide saving directory if you want to save the model checkpoint elsewhere', type = str

---
#### predict.py

Use predict.py to use your model to predict classes of images.

- You can have it predict on 1 image or an entire directory of images. 
- Use -sr to have it save results in a file called predictions.csv<br>
---
1. 'checkpoint' 'Path to location of trained model checkpoint. Mandatory.' type = str
2. '-i' or '--image' Mandatory mutually exclusive 'Path to image', type = str
3. '-d' or '--dir' Mandatory mutually exclusive 'Path to directory containing images', type = str
3. '-t' or '--top_k'. 'Top K most likely classes. Default is 5', type = int
4. '-cn' or '--category_names'. 'Mapping of categories to real names. JSON file name to be provided. Optional', type = str
5. '-g' or '--GPU'. "Option to use GPU. Optional", type = str
6. '-sr' or '--save_results' 'Save results to predictions.csv? Optional.' 
# PyTorch-Image-Classifier
