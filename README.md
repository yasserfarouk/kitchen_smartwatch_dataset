Title of Database: KDDI Smartwatch Kitchen Dataset
2. Sources:
   (a) Creators: Yasser Mohammad (yasserm@aun.edu.eg), Kazunori Matsumoto (matsu@kddi-research.jp), and Keiichiro Hoashi (hoashi@kddi-research.jp)
            KDDI Research Inc.
   (b) Donor of database: KDDI Research Inc.
   (c) Date received: October 19th 2017
3. Past Usage:
   - Y. Mohammad, K. Matsumoto and K. Hoashi, "A dataset for activity recognition in an unmodified kitchen using smart-watch accelerometers", The 16th International Conference on Mobile and Ubiquitous Multimedia (MUM 2017), Nov. 26-29, 2017, Stuttgart, Germany
    - Predicted activity on left and right hands using accelerometer data from smart watchs worn on both arms
      Best result used a deep convolutional neural network achieving an F1 value of 0.975 for within-session random split evaluation, 0.753 for personal evaluation with no overlap between training and test sets, and 0.680 for leave-one-person-out cross validation (interpersnal evaluation)
4. Relevant Information Paragraph:
   -- The dataset contains accelerometer data recorded using two smartwatchs (SONY smart watch 3) worn by 10 subjects while preparing two meals. Data was manually labeled with each activity on each hand at every second by a professional company leading to 74 different activities. A total of 40 sessions are available. Sampling frequency was 64Hz. After removing rare activities, 20 activities were finally used by the classifiers. To make it possible to combine data from both arms, we interpolated the records to synchronize data from both arms.
5. Number of Instances: 1580070
6. Number of Attributes: 12 
7. Attribute Information:
      -For left arm (cooking-clean-interpolated-left.csv):
          subject (int): Subject from 0 to 9
          class (int): activity (20 different codes). For details on these classes see (class_stats_interpolated-left.csv)
          timestep (int): Time in ms 
          x, y, z (float): acceleration
      -For right arm (cooking-clean-interpolated-right.csv):
          subject (int): Subject from 0 to 9
          class (int): activity (28 different codes). For details on these classes see (class_stats_interpolated-right.csv)
          timestep (int): Time in ms 
          x, y, z (float): acceleration

8. Missing Attribute Values: None
9. Class Distribution: 
Left arm
class,count,mean              ,std               ,min  ,25%   ,50%  ,75%   ,max   ,total             
4    ,67.0 ,204.67164179104478,139.0945163788193 ,2.0  ,68.0  ,194.0,257.5 ,522.0 ,13713.0           
5    ,31.0 ,286.83870967741933,181.41648156919547,51.0 ,66.5  ,319.0,511.5 ,520.0 ,8892.0            
6    ,115.0,69.07826086956521 ,20.686951487862455,4.0  ,63.0  ,65.0 ,66.0  ,137.0 ,7944.0
14   ,232.0,87.66810344827586 ,69.38622204281285 ,1.0  ,64.0  ,65.0 ,67.0  ,393.0 ,20339.0           
16   ,170.0,72.46470588235294 ,24.257529574077488,53.0 ,64.0  ,65.0 ,66.0  ,258.0 ,12319.0           
18   ,309.0,103.24271844660194,75.75226189491929 ,2.0  ,64.0  ,66.0 ,127.0 ,327.0 ,31902.0           
20   ,230.0,69.52608695652174 ,24.890444973860397,4.0  ,63.0  ,65.0 ,66.0  ,259.0 ,15991.0           
22   ,225.0,210.67111111111112,174.95100924236084,43.0 ,127.0 ,130.0,260.0 ,1172.0,47401.0           
23   ,42.0 ,264.1904761904762 ,155.53138466046607,65.0 ,129.25,259.5,326.0 ,522.0 ,11096.0           
26   ,39.0 ,215.2051282051282 ,76.50186770584841 ,118.0,130.0 ,195.0,261.0 ,326.0 ,8393.0            
35   ,144.0,106.82638888888889,38.5987662147672  ,58.0 ,65.0  ,127.0,130.0 ,196.0 ,15383.0           
39   ,100.0,153.36            ,90.16444236319921 ,1.0  ,65.0  ,130.5,250.75,327.0 ,15336.0
40   ,81.0 ,236.82716049382717,298.2273373671274 ,63.0 ,129.0 ,136.0,195.0 ,2149.0,19183.0           
42   ,53.0 ,415.35849056603774,213.45212887379392,10.0 ,198.0 ,567.0,586.0 ,775.0 ,22014.0           
43   ,45.0 ,824.0666666666667 ,279.1392125803897 ,446.0,705.0 ,769.0,910.0 ,1301.0,37083.0           
44   ,47.0 ,613.7021276595744 ,260.20108569215205,128.0,509.0 ,575.0,894.5 ,978.0 ,28844.0           
49   ,55.0 ,255.38181818181818,135.45321604662524,126.0,130.0 ,196.0,322.0 ,521.0 ,14046.0           
62   ,29.0 ,431.44827586206895,226.80381487829902,5.0  ,194.0 ,576.0,637.0 ,655.0 ,12512.0           
72   ,19.0 ,521.0526315789474 ,193.89615596562405,320.0,323.0 ,587.0,709.0 ,718.0 ,9900.0            
74   ,435.0,211.23218390804598,180.0485440776521 ,1.0  ,127.0 ,186.0,259.0 ,1105.0,91886.0   

Right arm
class,count,mean              ,std               ,min  ,25%   ,50%   ,75%   ,max   ,total   
5    ,28.0 ,292.85714285714283,139.8413689349774 ,67.0 ,130.0 ,322.0 ,447.5 ,456.0 ,8200.0  
10   ,96.0 ,128.83333333333334,75.53300661114515 ,63.0 ,66.0  ,129.0 ,130.0 ,391.0 ,12368.0 
12   ,40.0 ,193.575           ,156.0548699525184 ,1.0  ,66.75 ,129.0 ,305.75,456.0 ,7743.0  
14   ,187.0,80.32620320855615 ,37.24527115861711 ,1.0  ,64.0  ,65.0  ,67.0  ,198.0 ,15021.0 
15   ,197.0,65.30964467005076 ,11.2086227000591  ,8.0  ,64.0  ,65.0  ,66.0  ,133.0 ,12866.0 
18   ,214.0,107.57943925233644,76.369258296972   ,2.0  ,64.0  ,65.5  ,130.0 ,327.0 ,23022.0 
19   ,209.0,63.6267942583732  ,7.419079468140393 ,2.0  ,64.0  ,65.0  ,65.0  ,75.0  ,13298.0 
22   ,191.0,208.92146596858638,148.61815823727468,60.0 ,128.0 ,190.0 ,257.0 ,782.0 ,39904.0 
23   ,29.0 ,271.44827586206895,169.6825999596424 ,124.0,130.0 ,194.0 ,511.0 ,521.0 ,7872.0  
26   ,39.0 ,215.23076923076923,76.63394243808183 ,122.0,130.5 ,196.0 ,261.0 ,328.0 ,8394.0  
27   ,38.0 ,258.2631578947368 ,149.16319454199953,128.0,129.25,253.5 ,446.5 ,649.0 ,9814.0  
28   ,118.0,66.19491525423729 ,8.663962570824863 ,59.0 ,64.0  ,65.0  ,66.0  ,130.0 ,7811.0  
35   ,99.0 ,114.4949494949495 ,39.1283533445583  ,62.0 ,65.0  ,129.0 ,130.0 ,196.0 ,11335.0 
37   ,39.0 ,218.15384615384616,116.57063331134172,61.0 ,129.5 ,195.0 ,261.5 ,392.0 ,8508.0  
39   ,61.0 ,199.7377049180328 ,94.7915083467122  ,3.0  ,129.0 ,195.0 ,260.0 ,326.0 ,12184.0 
40   ,82.0 ,243.8048780487805 ,258.39573626343133,2.0  ,130.0 ,191.0 ,205.5 ,1690.0,19992.0 
42   ,61.0 ,640.8852459016393 ,504.22776263512293,8.0  ,258.0 ,577.0 ,649.0 ,2016.0,39094.0 
43   ,50.0 ,803.0             ,290.80668942141773,8.0  ,699.75,770.0 ,910.0 ,1301.0,40150.0 
44   ,53.0 ,616.377358490566  ,261.33232794920303,126.0,388.0 ,583.0 ,897.0 ,977.0 ,32668.0 
47   ,245.0,389.8857142857143 ,334.5318407252385 ,3.0  ,129.0 ,324.0 ,521.0 ,1365.0,95522.0 
49   ,75.0 ,243.94666666666666,142.57912865468046,122.0,130.0 ,193.0 ,260.0 ,521.0 ,18296.0 
52   ,59.0 ,201.33898305084745,195.4755130770631 ,4.0  ,64.0  ,65.0  ,390.0 ,651.0 ,11879.0 
53   ,77.0 ,184.94805194805195,103.01786969462299,2.0  ,128.0 ,192.0 ,252.0 ,391.0 ,14241.0 
61   ,267.0,986.2509363295881 ,1182.2758513451638,11.0 ,195.5 ,576.0 ,1559.0,5461.0,263329.0
62   ,31.0 ,674.7741935483871 ,401.23938903331504,5.0  ,584.0 ,640.0 ,831.5 ,2469.0,20918.0 
71   ,19.0 ,624.4736842105264 ,168.85640461681328,446.0,453.5 ,765.0 ,773.0 ,845.0 ,11865.0 
73   ,19.0 ,882.9473684210526 ,253.8891870447531 ,307.0,704.5 ,1021.0,1040.0,1496.0,16776.0 
74   ,304.0,191.82236842105263,128.6760509910935 ,2.0  ,127.0 ,131.0 ,259.0 ,845.0 ,58314.0 
     