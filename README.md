# Abalone 
## Domain
Abalone is a shellfish considered a delicacy in many parts of the world. An excellent source of iron and pantothenic acid, and a nutritious food resource and farming in Australia, America and East Asia. 100 grams of abalone yields more than 20% recommended daily intake of these nutrients. The economic value of abalone is positively correlated with its age. Therefore, to detect the age of abalone accurately is important for both farmers and customers to determine its price. However, the current technology to decide the age is quite costly and inefficient. Farmers usually cut the shells and count the rings through microscopes to estimate the abalones age. Telling the age of abalone is therefore difficult mainly because their size depends not only on their age, but on the availability of food as well. Moreover, abalone sometimes form the so-called 'stunted' populations which have their growth characteristics very different from other abalone populations This complex method increases the cost and limits its popularity. Our goal in this report is to find out the best indicators to forecast the rings, then the age of abalones (http://archive.ics.uci.edu/ml/datasets/Abalone)

## Problem Statement
Predict the age of abalone from physical measurements.

The age of abalone is determined by cutting the shell through the cone, staining it, and counting the number of rings through a microscope -- a boring and time-consuming task.  Other measurements, which are easier to obtain, are used to predict the age. Further information, such as weather patterns and location (hence food availability) may be required to solve the problem.

## Dataset

- Number of Instances: 4177
- Number of Attributes: 8
- Missing Attribute Values: None

![size](https://user-images.githubusercontent.com/33742913/35494570-5af42712-0470-11e8-95f0-6d57b293701d.PNG)

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

From the original data examples with missing values were removed (the majority having the predicted value missing), and the ranges of the continuous values have been scaled for use with an ANN (by dividing by 200). *As per UCI website** 


## Proposed Solution

We are provided with attribute name, attribute type, the measurement unit and a brief description. 
Our aim for abalone dataset is to predict abalone age (through the number of rings on the shell) given various descriptive attributes of the abalone (length, diameter, weights of whole abalone and parts of shucked abalone). 
As we know rings are used to claculate age & to achieve this goal we will attempt to predict rings using the the shell sizes (height, length, width, and weights etc. The problem associated with this dataset is that these descriptive attributes are all heavily correlated.

The number of rings is the value to predict: either as a continuous value or as a classification problem. 

Apply different regression techniques:
We are interested in performing various regression techniques such as additive models, interactions, polynomial transformations of the variables etc to be able to predict and assess the accuracy of our prediction.

## Benchmark Model
Given that we seek a regression model a good naive benchmark would be to use either the mean or the median of the volume of the abalone assuming it's a cylinder shape, πr^2h or a simple regressin model

## Performance Metric
Given that this is a regression task, we can measure the success of our model using the R^2 metric, the Mean Absolute Error, or the Mean Square Error.

## Conclusion
