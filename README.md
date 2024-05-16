# MAFAttention
**Abstract:**
Embedding attention modules into deep convolutional neural networks (CNNs) is currently one of the common deliberations to enhance their learning ability of feature representation. In previous works, the global channel-wise features of a given tensor are computed and squeezed into CNN-based models through an attention mechanism. Squeezing different kinds of these features can lead to the less fusion of attentive information due to the independent operations of channel-wise recalibration. To deal with this issue, an efficient attention module of accumulated features (MAF) is proposed by accumulating these diverse squeezes for a unitary recalibrating perceptron as follows. Firstly, we take advantage of average and deviation calculations to produce correspondingly statistical patterns of a given tensor for aggregating the global channel information. An adaptative perceptron of deformed-bottleneck recalibration (DBR) is then presented to cohere the resultant features. Finally, the robust DBR-based lightweights will be utilized to weight the concerning tensor. Additionally, to exploit more spatial-wise information, we address MAF for an effective alternative of the channel-wise component in two critical attention units to form two corresponding modules that will be then inspected to indicate which integration is good for real applications. We adapt the MAF-based modules to MobileNets for further enhancement investigation. Experiments on benchmark datasets for image classification have proved the efficacy of our proposals.
<u>**An example for training CGDFNet on Places365:**</u>

```
$ python CGDFNet_places365.py
```
Note: Subject to your system, modify these training files (*.py) to have the right path to dataset

**Validating the trained model of CGDFNet on Places365:**
```
$ python CGDFNet_places365.py --evaluate
```
Note: For instances of validation of CGDFNet, download the trained model of CGDFNet on Places365: [Click here](https://drive.google.com/file/d/1BpoTBLcdAFwFVVv4dZJ5NxslqKcq5AQ8/view?usp=drive_link). And then locate the downloaded file at ./runs/CGDFNet_g1_/

**Related citations:**

If you use any materials, please cite the following relevant works.

```
@article{MAFAttNguyen24,
  author       = {Thanh Tuan Nguyen, Thanh Phuong Nguyen, and Vincent Nguyen},
  title        = {Accumulating global channel-wise features via deformed-bottleneck recalibration},
  journal      = {Pattern Analysis and Applications},
  note         = {(submitted in 2024)}
}
```
