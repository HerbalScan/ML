## Machine Learning (ML) for HerbalScan
Our main goal is to build plant identification. Here are the steps to do it:
### Create dataset
First, we collect images of medicinal plants. Currently, our dataset consists of >4500 images for 15 classes.
### Preprocess data
Our data may contain invalid images that can't be trained, e.g. some image extensions are not compatible. So, the data is further cleaned. Then, we split the data and use ImageDataGenerator to do data augmentation (rotate, zoom, flip, etc.).
### Train model
We attempted to use CNN to build the model. Also, we tried to do transfer learning with MobileNet. The final model is saved in HDF5 format to be deployed using FastAPI.
