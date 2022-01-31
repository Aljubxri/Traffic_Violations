# Traffic_Violations
## Preprocessing and cleaning - <br>
• Some traffic violations were made by people on foot, however I am only interested in vehicle traffic violations so I removed those. 

• Looking at the counts for each attribute, some information is missing on things like “Geolocation”, "Driver City", "Driver State", "DL State", "Arrest Type", "Geolocation", “Color”, “Article”. This could be seen since the max count is 5906 and the count for those attributes is less than that

• Some missing information is nominal (strings) so I could not fill it, but since this dataset is so big, dropping the rows with the missing values will not have a large effect on it.

• Many of the car manufacturer names have been misspelt, so I had to find all the misspellings and locate them then change them to the correct spellings, this reduced the unique count by about 100!

• The “Time of Stop” has been discretized, because for the information I’m trying to get out of it, having something like Afternoon and Midnight etc. is better than the time down to the seconds. For example: Morning is from 6:00 to 12:00. Afternoon is from 12:01 to around 17:00. etc.

## Machine Learning (Trial and error)-
• I used One-Hot Encoding algorithm on the non-categorical parts then I used K clustering which did not go well for my data.
• I then used logistic regression on the binary and catagorical parts of the data which yeilded good results, however when I used linear regression on the non-categorical datait the results were not the best. 

## Takeaways-
While cleaning data is not supposed to easy, for this project specifically it was time consuming.
Using one hot encoding can give out the wrong data if used incorrectly
When wanting to predict data from a dataset, having a categorical only dataset makes it a lot harder than for example an all numerical dataset, or even a categorical and numerical dataset.
the best choice for predicting categorical data is logistical regression.

## Interesting Analysis takeaways - 
![image](https://user-images.githubusercontent.com/64828238/151828350-b7a55b89-ef34-4955-82d2-b861a9607052.png)
![image](https://user-images.githubusercontent.com/64828238/151828457-4b196ffa-5a88-4448-b69b-8f911cdbaac8.png)


