**detectron2**
- configs： Sample profile collection , Including the configuration of network models such as detection and segmentation , image faster rcnn,cascade rcnn etc. .
- datasets： Data set preparation , It is mainly the basic structure of each data set , And how to preprocess .
- demo： Quick experience Detectron2, And Getting Started The document corresponds to . If you want to experience Model ZOO You can use this for the content of the result in .

tests： Unit test class .
tools： Frequently used scripts , Such as training 、benchmark、 Display data sets, etc .
Pros:

It has been designed to be modular, flexible, and extensible for efficient training on single or multiple GPUs. 
The Detectron2—the successor of Detectron and maskrcnn-benchmark includes SOTA object detection algorithms such as DensePose, panoptic feature pyramid networks, and numerous variants of the pioneering Mask R-CNN. 
It is one of the tools published in the PyTorch ecosystem.
Cons:

It does not offer access to all SOTA models. 
It is restricted to detection and segmentation and does not support other computer vision tasks such as classification. 
Its hard integration involving a modular yet abstract approach makes it very difficult to make changes to the deep learning model. 

--------------------------------------------------------------------------------------------------------------


**mmdetection** 
configs： Sample profile collection , Including the configuration of network models such as detection and segmentation , image faster rcnn,cascade rcnn etc. .
demo： Quick experience Detectron2, And Getting Started The document corresponds to . If you want to experience Model ZOO You can use this for the content of the result in .
mmdet： The main code of the project is here .
docker： Nothing to introduce .
docs： Some official documents .
tests： Unit test class .
tools： Frequently used scripts , Such as training 、benchmark、 Display data sets, etc .

Pros:

It provides access to SOTA object detection deep learning models such as FasterRCNN, DETR, VFNet, and others. 
The major features of the toolbox include modular design, support of multiple frameworks out of box, and high efficiency. 
The toolbox also includes scripts for visualization, model conversion, benchmarking, hyper-parameter optimization, among other related tasks.
Cons:

It is restricted to supporting object detection models and some instance detection models. 
It does not support other computer vision problems such as classification.







https://mmdetection.readthedocs.io/en/latest/model_zoo.html#comparison-with-detectron2


https://www.libhunt.com/compare-mmdetection-vs-detectron2?ref=compare
















