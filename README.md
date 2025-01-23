# HToPred
Human Topoisomerase II inhibitor Prediction Tool


The enzyme human topoisomerase IIα (hTopoIIα) is an important anticancer drug target. Due to the availability of multiple inhibitor-binding sites in this enzyme, the anti-hTopoII agents possess high chemical diversity. Chemoinformatics methods can be used to identify lead compounds from large databases for hTopoII inhibitory activity and classify them. In this work, we report the use of machine learning methods to develop classification models for the identification of possible anti-hTopoIIα agents and to classify them as catalytic inhibitors vs. poisons. Initially, an extensive dataset of small molecules which are reported to be evaluated towards hTopoIIα inhibition was collected from ChEMBL database and literature. Using this dataset, predictive models for classifying small molecules into hTopoIIα inhibitors and non-inhibitors were developed. Additionally, the model development was taken up for the prediction of the type of hTopoIIα inactivation. Several molecular fingerprints and physicochemical descriptors of the molecules in the dataset were calculated using the chemoinformatics tool RDKit. Various classifiers were evaluated to establish suitable protocol. Further, ensemble models were developed by bagging of homogenous classifier and selective fusion of heterogeneous classifiers. The models were thoroughly validated with 5-fold cross validation and external validation. The best performing models were incorporated into a tool Human Topoisomerase IIα Inhibitor Prediction (HToPred). 



![image](https://github.com/user-attachments/assets/968c9228-de21-45f4-842d-0dd5ba5cf594)


To run thepredictions, you need:
  numpy==1.11.0
  pandas==0.19.2
  scikit-learn==0.17
  rdkit
  joblib==0.10.3
  
To perform activity prediction

python Predicting//HToPredActivity.py -i molecule.sdf

To perform type of inhibitor prediction
python Predicting//HToPredTypeofInhibitor.py -i molecule.sdf

Cite: 
Tripathi, N.; Shaikh, N.; Bharatam, P. V.; Garg, P., HToPred: a tool for human topoisomerase II inhibitor prediction. Mol. Inform. 2019, 38, 1800046. (https://doi.org/10.1002/minf.201800046)
