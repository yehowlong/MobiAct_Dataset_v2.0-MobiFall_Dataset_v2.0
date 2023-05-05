===========================MobiFallDatasetv2.0===========================


Filename format:
<ADL OR FALL_CODE>_<SENSOR_CODE>_<SUBJECT_ID>_<TRIAL_NO>.txt


examples:
1 -->	WAL_acc_5_1.txt
2 -->	STD_ori_9_5.txt
3 -->	FKL_gyro_3_2.txt


Subjects:
+----+-------+---------+-----+--------+--------+--------+
| id | Name  | Surname | Age | Height | Weight | Gender |
+----+-------+---------+-----+--------+--------+--------+
| 1  | pat1  | pat1    | 32  | 180    | 85     | M      |
| 2  | pat2  | pat2    | 26  | 169    | 64     | M      |
| 3  | pat3  | pat3    | 26  | 164    | 55     | F      |
| 4  | pat4  | pat4    | 32  | 186    | 93     | M      |
| 5  | pat5  | pat5    | 36  | 160    | 50     | F      |
| 6  | pat6  | pat6    | 22  | 172    | 62     | F      |
| 7  | pat7  | pat7    | 25  | 189    | 80     | M      |
| 8  | pat8  | pat8    | 22  | 183    | 93     | M      |
| 9  | pat9  | pat9    | 30  | 177    | 102    | M      |
| 10 | pat10 | pat10   | 26  | 170    | 90     | F      |
| 11 | Pat11 | pat11   | 26  | 168    | 80     | F      |
| 12 | sub12 | sub12   | 29  | 178    | 83     | M      |
| 13 | sub13 | sub13   | 24  | 177    | 62     | M      |
| 14 | sub14 | sub14   | 24  | 178    | 85     | M      |
| 15 | sub15 | sub15   | 25  | 173    | 82     | M      |
| 16 | sub16 | sub16   | 27  | 172    | 56     | F      |
| 17 | sub17 | sub17   | 25  | 173    | 67     | M      |
| 18 | sub18 | sub18   | 25  | 176    | 73     | M      |
| 19 | sub19 | sub19   | 25  | 161    | 63     | F      |
| 20 | sub20 | sub20   | 26  | 178    | 71     | M      |
| 21 | sub21 | sub21   | 25  | 180    | 70     | M      |
| 29 | sub29 | sub29   | 27  | 186    | 103    | M      |
| 30 | sub30 | sub30   | 47  | 172    | 90     | M      |
| 31 | sub31 | sub31   | 27  | 170    | 75     | M      |
+----+-------+---------+-----+--------+--------+--------+


Activities of Daily Living:
+----+------+--------------+--------+----------+--------------------------------+
| id | Code | Activity     | Trials | Duration | Description                    |
+----+------+--------------+--------+----------+--------------------------------+
| 1  | STD  | Standing     | 1      | 5m       | Standing with subtle movements |
| 2  | WAL  | Walking      | 1      | 5m       | Normal walking                 |
| 3  | JOG  | Jogging      | 3      | 30s      | Jogging                        |
| 4  | JUM  | Jumping      | 3      | 30s      | Continuous jumping             |
| 5  | STU  | Stairs up    | 6      | 10s      | Stairs up (10 stairs)          |
| 6  | STN  | Stairs down  | 6      | 10s      | Stairs down (10 stairs)        |
| 7  | SCH  | Sit chair    | 6      | 6s       | Sitting on a chair             |
| 8  | CSI  | Car-step in  | 6      | 6s       | Step in a car                  |
| 9  | CSO  | Car-step out | 6      | 6s       | Step out a car                 |
+----+------+--------------+--------+----------+--------------------------------+


Falls:
+----+------+--------------------+--------+----------+---------------------------------------------------------+
| id | Code | Activity           | Trials | Duration | Description                                             |
+----+------+--------------------+--------+----------+---------------------------------------------------------+
| 10 | FOL  | Forward-lying      | 3      | 10s      | Fall Forward from standing, use of hands to dampen fall |
| 11 | FKL  | Front-knees-lying  | 3      | 10s      | Fall forward from standing, first impact on knees       |
| 12 | BSC  | Back-sitting-chair | 3      | 10s      | Fall backward while trying to sit on a chair            |
| 13 | SDL  | Sideward-lying     | 3      | 10s      | Fall sidewards from standing, bending legs              |
+----+------+--------------------+--------+----------+---------------------------------------------------------+


Sensors:
+------+---------------+----------------------------------------------------+--------------------------------------------------------------+
| Code | Type          | Values                                             | Description                                                  |
+------+---------------+----------------------------------------------------+--------------------------------------------------------------+
| acc  | accelerometer | timestamp(ns),x,y,z(m/s^2)                         | Acceleration force along the x y z axes (including gravity). |
| gyro | gyroscope     | timestamp(ns),x,y,z(rad/s)                         | Rate of rotation around the x y z axes (Angular velocity).   |
| ori  | orientation   | timestamp(ns),Azimuth,Pitch,Roll(degrees)          | Angle around the z x y axes.                                 |
+------+---------------+----------------------------------------------------+--------------------------------------------------------------+

=================================CHANGES=======================================

v2.0 subjects added with only falls performed 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 29, 30, 31
