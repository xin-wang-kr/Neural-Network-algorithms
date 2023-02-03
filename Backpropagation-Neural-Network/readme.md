A neural network was firstly trained with training dataset size of 30. Error metrices, including mean squared error (MSE), mean absolute error (MAE), root mean squared error (RMSE), and R2 value, were calculated. Figure 6 shows that the changes of error metrices during training process. 

<img width="468" alt="image" src="https://user-images.githubusercontent.com/28020765/216695214-9ef4b5a3-af52-4b07-b0e0-396b13576f03.png">
Figure 6. Training process on dataset of size of 30

Figure 6 indicates that MSE, MAE, and RMSE kept decreasing, as the number of epochs increased. Only the R2 score shows the increasing tendency. All the turning points for these four parameters happened between 0 to 200 epochs. After that, the curves level off.

Another neural network was also trained with training dataset size of 300. Figure 7 visualized the error metric changes during the training process. It is obvious to see that the MAE decreased much more compared to the case of the training dataset size of 30. The MAE in this cased decreased from 23 to 13, which it only reduced 0.15 in the case of the training dataset size of 30.

<img width="468" alt="image" src="https://user-images.githubusercontent.com/28020765/216695441-505c344c-a985-4e20-8e8b-c5630aa33241.png">
Figure 7. Training process on dataset of size of 300

These two neural networks were tested on the dataset of size 500. Table 3 shows the testing results on both size 30 and size 300. It can be seen clearly that the neural network trained with the dataset of size 300 can achieve lower MSE, ABE, and RMSE. For both training sizes, R2 value got negative value, that means that the model has not fitted the data well enough, and the certain bias might need to be considered. However, due to the limited number of variables and training data, bias was set to 0, as discussed earlier in question 5.

![image](https://user-images.githubusercontent.com/28020765/216697759-3b72c400-6f7e-4318-9ffe-7bc3d986a25e.png)
![image](https://user-images.githubusercontent.com/28020765/216697136-a61db566-fece-47a2-9141-e2944e5c8e2c.png)
