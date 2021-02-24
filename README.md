# NCI-DOE-Collab-Pilot1-Tumor_Classifier

### Description:
The Tumor Classifier capability (TC1) shows how to train and use a neural network model to classify tumor types from molecular features 
(e.g., RNASeq expressions) provided in Genomics Data Commons (GDC).

### User Community:	
Primary: Cancer biology data modeling<br />
Secondary: Machine Learning; Bioinformatics; Computational Biology

### Usability:	
The provided untrained model can be used by a data scientist. The scripts use already processed data. The untrained model makes heavy use of CANDLE API layers which may limit its usability for novice users.

### Uniqueness:	
Using neural networks in classification of somatic mutation has been presented in other research papers. This model aggregates the variation impact by gene from 2.7 million unique SNPs which might not be the best way to reduce the features space. The technical team is not sure about the uniqueness of the method used to reduce the dimension of the somatic mutations.

### Components:	

Untrained model: 
* Untrained neural network model is defined in p1b2.model.json.

Data:
* Processed training and test data in MoDaC.

Trained Model:
* Trained model is defined by combining the untrained model + model weights.
* Trained model weights are used in inference p1b2.model.h5

### Technical Details:
Please refer to this [README](./Pilot1/TC1/README.md)
