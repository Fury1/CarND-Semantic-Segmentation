# Semantic Segmentation
### Introduction
In this project a Fully Convolutional Network (FCN) is used to define the pixels in an image that represent the road.

### Setup
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/) <-- GPU version preferably
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)

---

#### Dataset
Download the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).  Extract the dataset in the `data` folder.  This will create the folder `data_road` with all the training a test images.

#### Start
Ensure you have the above packages installed. If training on a CPU be prepared to wait a while. This project it best trained on a GPU due to the complexity of FCNN semantic segmentation.

#### Run
Run the following command to train and run the model on the Kitti Road dataset test images:
```
python main.py
```
**Note** If running this in Jupyter Notebook system messages, such as those regarding test status, may appear in the terminal rather than the notebook.

---

### Successfully trained model examples:
[image1]: ./example_images/umm_000008_original.png
[image2]: ./example_images/um_000022_original.png
[image3]: ./example_images/umm_000008.png
[image4]: ./example_images/um_000022.png

|Example 1| Example 2|
|:---:|:---:|
|![Original Sample 1][image1] |![Original Sample 1][image2]|
|![Prediction Sample 1][image3] |![Prediction Sample 1][image4]|

### Future Improvements
* Gather more data to train and increase the accuracy
* Add more classes to find more objects in images
* Apply the above model improvements to a video and optimize for real time predictions



