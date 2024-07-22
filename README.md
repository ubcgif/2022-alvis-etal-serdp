# Machine learning methods for the classification of UXO from electromagnetic data in marine setting

_Jorge Lopez-Alvis, Lindsey J. Heagy, Douglas W. Oldenburg, Stephen Billings and Lin-Ping Song_

![thumbnail](./abstract/thumbnail.png)

## Summary 

Multicomponent time-domain electromagnetic (TDEM) systems are currently used to successfully detect and classify unexploded ordnance objects (UXOs) in terrestrial settings. Typically, classification is done by first performing a physics-based inversion, which assumes a dipolar response and gives the polarizabilities of the ordnance object as an output. The polarizabilities are then compared with a library of known ordnance objects and a class is assigned. In marine settings, several complicating factors are introduced.The conductive seawater and sediments have an EM response that needs to be accounted for and there is typically larger uncertainty in sensor positioning as compared to the terrestrial case. These factors may adversely impact inversion results and hence classification. Machine learning (ML) methods and in particular convolutional neural networks (CNNs) have been very successful in classifying directly from data given a sufficiently large set of examples. Our work is examining the use of CNNs to classify ordnance objects from TDEM data. We train a CNN with synthetic data generated using ordnance libraries by randomly assigning class, noise level and location and orientation of the target object. Once trained, our CNN outputs a probability that the signal in a given spatial window is associated with an ordnance object. An important component of the success of CNNs for classification is feature design. Ultimately, we want input features and a network architecture that are robust to challenges such as positional uncertainties, a range of levels of background noise, and different types of clutter. We examine and test a suite of input features (e.g. by applying scaling or normalizations to the data) and their utility for classification. Our initial focus is on synthetic and terrestrial data to develop a proof-of-concept for the use of CNNs as a complementary tool to inversions for classification of UXO from TDEM data. We plan to further investigate network architectures, input features, and choice of loss function that enable transferability to the marine setting.

## Citation 

