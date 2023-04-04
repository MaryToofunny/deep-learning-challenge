# deep-learning-challenge


## Overview
This project tried to predict whether applicants will be successful if funded by the Alphabet Soup Co. Alphabet Soup Co. wants to provide funding to companies but it needs to know in advance whether it will be successful or not. Money is on the line here and we would not want for it to go to waste. 

For this I will create a neural network by using Data Manipulation, creating training and testing sets, and finally analyzing my models that I have created.  


## Results
- **Data Processing**
   - To clean the data I removed the EIN and NAME columns since they have no value to the model. 
   - The varibales being considered for my model are as follows: 'STATUS', 'ASK_AMT', 'IS_SUCCESSFUL', 'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT'. I dropped "USE_CASE_Other","AFFILIATION_Other" columns. 
   - My Dependent varible is "IS_SUCCESFUL" since we want to try to predict this with high accuracy. 
   


- **Compiling, Training, and Evaluating the Model**
  **Attempt #1**
   - 2 Hidden Layers
   - 80 neurons (Layer1), 30 neurons(Layer2)
   - Used ReLU and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and LeakyReLU is for nonlinear datasets.
   <img width="661" alt="image" src="https://user-images.githubusercontent.com/116314027/229868907-a1be5cc6-73a9-4a69-9113-6515323e6d9f.png">
 
   
  **Attempt #2**
   - 3 Hidden Layers 
   - 80 neurons (Layer1), 30 neurons(Layer2), 10 neurons(Layer3)
   - Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
   <img width="608" alt="image" src="https://user-images.githubusercontent.com/116314027/229873291-88c8277f-7278-4895-9802-e3d65f53a958.png">

     
  **Attempt #3**
   - used hyperparameter option
   - activation choice of relu,tanh and sigmoid
  
  <img width="631" alt="image" src="https://user-images.githubusercontent.com/116314027/229871028-0881a86d-d228-4ae7-a41c-4ff083fe616d.png">
  
  <img width="796" alt="image" src="https://user-images.githubusercontent.com/116314027/229871337-6019e504-bc93-4541-b5a2-a56d082e68d3.png">

<img width="598" alt="image" src="https://user-images.githubusercontent.com/116314027/229871409-7774ac73-cf69-4d88-8431-994f44d9f5ae.png">


I tried to change my models in order to achieve a more than 75% accuracy rate but only got about 73%. I changed my features, activation functions, Hidden Layers, and the number of neurons in order to achieve this. 
  
## Summary 
On Average my models kept around 73% accuracy score which is decent considering it was an improvement. My recommendation to improve this model would be to find better features to help explain what determines "IS_SUCCESFUL" such as more indepth knowledge of the other associates/ firms being funded. At the end of the day, knowledge is power and if we had more indepth data between all these applications, we can create a better model.
