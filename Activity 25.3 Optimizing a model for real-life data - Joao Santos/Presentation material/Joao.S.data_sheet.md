# Datasheet Template 

## Motivation

**- For what purpose was the dataset created?** 
**- Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?**

The dataset was crated as more and more data is necessary at present to develop a diagnosis module to detect a fault, that may afect the operation of industrial system and locate their causes - thereby improving manufacturing effeciency, reducing downtime and therefore reducing costs. 

The dataset was created by an independant contributor on Kaggle. 
 
## Composition

**- What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)?** 
**- How many instances of each type are there?** 
**- Is there any missing data?**
**- Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals' non-public communications)?**

In the dataset, there are 62,629 total values of temperature readings for the temperature sensor in question - with no missing data and no confidential data. All this information is of public domain. 

## Collection process

**- How was the data acquired?** 
**- If the data is a sample of a larger subset, what was the sampling strategy?** 
**- Over what time frame was the data collected?**

The data was acquired in an automated fashion in an industrial sensor between the 1st of August 2016 and the 1st of September 2017. 

## Preprocessing/cleaning/labelling

**- Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section.** 
**- Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?** 

Initially, the data was sorted on Excel by date and time - and the loaded onto Jupyter notebooks. After this a visualization was performed, the data was checked for missing values (none were found) and hen the data was cleaned and transformed. Feature matrix X and target variable Y were defined, a train-test split was performed and data scaling / normalization process was done. 
 
## Uses

**- What other tasks could the dataset be used for?** 
**- Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms?** 
**- Are there tasks for which the dataset should not be used? If so, please provide a description.**

This task provides valuable information for understanding temperature variations over time, identifying patterns and detecting potential faults. This can be applied in a plethora of aspplications - whether these are industrial or not. This model can be used for anomaly detection for example, predictive maintenance and trend analysis. 

Preprocessing steps, such as data scaling and feature engineering, might impact model performance. Users should be aware of potential biases introduced during cleaning and preprocessing.

This model can be used for a plethora of other applications both industrial or not (such as with the use of pressure sensors, flow, vibrations, acceleration, conductivity, pH etc.). However slight modifications must be made and the data processing would have to be revisited to check if it suits a new set of data. 

## Distribution

**- How has the dataset already been distributed?** 
**- Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?**  

The dataset has been distributed on Kaggle by an independent user, it is of CC0 Public domain and is licensed under Open Database License (ODbL) V1.0.

## Maintenance

**- Who maintains the dataset?**

Independant user on Kaggle

