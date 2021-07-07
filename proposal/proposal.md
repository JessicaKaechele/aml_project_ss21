# Advanced Machine Learning Project Proposal

## Team

* Jessica Kächele, 3588787, uo251@stud.uni-heidelberg.de
* Jonas Reinwald, 3600238, am248@stud.uni-heidelberg.de

## Proposal 1
### Scientific Question
### Papers
### Methods
### Data Sources
### Possible Difficulties

## Proposal 2: Federated Machine Learning
### Scientific Question
### Papers
### Methods
### Data Sources
### Needed Computational Resources 
The paper mentions the following hardware that was used during experiments:
| Type | Hardware | 
|---|---|
| CPU | Intel Core i7–6700HQ |
| GPU | NVIDIA GeForce GTX 950M (4GB DDR3) |
| Storage | 256GB SSD + 1000 GB HDD |
| RAM | 16GB DDR3L, 2133 MHz |

### Possible Difficulties
It might be difficult to successfully adopt federated ML to other approaches, but this is exactly what we want to find out.

### Additional Goals
Instead of adopting existing models manually to federated learning, it would be helpful if this could be done automatically. If time and other project parameters allow we could try so build an automated process for this (for specific ML frameworks and/or model types, e.g. Pytorch, Tensorflow, ... / CNNs, ... ).

## Bonus Proposal
We are also interested in another project idea, but we were not sure how feasible it is to achieve and will therefor only briefly mention it. If it sounds like a reasonable idea, we could flesh it out to the length of the other proposals in the feedback week.

There are a lot of papers trying to detect COVID-19 on lung CT scans, lung X-rays or similar data using mostly CNNs. `f-AnoGAN` (https://www.researchgate.net/publication/330796048_f-AnoGAN_Fast_Unsupervised_Anomaly_Detection_with_Generative_Adversarial_Networks) is a paper that tries to detect anomalies in retina images by utilizing a GAN to compare input images with reconstructions. This method could be modified to detect if a given query image contains COVID-19 and the performance compared against a few of the aforementioned papers (see also proposal 2 data sources for papers that could be used). 

As their training is rather resource intensive, we are not sure if it is possible for us to train a sufficiently big enough GAN to tackle this project.

## Available Computational Resources

* Intel Skylake 6th Gen 4C / 8T CPU
* 16GB RAM
* Nvidia RTX 2070 Super (8GB VRAM)

or, if necessary, some form of online resource:
* https://colab.research.google.com/notebooks/intro.ipynb
* https://cloud.google.com/gpu/
* https://www.paperspace.com/
* https://www.floydhub.com/
* https://crestle.ai/
* https://azure.microsoft.com/en-us/pricing/details/virtual-machines/linux/

