# Dataset Description
The survey was conducted with 158 participants, and it is composed by three sources of data: (i) Online questionnaire (synchronic); (ii) Time Diaries (diachronic); Sensor data (diachronic).

## Participants
Of the 158 participants, 77 were Female and 81 were Male. Additional information are listed below.

|  | Range | Average |
|-------|--------|---------|
**Age** | 20-26 | 22 |
**N. obs.** | 396-932 | 700 |


## Online questionnaires 
Were used to invite the students, to evaluate the app, and to understand their habits and routine. They are composed by attributes regarding:
1. Socio-demographics: age, gender, students’ accommodation(s) and flat mates
2. Habits about travel, occupation, and university experience
3. Psycho-social profile, concerning:
- personality, collected with a 10-item short version of the [Big Five](https://pdfs.semanticscholar.org/4646/5a97ab883cc72d9f601263a208afae6fb31a.pdf) Inventory-44
- attitude towards procrastination [Irrational Procrastination Scale (IPS)](https://prism.ucalgary.ca/bitstream/handle/1880/47914/Steel_PsychBulletin_2007_Postprint.pdf?sequence=1)
- smartphone habits [Smartphone Addiction Scale (SAV-SV)](https://www.scirp.org/journal/paperinformation.aspx?paperid=78277)
- perceived stress [Perceived Stress Scale](http://www.mindgarden.com/documents/PerceivedStressScale.pdf)

The complete [questionnaire](https://github.com/Gengis-Khan/SU2Dataset/blob/gh-pages/Documentation/SU2-Questionnaire.pdf) and the [codebook](https://github.com/Gengis-Khan/SU2Dataset/blob/gh-pages/Documentation/SU2-Questionnaire_codebook.pdf) can be found at the respective links.

## Time Diaries
Time diaries are a classic data collection tool, where respondents are asked to indicate three main dimensions of their everyday life: the activities performed, the locations they visit, and the people around them. In this case we administered a version, following the [HETUS](https://ec.europa.eu/eurostat/web/time-use-surveys) standard, implemented in the app [iLog](http://datascientia.disi.unitn.it/ilog/). Participants received a notification on their smartphone with four questions (see Figure), namely: 
1. “What are you doing?” 
2. “Where are you?” 
3. “Who is with you?” 
4. “What is your mood?” 

![TD_Labels](https://github.com/Gengis-Khan/SU2Dataset/blob/gh-pages/images/TD_Labels.png)

*Time Diaries labels*

During the month of data collection, time diaries were asked every 30 minutes for the first two weeks and every 1 hour for the second two weeks. Therefore, we collected 48 labels per days per person for the first two weeks, and 24 for the second two weeks, for a total of 114.830 labels.

## Sensor Data
The data from the sensors can be divided into: 
-	Hardware (HW) sensors, namely the sensors that one can find in a phone, e.g., accelerometer, gyroscope, GPS. The complete list of HW sensors used in this survey is reported in Table 1 
-	Software (SW) sensors, by which we mean all the SW events that can be collected from the Operating system and SW, for instance the Wifi the HW is connected and so on. The complete list of SW sensors is reported in Table 2
-	QU sensors (where QU stands for Questionnaire), by which we mean events which relate to the compilation of the Time Use Diary, mainly related to the various execution times, e.g., when a question arrived or was answered. The complete list of QU sensors is reported in Table 3

The complete documentation can be found [here]().


No | HW Sensor | Estimated Frequency |  Category | Description |
|-------|--------|---------|---------|---------|
1 | Accelerometer | up to 20 samples per second | Big | measures the acceleration to which the phone is subjected and it captures it as a 3D vector |
2 | Gyroscope | up to 20 samples per second | Big | measures the rotational forces to which the phone is subjected and it captures it as a 3D vector |
3 | Linear Acceleration | up to 20 samples per second | Big | measures the acceleration force to which the phone is subjected and it captures it as a 3D vector |
4 | Location | Once every minute | Small | returns the geocoordinates of where the phone is located, for more accuracy this sensor combines GPS and WIFI/cellular connections |
5 | Magnetic Field | up to 20 samples per second | Big | measures the magnetic field to which the phone is subjected and it captures it as a 3D vector |
6 | Pressure | up to 20 samples per second | Big | measures the ambient air pressure to which the phone is subjected |

*Table 1. HW sensors.*

No | SW Sensor | Estimated Frequency | Category | Description |
|-------|--------|---------|---------|---------|
7  | Activity Performed (Google Data)                   | Once every minute     | Small | returns a label identifying the activity performed by the user. This value is computed by Android using Google's Activity Recognition API along with low power signals from multiple sensors in the device. Possible activities are: _still, in\_vehicle, on\_bicycle, on\_foot, running, tilting, walking_ |
8  | Audio from the internal microphone                 | 10 seconds per minute | Small | Audio from the internal microphone |
9  | Audio mode (Silent/Normal)                     | On change             | Small | Audio from the internal microphone |
10 | Battery Charge (ON/OFF)                        | On change             | Small | returns whether the phone is currently charging its battery |
11 | Battery Level                                      | On change             | Small | returns the phone's battery level |
12 | Cellular network info                              | Once every minute     | Small | returns information related to the cellular network (cellid, dbm, type) to which the phone is connected to |
13 | Doze Modality (ON/OFF)                         | On change             | Small | returns whether the phone's doze mode is on or off. Doze mode is a low battery consumption state in which the phone enters after some time of not being used |
14 | Flight Mode (ON/OFF)                           | On change             | Small | returns whether the phone's Airplane mode is on or off, Airplane mode turns off all the connectivity features of the phone |
15 | Gravity                                            | 20 times per second   | Small | report the force of gravity on the axis |
16 | Headset plugged in (ON/OFF)                    | On change             | Small | returns whether the headphones of the phone where connected |
17 | Humidity                                           | 20 times per second   | Small | return ambient relative humidity.
18 | Music Playback (no track information) (ON/OFF) | On change             | Small | eturns whether music is being played on the phone (yes or no) using the default music player from the operating system |
19 | Notifications received                             | On change             | Small | measures when the phone receives a notification and when it is dismissed by the user |
20 | Orientation                                        | 20 times per second   | Small | return the azimuth, pintch and roll.
21 | Proximity                                          | On change             | Small | measures the distance between the user's head and the phone, depending on the phone it may be measured in centimeters (i.e., the absolute distance) or as labels (e.g, 'near', 'far') |
22 | Rotation Vector                                    | 20 times per second   | Small | return the rotation vector component along the axis
23 | Running Application                                | Once every 5 seconds  | Small | returns the name of the application (or application package) that is currently running in the foreground of the phone |
24 | Screen Status (ON/OFF)                         | On change             | Small | returns whether the phone's screen is on or off |
25 | Temperature                                        | 20 times per second   | Small | return the ambient air temperature.
26 | Touch event                                        | On change             | Small | generates a touch value each time the user touches the screen |
27 | WIFI Network Connected to                          | On change             | Small | returns information related to the WiFi network to which the phone is connected to, if connected will also report the WiFi network id |
28 | WIFI Networks Available                            | Once every minute     | Small | returns all WiFi networks detected by the smartphone |

*Table 2. SW sensors.*

No | QU Sensor | Estimated Frequency | Category | Description |
|-------|--------|---------|---------|---------|
29 | Time Diary questions | On change | Small| contains the question, the question id (for traceability purposes) and the timestamp when it was generated on the server and sent to the cloud provider for delivery |
30 | Time Diary confirmation | On change | Small| contains the timestamp at which each question, identified by its unique id, has been delivered to the device of the participant (which may coincide or not with the time the participant sees it) |
31 | Time Diary answers | On change | Small| contains the answer, the timestamp when it was saved in the server, and the difference between answer and notification times in milliseconds |
32 | Task questions | On change | Small| contains the question and the timestamp when it was sent from the server |
33 | Task confirmation | On change | Small| contains the timestamp when each specific question was notified to the participant |
34 | Task answers | On change | Small| contains the answer, the timestamp when it was saved in the server, and the difference between answer and notification times in milliseconds |

*Table 3. Questionnaire sensors.*

In these three sensor tables, the frequency by which the sensors are captured is reported, according to the following conventions: _on change_ means that the value of the sensor is recorded only when the current value is changed (along with a timestamp of when it happened), _up to X samples per second_ means that for each second the value of the sensor will be stored up to maximum of X times (these values are estimated), and _once every Y_ means that the values of a sensor is recorded once the time Y has passed (these values are estimated).


# Data collection
![SU2 Protocol](https://github.com/Gengis-Khan/SU2Dataset/blob/gh-pages/images/SU2_Protocol.png)

*The different phases of the data collection protocol*

The data collection was conducted in an interdisciplinary framework, involving sociology and IT experts. The survey methodology adopted is a variant of the ESM. In our case, in addition to the self-reported question, data from the smartphone sensors were collected through an app called [iLog](http://datascientia.disi.unitn.it/ilog/).

## Timing
The overall data collection process last for 6 weeks. The first two weeks were dedicated to sample recruitment by sending the first two questionnaires (invitation and assessment of habits). The remaining month was entirely dedicated to ESM through iLog, separated into two parts: during the first two weeks the notification time diaries was sent every half an hour, while for the second two weeks the notifications were reduced to one. The sensors were always collected with the same frequency. Questions that were not immediately answered were put in a FIFO queue, for a maximum of 12 questions. This means that a student could avoid answering for a maximum of 6 hours.

## Sample recruitment
The sample was selected within the entire student population of the University of Trento. All students were sent an invitation to participate in the survey, excluding a priori those who did not have a smartphone compatible with the study (only Android Operating System greater than 5.0) and did not regularly attend classes. After the first contact via email, the online questionnaire was sent to investigate their habits and routine, and finally it was sent a password to download and install the app iLog. 

From 1042 responses were excluded those who were born after 1993, to limit the dynamics of students out-of-school or who did not participate in university life. Of the 860 candidates, 318 students were selected, weighting the sample in such a way that it was proportional to the student population of each department, in order to avoid the misrepresentation of daily routines due to the different schedules.

## Incentive strategy
The strategy was based on a fixed salary and a series of bonuses. All participants who filled in at least 75\% received €20 every two weeks and the opportunity to participate in the draw for 3 prizes of €100 for the first two weeks of participation and 3 prizes of €150 for the second two weeks. Furthermore, every day 3 prizes of €5 were drawn and communicated via email to the winning participants, in order to (i) keep the participants' attention high; (ii) encourage communication with the helpdesk.

\subsection{Data preparation}
Once the data was collected, two different preparation procedures were performed, namely data cleaning and anonymization. The first was aimed at consolidating the data and making it accessible, while the second was aimed at removing personal information from the datasets.

# Example of application
This dataset hasalready been used in various fields to build KG on the notion of context. Examples of this are the following articles:
- Giunchiglia, F., Bignotti, E., & Zeni, M. (2017, March). Personal context modelling and annotation. In 2017 IEEE International Conference on Pervasive Computing and Communications Workshops (PerCom Workshops) (pp. 117-122). IEEE.
- Giunchiglia, F., Zeni, M., Bignotti, E., & Zhang, W. (2018, March). Assessing annotation consistency in the wild. In 2018 IEEE International Conference on Pervasive Computing and Communications Workshops (PerCom Workshops) (pp. 561-566). IEEE.
Chicago	
- Osman, N., Chenu-Abente, R., Shen, Q., Sierra, C., & Giunchiglia, F. (2021). Empowering Users in Online Open Communities. SN Computer Science, 2(4), 1-19.
Chicago	

In any case, the diversity of the data collected makes the dataset flexible and adaptable, such as computational social science: 
- Giunchiglia, F., Zeni, M., Gobbi, E., Bignotti, E., & Bison, I. (2018). Mobile social media usage and academic performance. Computers in Human Behavior, 82, 177-185.
or machine learning:
- Bontempelli, A., Teso, S., Giunchiglia, F., & Passerini, A. (2020). Learning in the wild with incremental skeptical gaussian processes. arXiv preprint arXiv:2011.00928.

Finally, this approach is the basis of a hackaton conducted with [EUROSTAT](https://ec.europa.eu/eurostat) in 2019, as well as in the various data collections conducted within the European project [WeNet](https://www.internetofus.eu), based on Horizon 2020 funds.

### Contact

Do you want to acess our dataset? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) and contact us at [datadistribution.knowdive@unitn.it](datadistribution.knowdive@unitn.it).
