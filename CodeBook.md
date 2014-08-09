1. Data for the project download from site below as specified in Course Projet assignment:

	https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

2. Ran run_analysis.R script that does the listed activities as required for this project work:

	- 	Read X_train.txt, y_train.txt and subject_train.txt from train folder in my working directory
		and stored each in variables.

	-	Read X_test.txt, y_test.txt and subject_test.txt from test folder in my working directory
		and stored each invariables. 

	-	Concatenated test data to train data to generate required data frame, 
		join data; concatenated test label to train label to generate required data frame, 
		join label;concatenated test subject to train subject to generate required data frame etc.

	-	Read the features.txt file from my working folder and stored data in a variable called features. 
		Extracted measurements on the mean and standard deviation.  

	-	Cleaned column names of the subset. Removed "()" and "-" symbols in the names.
		Also made sure the first letter of "mean" and "std" to capital letter "M" and "S".

	-	Read the activity_labels.txt file from my working folder and store the data in a variable activity.

	-	Cleaned the activity names in the second column of activity. 
		Also if the name has an underscore between letters, removed underscore and made the letter next to
		a capitalized letter.

	-	Transformed values of join label according to the activity data frame.

	-	Combined join subject, join label and join data by column to get a new clean data frame. 
		Properly name the first two columns, "subject" and "activity". 
		
	-	Wrote the cleane dData out to "merged_data.txt" file in my working directory.

	-	Generated second independent tidy data set with the average of each measurement for each activity 
		and each subject. For each subject and activity combinatons, did calculate mean of each measurement
		with corresponding combination to get the desired data frame.

	-	Wrote the result out to "data_with_means.txt" file in my working directory. 