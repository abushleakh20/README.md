Code Book
The source is https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip. For creating "tidy data", only mean and standard deviation values as well as labels of actvities and features are taken over and merged from the source. Finally, the average of each variable (grouped by activity and subject) is calculted and stored in the file "tidy_data.txt".

Description
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix ‘t’ to denote time) were captured at a constant rate of 50 Hz. and the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) – both using a low pass Butterworth filter.

The body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag).

A Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the ‘f’ to indicate frequency domain signals).

Description of abbreviations of measurements
Leading t or f is based on time or frequency measurements.

Body = related to body movement.
Gravity = acceleration of gravity
Acc = accelerometer measurement
Gyro = gyroscopic measurements
Jerk = sudden movement acceleration
Mag = magnitude of movement
mean and std (=standard deviation) are calculated for each subject for each activity for each mean and SD measurements.

Fields
ID Fields
1 subjectId - The participant ("subject") ID
2 activity - The label of the activity performed when the corresponding measurements were taken. This variable covers 6 different activities:
WALKING (value 1): Subject was walking during the test.
WALKING_UPSTAIRS (value 2): subject was walking up a staircase during the test.
WALKING_DOWNSTAIRS (value 3): subject was walking down a staircase during the test.
SITTING (value 4): subject was sitting during the test.
STANDING (value 5): subject was standing during the test.
LAYING (value 6): subject was laying down during the test.
Extracted Feature Fields
3 tBodyAccMeanX (from column of source 1)
4 tBodyAccMeanY (from column of source 2)
5 tBodyAccMeanZ (from column of source 3)
6 tBodyAccStdX (from column of source 4)
7 tBodyAccStdY (from column of source 5)
8 tBodyAccStdZ (from column of source 6)
9 tGravityAccMeanX (from column of source 41)
10 tGravityAccMeanY (from column of source 42)
11 tGravityAccMeanZ (from column of source 43)
12 tGravityAccStdX (from column of source 44)
13 tGravityAccStdY (from column of source 45)
14 tGravityAccStdZ (from column of source 46)
15 tBodyAccJerkMeanX (from column of source 81)
16 tBodyAccJerkMeanY (from column of source 82)
17 tBodyAccJerkMeanZ (from column of source 83)
18 tBodyAccJerkStdX (from column of source 84)
19 tBodyAccJerkStdY (from column of source 85)
20 tBodyAccJerkStdZ (from column of source 86)
21 tBodyGyroMeanX (from column of source 121)
22 tBodyGyroMeanY (from column of source 122)
23 tBodyGyroMeanZ (from column of source 123)
24 tBodyGyroStdX (from column of source 124)
25 tBodyGyroStdY (from column of source 125)
26 tBodyGyroStdZ (from column of source 126)
27 tBodyGyroJerkMeanX (from column of source 161)
28 tBodyGyroJerkMeanY (from column of source 162)
29 tBodyGyroJerkMeanZ (from column of source 163)
30 tBodyGyroJerkStdX (from column of source 164)
31 tBodyGyroJerkStdY (from column of source 165)
32 tBodyGyroJerkStdZ (from column of source 166)
33 tBodyAccMagMean (from column of source 201)
34 tBodyAccMagStd (from column of source 202)
35 tGravityAccMagMean (from column of source 214)
36 tGravityAccMagStd (from column of source 215)
37 tBodyAccJerkMagMean (from column of source 227)
38 tBodyAccJerkMagStd (from column of source 228)
39 tBodyGyroMagMean (from column of source 240)
40 tBodyGyroMagStd (from column of source 241)
41 tBodyGyroJerkMagMean (from column of source 253)
42 tBodyGyroJerkMagStd (from column of source 254)
43 fBodyAccMeanX (from column of source 266)
44 fBodyAccMeanY (from column of source 267)
45 fBodyAccMeanZ (from column of source 268)
46 fBodyAccStdX (from column of source 269)
47 fBodyAccStdY (from column of source 270)
48 fBodyAccStdZ (from column of source 271)
49 fBodyAccMeanFreqX (from column of source 294)
50 fBodyAccMeanFreqY (from column of source 295)
51 fBodyAccMeanFreqZ (from column of source 296)
52 fBodyAccJerkMeanX (from column of source 345)
53 fBodyAccJerkMeanY (from column of source 346)
54 fBodyAccJerkMeanZ (from column of source 347)
55 fBodyAccJerkStdX (from column of source 348)
56 fBodyAccJerkStdY (from column of source 349)
57 fBodyAccJerkStdZ (from column of source 350)
58 fBodyAccJerkMeanFreqX (from column of source 373)
59 fBodyAccJerkMeanFreqY (from column of source 374)
60 fBodyAccJerkMeanFreqZ (from column of source 375)
61 fBodyGyroMeanX (from column of source 424)
62 fBodyGyroMeanY (from column of source 425)
63 fBodyGyroMeanZ (from column of source 426)
64 fBodyGyroStdX (from column of source 427)
65 fBodyGyroStdY (from column of source 428)
66 fBodyGyroStdZ (from column of source 429)
67 fBodyGyroMeanFreqX (from column of source 452)
68 fBodyGyroMeanFreqY (from column of source 453)
69 fBodyGyroMeanFreqZ (from column of source 454)
70 fBodyAccMagMean (from column of source 503)
71 fBodyAccMagStd (from column of source 504)
72 fBodyAccMagMeanFreq (from column of source 513)
73 fBodyBodyAccJerkMagMean (from column of source 516)
74 fBodyBodyAccJerkMagStd (from column of source 517)
75 fBodyBodyAccJerkMagMeanFreq (from column of source 526)
76 fBodyBodyGyroMagMean (from column of source 529)
77 fBodyBodyGyroMagStd (from column of source 530)
78 fBodyBodyGyroMagMeanFreq (from column of source 539)
79 fBodyBodyGyroJerkMagMean (from column of source 542)
80 fBodyBodyGyroJerkMagStd (from column of source 543)
81 fBodyBodyGyroJerkMagMeanFreq (from column of source 552)
