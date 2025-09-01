# Detecting Colon Cancer

## Dataset Link: https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images

## Kaggle Notebook: https://www.kaggle.com/code/shasan7/detecting-colon-cancer

The images were transformed and normalized using torch, then we fed them to the **pretrained DeiT-base model for fine-Tuning**

**The best validation accuracy achieved by our model is 100%**.

Training Summary:

    Epoch	Training Loss	Validation Loss	Accuracy	Precision	Recall	      F1
        1	0.125900	    0.000314	    1.000000	1.000000	1.000000	1.000000
        2	0.000000	    0.000023	    1.000000	1.000000	1.000000	1.000000
        3	0.000000	    0.000016	    1.000000	1.000000	1.000000	1.000000
        4	0.000000	    0.000015	    1.000000	1.000000	1.000000	1.000000
        5	0.000000	    0.000011	    1.000000	1.000000	1.000000	1.000000
        6	0.000000	    0.000012	    1.000000	1.000000	1.000000	1.000000
        7	0.000000	    0.000012	    1.000000	1.000000	1.000000	1.000000
        8	0.000000	    0.000011	    1.000000	1.000000	1.000000	1.000000
        9	0.000000	    0.000010	    1.000000	1.000000	1.000000	1.000000
       10	0.000000	    0.000011	    1.000000	1.000000	1.000000	1.000000


Obtained Results:

    Classification Report:

                  precision    recall  f1-score   support
    
       colon_aca       1.00      1.00      1.00      1012
         colon_n       1.00      1.00      1.00       988
    
        accuracy                           1.00      2000
       macro avg       1.00      1.00      1.00      2000
    weighted avg       1.00      1.00      1.00      2000


![Confusion Matrix: ](Conf_Mat.png)

![Accuracy Curve: ](Acc.png)

![Loss_Curve): ](Loss.png)
