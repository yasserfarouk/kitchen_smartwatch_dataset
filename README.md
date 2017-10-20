KDDI Smartwatch Kitchen Dataset
===============================
The dataset contains accelerometer data recorded using two smartwatchs (SONY smart watch 3) worn by 10 subjects while preparing two meals. Data was manually labeled with each activity on each hand at every second by a professional company leading to 74 different activities. A total of 40 sessions are available. Sampling frequency was 64Hz. After removing rare activities, 20 activities were finally used by the classifiers. To make it possible to combine data from both arms, we interpolated the records to synchronize data from both arms. Please check the license file before use.

Creators:
--------
   Yasser Mohammad (yasserm@aun.edu.eg), Kazunori Matsumoto (matsu@kddi-research.jp), and Keiichiro Hoashi (hoashi@kddi-research.jp), KDDI Research Inc.

Citation Request:
----------------
Any publications resulting from the use in any way of the dataset MUST explicitly site the following publication:

- Y. Mohammad, K. Matsumoto and K. Hoashi, "A dataset for activity recognition in an unmodified kitchen using smart-watch accelerometers", The 16th International Conference on Mobile and Ubiquitous Multimedia (MUM 2017), Nov. 26-29, 2017, Stuttgart, Germany

Past Usage:
-----------
   - Y. Mohammad, K. Matsumoto and K. Hoashi, "A dataset for activity recognition in an unmodified kitchen using smart-watch accelerometers", The 16th International Conference on Mobile and Ubiquitous Multimedia (MUM 2017), Nov. 26-29, 2017, Stuttgart, Germany
   - Predicted activity on left and right hands using accelerometer data from smart watchs worn on both arms
      Best result used a deep convolutional neural network achieving an F1 value of 0.975 for within-session random split evaluation, 0.753 for personal evaluation with no overlap between training and test sets, and 0.680 for leave-one-person-out cross validation (interpersnal evaluation)

Relevant Information:
-------------------- 
**Number of Instances**: 1580070

**Number of Attributes**: 12 

**Missing Attribute Values**: None

Attribute Information:
----------------------
      - *For left arm (cooking-clean-interpolated-left.csv)* :
          subject (int): Subject from 0 to 9
          class (int): activity (20 different codes). For details on these classes see (class_stats_interpolated-left.csv)
          timestep (int): Time in ms 
          x, y, z (float): acceleration
      - *For right arm (cooking-clean-interpolated-right.csv)* :
          subject (int): Subject from 0 to 9
          class (int): activity (28 different codes). For details on these classes see (class_stats_interpolated-right.csv)
          timestep (int): Time in ms 
          x, y, z (float): acceleration
