Environment details
1. I used windows 10, I5 9600KF, GTX 1650 super, 16gb RAM and 240gb storage
2. Used jupyter notebook to run the project using python 3
3. Downloaded jupyter notebook and ran it on my above setup using cmd. 
4. The other requirements are listed in the requirement.txt file as asked in the rules.

NOTE:
The upload option only allows 20mb of upload but the datasets provided to us were 133mb even in
.zip format. So i couldn't provide those. So you would have to use those on your own or you can
email me if you require them as  i cannot upload it in the submission window due to the upload limit.

Instructions:
Data pre-processing:
I used the metadata provided directly and removed few values and features while training my model
based on my observation, visualisation graphs and results. Those details are properly documented in the
source code provided in form of a jupyter notebook as well as .txt format. Preferably use jupyter notebook
for testing. 
I took the average of the the image pixel data, description data and title data and added those to a common file
which was used for training the model. The file has been provided.
All the graphs and techniques used are provided in the jupyter notebook file for reference as well.

Features used:
I didn't use 'views' and 'comp_id' for obvious reasons with the training dataset.
The list of features used are:
1.embed
2.ratio
3.duration
4.language
5.partner
6.n_likes
7.n_tags
8.n_formats
9.hour
10.Average(average of pixel data of images)
11.average_d(average of description data)
The features were selected using common logic, graphs, results from testing and observations.

After setting up the files, data pre processing and feature extraction, i tested several machine learning models 
Some of the test ones include XGBoost, Random Forest, Linear Regression and SVM regression
Finally, I came to the conclusion that Linear Regression was based for the given dataset(based on
my knowledge). The model was imported from sklearn library.

Then i trained the model using the code i have provided.

I removed fractional and negative values as they were not suitable for us. Also, based on my observation
and 25% percentile of views training set, I found that minimum views should be 70.
So i converted all values computed which were less than 70 to 70. This was meant to remove errors
due to errors in dataset and get a more logical and understandable result.

Finally, I saved the file on a .csv format using the code provided in the format as given.
I used pandas dataframe method to achieve this task.

To reproduce the results:
(preferably use jupyter notebook code as that is properly formatted and my used platform as well)
1. Set the environment as listed above
2. Open the jupyter notebook/source code provided
3. Give the import location of the training dataset and testing dataset as mentioned in the code
4. All details have been mentioned in the code with appropriate comments.
5. Run the code after this.
6. You will get the solution.txt file in the directory or you can change location or name according to your requirements.
7. The solution.csv file can be used to do analysis and testing after that.

I have provided my submitted solution.csv as well for reference purpose.

I have explained and answered all questions as were asked to the best of my ability. If i have missed anything or there are certain
issues you can contact me. I have tried my best to explain my model building process as well. Though some minor error might have crept in
during the documentation process. If that is the case or there are any questions, feedbacks etc feel free to contact me.

My details are:

Email - aaryan2134@gmail.com
Phone number - +91-9650362429

Thank you!
