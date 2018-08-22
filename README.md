# DeepDream
Playing around with Google's [DeepDream](https://ai.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html) algorithm for feature visualization.

## Resources
This example is based on Google's algorithms for feature visualization in their [Tensorflow examples](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/examples/tutorials/deepdream) and [HvassLabs](https://github.com/Hvass-Labs/TensorFlow-Tutorials)'s recursive image optimization algorithm. 

## Idea
Testing how the Inception V5 and VGG16 models and their layers react to random noise and different input images in terms of features. The following algorithms suggested by Google were tested:
1. Simple gradient ascent
2. Multiscaled gradient ascent
3. Laplacian Pyramid Gradient Normalization
4. DeepDream
5. HvassLabs's recursive optimization algorithm.

## Examples
Input image:

![Cat](https://github.com/JadeBlue96/DeepDream/blob/master/test_images/cat.jpg)

Inception V5 DeepDream on the conv2d1 layer:

![CatDeep](https://github.com/JadeBlue96/DeepDream/blob/master/test_output/output_cat_Inception5h_conv2d1_recursive_optimize.jpg)

VGG16 DeepDream on the conv3_2 layer:

![CatDeep2](https://github.com/JadeBlue96/DeepDream/blob/master/test_output/output_cat_VGG16_conv3_2_recursive_optimize.jpg)

Inception V5 DeepDream on the mixed4_b layer applied to a clean gray image:

![IncGray](https://github.com/JadeBlue96/DeepDream/blob/master/test_output/output_Inception5h_mixed4b_render_deepdream.jpg)

VGG16 DeepDream on the conv5_1 layer applied to a clean gray image:

![VGGGray](https://github.com/JadeBlue96/DeepDream/blob/master/test_output/output_VGG16_conv5_1_render_deepdream.jpg)

Check out the `test_output` directory for more interesting examples.
