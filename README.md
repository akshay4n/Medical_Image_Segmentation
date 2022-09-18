Multi-scale self-guided attention for medical image segmentation
<br>
Objectives:<br>
* To provide automatic segmentations of medical images which are of good precision.
* To capture richer contextual dependencies based on the use of guided self-attention mechanism
* To neglect irrelevant information and focus on more discriminant regions of the image by emphasizing relevant feature association
<br>
Datasets:CHAOS Dataset<br>
Methodology:
1. Multiple Scales attention maps
    1. Positional Attention Module(PAM)
    2. Channel Attention Model (CAM)
    ![img2](/images/model_attention.jpg)
2. UNet Model for comparison
<br>
Results:<br>
![imag](/images/result.png)
