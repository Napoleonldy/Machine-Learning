# Machine Learning Project 2 
# ** Comparison of the results in LetNet through different parameters  **
- Environment：anaconda3、jupyter notebook、python3.6
- Project library：
	
  ```
   from tensorflow.keras.optimizers import SGD
   from tensorflow.examples.tutorials.mnist import input_data

  ```
### Aim
TensorFlow and Keras were used to solve the algorithm CNN, and the parameters were adjusted for 3 trials each, for a total of 6 trials.


#### project "LetNet-5"
Tensorflow
1.①Input = 32x32x1. Output = 28x28x6. ②Input = 28x28x6. Output = 14x14x6. ③Output = 10x10x16. ④Input = 10x10x16. Output = 5x5x16. ⑤Input = 5x5x16. Output = 400.

EPOCH 1  Validation Accuracy = 0.969
EPOCH 2  Validation Accuracy = 0.982
EPOCH 3  Validation Accuracy = 0.982
EPOCH 4  Validation Accuracy = 0.986
EPOCH 5  Validation Accuracy = 0.985
EPOCH 6  Validation Accuracy = 0.987
EPOCH 7  Validation Accuracy = 0.989
EPOCH 8  Validation Accuracy = 0.988
EPOCH 9  Validation Accuracy = 0.989
EPOCH 10 Validation Accuracy = 0.987

2.①Input = 32x32x1. Output = 26x26x6. ②Input = 26x26x6. Output = 13x13x6. ③Output = 11x11x16. ④Input = 11x11x16. Output = 5x5x16. ⑤Input = 5x5x16. Output = 400.

EPOCH 1  Validation Accuracy = 0.964
EPOCH 2  Validation Accuracy = 0.978
EPOCH 3  Validation Accuracy = 0.983
EPOCH 4  Validation Accuracy = 0.980
EPOCH 5  Validation Accuracy = 0.983
EPOCH 6  Validation Accuracy = 0.985
EPOCH 7  Validation Accuracy = 0.988
EPOCH 8  Validation Accuracy = 0.988
EPOCH 9  Validation Accuracy = 0.985
EPOCH 10 Validation Accuracy = 0.989

3.①Input = 32x32x1. Output = 24x24x6. ②Input = 24x24x6. Output = 12x12x6. ③Output = 8x8x16. ④Input = 8x8x16. Output = 4x4x16. ⑤Input = 4x4x16. Output = 256.

EPOCH 1  Validation Accuracy = 0.971
EPOCH 2  Validation Accuracy = 0.979
EPOCH 3  Validation Accuracy = 0.982
EPOCH 4  Validation Accuracy = 0.987
EPOCH 5  Validation Accuracy = 0.986
EPOCH 6  Validation Accuracy = 0.988
EPOCH 7  Validation Accuracy = 0.989
EPOCH 8  Validation Accuracy = 0.990
EPOCH 9  Validation Accuracy = 0.989
EPOCH 10 Validation Accuracy = 0.990

Keras
1.①Input = 28x28x1. Output = 24x24x6. ②Input = 24x24x6. Output = 12x12x6. ③Input = 12x12x6. Output = 8x8x16. ④Input = 8x8x16. Output = 4x4x16. ⑤Input = 4x4x16. Output = 256.

EPOCH 1  Validation Accuracy = 0.9725
EPOCH 2  Validation Accuracy = 0.9809
EPOCH 3  Validation Accuracy = 0.9837
EPOCH 4  Validation Accuracy = 0.9793
EPOCH 5  Validation Accuracy = 0.9828
EPOCH 6  Validation Accuracy = 0.9821
EPOCH 7  Validation Accuracy = 0.9819
EPOCH 8  Validation Accuracy = 0.9864
EPOCH 9  Validation Accuracy = 0.9841
EPOCH 10 Validation Accuracy = 0.9851

2.①Input = 28x28x1. Output = 22x22x6. ②Input = 22x22x6. Output = 11x11x6. ③Input = 11x11x6. Output = 8x8x16. ④Input = 8x8x16. Output = 4x4x16. ⑤Input = 4x4x16. Output = 256.

EPOCH 1  Validation Accuracy = 0.9758
EPOCH 2  Validation Accuracy = 0.9807
EPOCH 3  Validation Accuracy = 0.9843
EPOCH 4  Validation Accuracy = 0.9847
EPOCH 5  Validation Accuracy = 0.9806
EPOCH 6  Validation Accuracy = 0.9841
EPOCH 7  Validation Accuracy = 0.9839
EPOCH 8  Validation Accuracy = 0.9841
EPOCH 9  Validation Accuracy = 0.9863
EPOCH 10 Validation Accuracy = 0.9852

3.①Input = 28x28x1. Output = 24x24x6. ②Input = 24x24x6. Output = 12x12x6. ③Input = 12x12x6. Output = 10x10x16. ④Input = 10x10x16. Output = 5x5x16. ⑤Input = 5x5x16. Output = 400.

EPOCH 1  Validation Accuracy = 0.9737
EPOCH 2  Validation Accuracy = 0.9796
EPOCH 3  Validation Accuracy = 0.9766
EPOCH 4  Validation Accuracy = 0.9844
EPOCH 5  Validation Accuracy = 0.9854
EPOCH 6  Validation Accuracy = 0.9842
EPOCH 7  Validation Accuracy = 0.9874
EPOCH 8  Validation Accuracy = 0.9843
EPOCH 9  Validation Accuracy = 0.9859
EPOCH 10 Validation Accuracy = 0.9857


###  Summary
1.Layer 1: Convolutional. The smaller the output shape, the more accurate you get in EPOCH 1.
2.Pooling.In this example, the output shape of 5x5x16 or 4x4x16 has little effect on the prediction accuracy.
