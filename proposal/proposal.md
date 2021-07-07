# Advanced Machine Learning Project Proposal

## Team

* Jessica Kächele, 3588787, uo251@stud.uni-heidelberg.de
* Jonas Reinwald, 3600238, am248@stud.uni-heidelberg.de

## Proposal 1: Reinforcement Learning of Countermeasures
### Scientific Question
The Covid-19 crisis confronts everyone with new, previously unknown challenges. Politicians in particular have to make decisions with consequences that are not fully foreseeable. Simulations can help to simulate countermeasures and observe their consequences before trying them out in the real world. This can help politicians to make better decisions. However, there are many different possibilities and scenarios. Trying them all out would be very time-consuming and hardly feasible. However, a reinforcement learning model could learn the correct use of countermeasures. With the help of the model, one could create a walkthrough that may be followed to keep the negative consequences as small as possible.

### Papers
There are several papers that employ this approach [https://www.nature.com/articles/s41598-020-79147-8,
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7311597/, 
https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0251550,
https://kowshikchilamkurthy.medium.com/reinforcement-learning-for-covid-19-simulation-and-optimal-policy-b90719820a7f]. All of them use deep Q-learning. 
Mostly, however, the simulations are kept very simple. Only movement restrictions are used as countermeasures.
Measures such as vaccinations or wearing masks are not included. However, these can be very important factors that should not be excluded. Furthermore, the psychological effects of, for example, contact restrictions should not be ignored.
In the papers mentioned, however, only economic and health system factors are considered. This neglects an important factor of the pandemic. The strictest contact restrictions do not help if they are not being followed.

### Methods
We would like to use and expand the above simulation. More countermeasures such as wearing masks, keeping distance, contact tracing and quarantine, compulsory home office and school closures, vaccinations will be implemented. Furthermore, in addition to the overload of the health system and the economic impact, the psychological impact will also be measured.
These impacts will then be used as rewards for the reinforcement learning agent. 
We want to use deep reinforcement learning and will orient ourselves on the above-mentioned papers.

### Data Sources
This project does not require any data sources, as the data is produced by the simulation itself. However, key figures are needed on the extent to which a countermeasure reduces the risk of infection. Studies such as this [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7684142/] can be used for this purpose.
There is also data available on the effectiveness of vaccination, such as [https://www.rki.de/DE/Content/Infekt/EpidBull/Archiv/2021/Ausgaben/02_21.pdf?__blob=publicationFile] or [https://www.astrazeneca.com/content/astraz/media-centre/press-releases/2021/astrazeneca-us-vaccine-trial-met-primary-endpoint.html] and studies / reports of the psychological impact from countermeasures like [https://www.iao.fraunhofer.de/en/press-and-media/latest-news/pinpointing-the-impact-of-the-covid-19-pandemic-with-ai.html, https://onlinelibrary.wiley.com/doi/10.1002/epa2.1091, https://www.rki.de/EN/Content/Health_Monitoring/Health_Reporting/GBEDownloadsJ/JoHM_S7_2020_Social_Inequalities_COVID_19.pdf?__blob=publicationFile].

### Possible Difficulties
The main concern is that the model takes a long time to converge, as it is the case in [https://www.nature.com/articles/s41598-020-79147-8]. 
Furthermore, it might be difficult to evaluate countermeasures in terms of their psychological impact.

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

There are a lot of papers trying to detect COVID-19 on lung CT scans, lung X-rays or similar data using mostly CNNs. `f-AnoGAN` [https://www.researchgate.net/publication/330796048_f-AnoGAN_Fast_Unsupervised_Anomaly_Detection_with_Generative_Adversarial_Networks] is a paper that tries to detect anomalies in retina images by utilizing a GAN to compare input images with reconstructions. This method could be modified to detect if a given query image contains COVID-19 and the performance compared against a few of the aforementioned papers (see also proposal 2 data sources for papers that could be used). 

As their training is rather resource intensive, we are not sure if it is possible for us to train a sufficiently big enough GAN to tackle this project.

## Available Computational Resources

* Intel Skylake 6th Gen 4C / 8T CPU (6700K)
* 16GB RAM
* Nvidia RTX 2070 Super (8GB VRAM)

or, if necessary, some form of online resource:
* https://colab.research.google.com/notebooks/intro.ipynb
* https://cloud.google.com/gpu/
* https://www.paperspace.com/
* https://www.floydhub.com/
* https://crestle.ai/
* https://azure.microsoft.com/en-us/pricing/details/virtual-machines/linux/

