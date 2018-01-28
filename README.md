# Abalone 
## Domain
Abalone is a shellfish considered a delicacy in many parts of the world. The abalone shell and the meat is of value.  The goal of this project is to perform exploratory data analysis for the HAbalone dataset which is a modification of the Abalone Dataset (http://archive.ics.uci.edu/ml/datasets/Abalone). The original Abalone dataset is a 9D dataset and HAbolone is a 10D dataset with an ordinal Age attribute added; HAbalone has the the following attributes:

## Problem Statement
Predict the age of abalone from physical measurements

## Dataset

- Number of Instances: 4177
- Number of Attributes: 8
- Missing Attribute Values: None

|Name		        | Data Type	     |Meas.	  |Description                |
|---------------|:--------------:|:------:|--------------------------:| 
|	Sex       	  | nominal			   |        |M, F, and I (infant)       |
|	Length	      | continuous	   |  mm    |Longest shell measurement  |
|	Diameter	    | continuous	   |  mm  	|perpendicular to length    |
|	Height		    | continuous	   |  mm	  |with meat in shell         |
|	Whole weight  |	continuous	   | grams	|whole abalone              |
|	Shucked weight|	continuous	   | grams	|weight of meat             |
|	Viscera weight|	continuous	   | grams	|gut weight (after bleeding)|
|	Shell weight	| continuous	   | grams	|after being dried          | 
|	Rings	        | integer			   |        |+1.5 gives the age in years|

Predicting the age of abalone from physical measurements. The age of abalone is determined by cutting the shell through the cone, staining it, and counting the number of rings through a microscope -- a boring and time-consuming task. Other measurements, which are easier to obtain, are used to predict the age. Further information, such as weather patterns and location (hence food availability) may be required to solve the problem. 

From the original data examples with missing values were removed (the majority having the predicted value missing), and the ranges of the continuous values have been scaled for use with an ANN (by dividing by 200).


## Proposed Solution
Given is the attribute name, attribute type, the measurement unit and a brief description. The number of rings is the value to predict: either as a continuous value or as a classification problem. 


## Benchmark Model


## Performance Metric


## Conclusion
