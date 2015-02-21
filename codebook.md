### Code book for tidy_dataset.txt
 CREATED BY : Vinay Tyagi 
- for coursera Getting and Cleaning data - signature track - data science.

---

The project goal is to create a tidy dataset using the supplied dataset with following 
steps.  

* Merges the training and the test sets to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement. 
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names. 
* Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 

The final tidy dataset contains the result of above activities.

* The tidy narrow dataset contains 5 variables 

column        : 1

Variable name : Activity label 

type          : numeric 

values        : 1, 2, 3, 4, 5, 6

length        : 1

the values are corresponding to the next variable called activity names.
there are 6 activity named as follows 

1 WALKING

2 WALKING_UPSTAIRS

3 WALKING_DOWNSTAIRS

4 SITTING

5 STANDING

6 LAYING

---


column        : 2

Variable name : Activity names

type          : character 

values        : WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING

length        : as indicated in the values


This column value is corresponding to column 1 
the purpose of of this column to include the description and the first column can be used
for sorting and analysis purpose where the descriptive names are not necessary.

---

column        : 3

variable name : subject

type          : numeric

values        : 1 to 30

length        : 2


This variable holds the 30 different persons id who contributed for the observation.
all activities are conducted by all the participants hence the 30 participants with 
6 different activities are captured.

---
column        : 4 

variable name : mean_and_std_variables

type          : character

values        : 66 different values as described below

length        : as indicated in the values


This is the subset of 563 variables which contains the mean or std with reference to the mean and standard deviation values obtained and supplied for the project.

The list of values : 

1             tBodyAcc.mean.X

2             tBodyAcc.mean.Y

3             tBodyAcc.mean.Z

4              tBodyAcc.std.X

5              tBodyAcc.std.Y

6              tBodyAcc.std.Z

7        tGravityAcc.mean.X

8         tGravityAcc.mean.Y

9         tGravityAcc.mean.Z

10          tGravityAcc.std.X

11         tGravityAcc.std.Y

12         tGravityAcc.std.Z

13       tBodyAccJerk.mean.X

14        tBodyAccJerk.mean.Y

15        tBodyAccJerk.mean.Z

16         tBodyAccJerk.std.X

17         tBodyAccJerk.std.Y

18         tBodyAccJerk.std.Z

19          tBodyGyro.mean.X

20          tBodyGyro.mean.Y

21          tBodyGyro.mean.Z

22           tBodyGyro.std.X

23           tBodyGyro.std.Y

24           tBodyGyro.std.Z

25      tBodyGyroJerk.mean.X

26      tBodyGyroJerk.mean.Y

27      tBodyGyroJerk.mean.Z

28       tBodyGyroJerk.std.X

29       tBodyGyroJerk.std.Y

30      tBodyGyroJerk.std.Z

31          tBodyAccMag.mean

32           tBodyAccMag.std

33       tGravityAccMag.mean

34        tGravityAccMag.std

35      tBodyAccJerkMag.mean

36       tBodyAccJerkMag.std

37         tBodyGyroMag.mean

38          tBodyGyroMag.std

39     tBodyGyroJerkMag.mean

40      tBodyGyroJerkMag.std

41           fBodyAcc.mean.X

42           fBodyAcc.mean.Y

43           fBodyAcc.mean.Z

44            fBodyAcc.std.X

45            fBodyAcc.std.Y

46            fBodyAcc.std.Z

47       fBodyAccJerk.mean.X

48       fBodyAccJerk.mean.Y

49       fBodyAccJerk.mean.Z

50        fBodyAccJerk.std.X

51        fBodyAccJerk.std.Y

52        fBodyAccJerk.std.Z

53          fBodyGyro.mean.X

54          fBodyGyro.mean.Y

55          fBodyGyro.mean.Z

56           fBodyGyro.std.X

57           fBodyGyro.std.Y

58           fBodyGyro.std.Z

59          fBodyAccMag.mean

60           fBodyAccMag.std

61  fBodyBodyAccJerkMag.mean

62   fBodyBodyAccJerkMag.std

63     fBodyBodyGyroMag.mean

64      fBodyBodyGyroMag.std

65 fBodyBodyGyroJerkMag.mean

66  fBodyBodyGyroJerkMag.std



The following description is from the original dataset is given to understand the naming.

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ

tGravityAcc-XYZ

tBodyAccJerk-XYZ

tBodyGyro-XYZ

tBodyGyroJerk-XYZ

tBodyAccMag

tGravityAccMag

tBodyAccJerkMag

tBodyGyroMag

tBodyGyroJerkMag

fBodyAcc-XYZ

fBodyAccJerk-XYZ

fBodyGyro-XYZ

fBodyAccMag

fBodyAccJerkMag

fBodyGyroMag

fBodyGyroJerkMag


The set of variables that were estimated from these signals are: 


mean(): Mean value

std(): Standard deviation

Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable 

gravityMean

tBodyAccMean

tBodyAccJerkMean

tBodyGyroMean

tBodyGyroJerkMean

---


column        : 5

Variable name : average

type          : numeric 

length        : double precision average values


This variable contains the average calculated from the main data set for each subject, activity, and the mean_and_std_variables from the large dataset supplied for the project.


