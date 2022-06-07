
A mask detection model based on Tensorflow object detection API

This model is based on RetinaNet architecture trained on COCO dataset of 90 original classes.
However it has been modified to detect a new class, the presence of a human mask in the face.
The model is pretrained but removed the classification head and added another one for masks, 
it is trained further on a limited dataset of face masks annotated in Colab (in this case just
25 images). 

After transfer learning and training on the new images the model is used to detect images of faces with masks.

Furthermore if given a correctly annotated XML format images, a script is provided to obtain bounding box coordinates 
and feed them directly to the the model for training or inference.
