# _Once upon a time in... everywhere_
> That day, Juan entered his house slamming the door behind him. 
> He turned on the fan in the living room, opened the fridge and grabbed an ice-cold beer. 
> After a long sip, he began pacing the room like a caged lion, 
> his fingers tightening around the bottle. After a few more sips, 
> he finally lay down on his sofa and closed his eyes wondering **why the X-bank denied 
> the credit he requested!!!** 

X-bank has noticed that 30% of its total credits is in default, especially the ones to buy cars. The bank wants to increase its credit programs and to reduce its default rate.

# **How does the bank decide to whom it lends money?**

### Credit default prediction

### Exercise goal: 
##### Evaluate the accuracy of different models to predict the risk of credit default based on client's credit history.


| Files                          | Description | 
| :---                           |    :----:     | 
|Jupyter_Notebooks/Exploration_Data_Analysis.ipynb | Exploration_Data_Analysis | 
|Jupyter_Notebooks/ML_tunning.ipynb                | Parameter tunning        | 
|Jupyter_Notebooks/ML_PCA.ipynb                    | Playing with more metrics. Skippable _— alot of redundant code—_ |
|data/ Not included                    | [Download data here](https://raw.githubusercontent.com/ibmsoe/snap-ml/master/notebooks/credit-default-prediction-example.ipynb) | 



### Procedure
- **Data understanding and Data exploration** can be found in the jupyter notebook: *Exploration_Data_Analysis.ipynb*
- **Data preprocessing** 
1.Selecting data (Using only 10 K out of 10 Million data)
2.Balancing data
3.Standardization
4.Principal Component Analysis (Selecting x-number of components to be used in modeling)
- **Modeling** (Tuning parameter and model selection)
1.Decison Tree (with/without PCA)
2.Random Forest (without PCA)
3.K-Neighbors (PCA)
4.Logistic Regression (PCA)
5.Support Vector Machine (PCA)
- **Summary**

| Model                       | Mean Accuracy | std deviation |
| :---                        |    :----:     |          ---: |
|Decision Tree without PCA    | 94.84         | 0.73            |
|Decision Tree with PCA       | 94.11         | 1.02          |
|Random Forest   without PCA  | 96.48         | 0.3          |
|KNN with PCA                 | 95.48         | 0.56          |
|Logistic Regression with PCA | 94.84         | 0.65          |
|SVM with PCA                 | 94.73         | 0.55          |

Luis Sánchez
-----------

Note: This excersice was based on this one :
https://github.com/ibmsoe/snap-ml/blob/master/notebooks/credit-default-prediction-example.ipynb

