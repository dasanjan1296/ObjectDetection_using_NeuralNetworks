**There is no native leaky relu layer in Mathematica, but it can be constructed easily using a ElementwiseLayer
**There is no native leaky relu layer in Mathematica, but it can be constructed easily using a ElementwiseLayer
**The output of the final MyNetwork is a 1470 vector, which contains the coordinates and confidence of the predicted bounding boxes for different classes. The dataset "train.weights" has 20 classes mentioned in the labels set.
**The 1470 vector output is divided into three parts, giving the probability, confidence and box coordinates. Each of these three parts is also further divided into 49 small regions, corresponding to the predictions at each cell. Each of the 49 cells will have two box predictions. In postprocessing steps, we take this 1470 vector output from the network to generate the boxes that with a probability higher than a certain threshold. The overlapping boxes will be resolved using the non-max suppression method.
**The image extracted from the urls are displayed first and then fetched for Post-Processing step.
**After going through MyNetwork, the output is in form of a college with objects detected inside labelled bounding boxes.

                                                   ********THANK YOU**********