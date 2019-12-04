+++

title="Phase3 Image Caption"

+++
**Phase 3 Image Caption**<br>

Dataset Link: https://www.kaggle.com/hsankesara/flickr-image-dataset <br>
Github Link: https://github.com/sathvik-sankruth/Term-project <br>
Website Link: http://satsankruth.pythonanywhere.com/ <br>
Demo Video Link: https://www.youtube.com/watch?v=LwQrrgDDlmE <br>

Image captioning is the task of generating a caption for an image.
Uses TensorFlow and Neural Network to generate captions on the google collab repository.
This model architecture is similar to Neural Image Caption Generation with Visual Attention.
The code uses tf.keras and eager execution
The notebook will download the MS-COCO dataset, preprocess and cache a subset of the images using Inception V3, train an encoder-decoder model, and use it to generate captions on new images.
 <br>
 
**Contribution:**<br>
Modified the code to test my dataset and stored it in csv file with image url and captions.<br>
![img](https://sathvik-sankruth.netlify.com/img/imgcap1.PNG)
![img](https://sathvik-sankruth.netlify.com/img/imgcap2.PNG)
 <br>
**Challenges Faced:**<br>
Training the model takes around 3hrs.<br>
My dataset was huge 30K images which is around 4Gb hence modified my dataset to 2K images which is around 600Mb.<br>
Testing the model with the reduced data took additional 1hr.<br>
Understanding how Jupyter Notebook, Tensor flow, Neural Network, Google Collab Feature works was a bit challenging.<br>

**Reference:**<br>

* https://github.com/tensorflow/tensorflow/blob/r1.13/tensorflow/contrib/eager/python/examples/generative_examples/image_captioning_with_attention.ipynb

* https://arxiv.org/abs/1502.03044

* https://www.tensorflow.org/guide/keras

* https://www.tensorflow.org/guide/eager

* https://hackernoon.com/begin-your-deep-learning-project-for-free-free-gpu-processing-free-storage-free-easy-upload-b4dba18abebc 


<br><br>
[Phase 1 Search](https://sathvik-sankruth.netlify.com/project/phase1search/)
[Phase 2 Classify](https://sathvik-sankruth.netlify.com/project/phase2classifier/)
<br><br>
