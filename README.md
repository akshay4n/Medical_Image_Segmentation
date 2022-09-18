# Multi-scale self-guided attention for medical image segmentation


## Objectives:<br>
* To provide automatic segmentations of medical images which are of good precision.
* To capture richer contextual dependencies based on the use of guided self-attention mechanism
* To neglect irrelevant information and focus on more discriminant regions of the image by emphasizing relevant feature association


## Datasets:
        CHAOS Dataset, nucleus dataset from 2018 Data Science Bowl Challenge

## Methodology:<br>
1. Multiple Scales attention maps
    1. Positional Attention Module(PAM)<br>
    2. Channel Attention Model (CAM)<br>
  ![img2](/images/model_attention.jpg)<br>
2. UNet Model for comparison<br>
    ![img2](/images/model_unet.jpg)<br>
<br><br>
Proposed Model:<br>
![imageProp](/images/model_proposed.jpg)<br>

## Results:<br>

Unet vs Proposed model:<br>
    ![imag](/images/tab_Res.jpg)<br>

<!--     ![imag](/images/result.png)<br> -->
Result on CHAOS Dataset:<br>
    ![imag2](/images/Res_CHAOS.jpg)<br>
Result on NUCLEUS Dataset:<br>
    ![imag2](/images/Res_nucleus.jpg )<br>
    
We have considered the two models - the proposed model of multi scale self guided attention model and other model of Unet architecture. We have also considered two datasets for abdominal organ detection of CHAOS dataset and Nucleus detection of 2018 Data Science Bowl Challenge dataset. We have considered two metrics of DICE and MSE for evaluation the performance of the model

## Concluding Remarks:<br>
The model with multi-scale guided attention mechanism outperformed the Unet model as evident from the results. The use multi scale strategy and attention mechanism helped achieve better accuracy. The multi scale helped retrieve important semantic information and the self attention model aggregated the relevant contextual features. To filter out noises from the output so obtained the model uses a guided refinement module. There was a comparison made between two datasets and also their associated score with the two different models used in this paper. In both the cases the multi-scale guided attention mechanism outperformed the other model
