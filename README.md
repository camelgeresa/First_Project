# My first_Project
Dengue fever is a mosquito-borne tropical disease caused by the dengue virus. Symptoms typically begin three to fourteen days after infection. These may include a high fever, headache, vomiting, muscle and joint pains, and a characteristic skin itching and skin rash. Since this virus is carried by mosquitos, we can try predict the number of cases depending on variables such as temperature, which may influence the dispersion of these mosquitos. Here, I used data from data driven https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/page/82/, to predict the number of cases in San Juan and Iquitos. 
I tried a variety of models including linear regression, lasso regression and decision trees, however xgboost, used with feature selection and hyperparameter optimisation gave the best results (MAE=7.4).
Some interesting findings from EDA:

![image](https://user-images.githubusercontent.com/99748864/174491669-07fb7ca6-db37-4eba-b39b-8de475aa6dc7.png)

San Juan tends to have more cases, with the median values slightly increasing and upper quartiles increasing greatly, with there being many more days with an extremely high number of cases, between August and October, which makes sense as these are the months where the temperature is highest. 
Interestingly, the higher the minimum temperature was, the higher the number of cases was likely to be. However, the maximum temperature had the oppsoite effect, with a higher maximum temperature actually leading to a decrease in cases. It seems mosquitos have an optimum temperature, so that the minimum temperature is high enough for them to work optimally but also not too hot.
![image](https://user-images.githubusercontent.com/99748864/174492350-3b0b4965-7489-46b9-8958-ad70059cb80e.png)

The same applies with precipitation, where cases peak for a certain precipation, but deviations away from that value lead to a drop in cases.

![image](https://user-images.githubusercontent.com/99748864/174492539-95ab71e7-c580-403a-9e2f-c304662b44f3.png)
