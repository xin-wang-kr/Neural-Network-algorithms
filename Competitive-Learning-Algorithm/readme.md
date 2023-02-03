## Kohonen Self-Organizing Maps (SOM)
I designed the Kohonen SOM with 4 input units and 1 dim grid of 3 Kohonen neurons as output units. The initial weight is randomly generated. The initial radius is set as 1.5 and the radius decays exponentially as the training epochs. Three different initial learning rates (0.9, 0.5, 0.1) were applied. The learning rate decreases linearly. The model was trained in 1000 epochs. To perform smooth Euclidean distance calculation, data normalization was performed before training and testing. Figure 1 shows the grouping result in the training set by the trained network. Figure 1 is given when the initial learning rate is equal to 0.9.

<img width="671" alt="image" src="https://user-images.githubusercontent.com/28020765/216693185-7fdf057f-86c8-4563-8ac0-c878ddf92d89.png">

Figure 1 is plotted through the projection on column 0 and column 2 named in the dataset. It is obvious to see that totally 6 points are assigned in the wrong groups, which happened in the area for variable 0 is equal to 0 and variable 2 is equal to about 0.5. 
The trained network is further tested on testing set. Figure 2 shows the grouping result for the testing set.

<img width="693" alt="image" src="https://user-images.githubusercontent.com/28020765/216693457-c1b20dc7-1836-4cec-a60e-61c485eafcb0.png">

Figure 2 shows the comparison between the actual grouping and the predicted grouping by trained network. The wrongly clustered points appeared in the area where variable 0 is equal to 0 and variable 2 is equal to 0.5. In Figure 2, there are totally 6 wrongly clustered points in the grouping result on testing set. In general, the trained network can correctly group most points. 

## Learning Vector Quantization (LVQ)
I designed LVQ network with 4 input units and multiple classification units. The number of output neurons was set greater than and equal to 3. In the experiment, the different numbers of output neurons, including 3, 9, and 20, were applied. Three different initial learning rates (0.9, 0.5, 0.1) were also applied. Figure 3 shows the grouping result for the training set by the trained network.

<img width="704" alt="image" src="https://user-images.githubusercontent.com/28020765/216694121-3d70ea93-c80e-43da-813f-18c3f67f64e9.png">

Figure 7 is given by the trained network by 2000 epochs with the initial learning rate of 0.9. Compared to the actual grouping on training set, much more points are wrongly grouped. Even at the bottom, a few points are wrongly grouped in the separated area. Through checking and counting the predicted result, it is found that there are totally 35 instances are wrongly grouped in training set. The accuracy rate achieved 0.67. 

<img width="698" alt="image" src="https://user-images.githubusercontent.com/28020765/216694324-0b7c9c59-43c6-4e87-a6d0-9bb8cef4065c.png">

Figure 8 shows the predicted grouping result given by the network trained with 20 output neurons and an initial learning rate of 0.9. It is obvious to see that many wrong groupings happened. From the projection of Figure 8, there are about 22 points appearing in the wrong groups. Through checking and counting the predicted result, it is found that there are totally 25 instances are wrongly grouped in testing set. The accuracy rate achieved 0.44.

