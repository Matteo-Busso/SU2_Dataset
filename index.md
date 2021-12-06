# Dataset Description
The survey was conducted with 158 participants, and it is composed by three sources of data: (i) Online questionnaire (synchronic); (ii) Time Diaries (diachronic); Sensor data (diachronic).

## Participants


## Online questionnaires 
Were used to invite the students, to evaluate the app, and to understand their habits and routine. They are composed by attributes regarding:
1. Socio-demographics: age, gender, students’ accommodation(s) and flat mates
2. Habits about travel, occupation, and university experience
3. Psycho-social profile, concerning:
- personality, collected with a 10-item short version of the [Big Five]() Inventory-44
- attitude towards procrastination [Irrational Procrastination Scale (IPS)]()
- smartphone habits [Smartphone Addiction Scale (SAV-SV)]()
- perceived stress [Perceived Stress Scale]()

The complete questionnaire can be found [here]()

## Time Diaries
Time diaries are a classic [data collection tool](), where respondents are asked to indicate three main dimensions of their everyday life: the activities performed, the locations they visit, and the people around them. In this case we administered a version, following the [HETUS]() standard, implemented in the app [iLog](). Participants received a notification on their smartphone with four questions (see Figure), namely: 
1. “What are you doing?” 
2. “Where are you?” 
3. “Who is with you?” 
4. “What is your mood?” 
![TD_Labels v2](https://github.com/Gengis-Khan/SU2Dataset/blob/gh-pages/images/TD_Labels.png)

During the month of data collection, time diaries were asked every 30 minutes for the first two weeks and every 1 hour for the second two weeks. Therefore, we collected 48 labels per days per person for the first two weeks, and 24 for the second two weeks, for a total of 114.830 labels.

## Sensor Data
The data from the sensors can be divided into: 
-	Hardware (HW) sensors, namely the sensors that one can find in a phone, e.g., accelerometer, gyroscope, GPS. The complete list of HW sensors used in this survey is reported in Table 1 
-	Software (SW) sensors, by which we mean all the SW events that can be collected from the Operating system and SW, for instance the Wifi the HW is connected and so on. The complete list of SW sensors is reported in Table 2
-	QU sensors (where QU stands for Questionnaire), by which we mean events which relate to the compilation of the Time Use Diary, mainly related to the various execution times, e.g., when a question arrived or was answered. The complete list of QU sensors is reported in Table 3


No | HW Sensor | Estimated Frequency |  Category |
|-------|--------|---------|---------|
1 | Accelerometer | up to 10 samples per second | Big| 
2 | Gyroscope | up to 10 samples per second | Big |
3 | Light | up to 10 samples per second | Big |
4 | Location | Once every minute | Small |
5 | Magnetic Field | up to 10 samples per second | Big |
6 | Pressure | up to 10 samples per second | Big |

*Table 1. HW sensors.*

No | SW Sensor | Estimated Frequency | Category |
|-------|--------|---------|---------|
7 | Airplane Mode (ON/OFF) | On change | Small |
8 | Battery Charge (ON/OFF) | On change | Small |
9 | Battery Level | On change | Small |
10 | Bluetooth Devices | Once every minute | Small |
11 | Bluetooth LE (Low Energy) Devices | Once every minute | Small |
12 | Cellular network info | Once every minute | Small |
13 | Doze Mode (ON/OFF) | On change | Small |
14 | Headset Status (ON/OFF) | On change | Small |
15 | Movement Activity Label | Once every 30 seconds | Small |
16 | Movement Activity per Time | Once every 30 seconds | Small |
17 | Music Playback (no track information) | On change | Small |
18 | Notifications received | On change | Small |
19 | Proximity |  up to 10 samples per second | Small  |
20 | Ring mode (Silent/Normal) | On change | Small |
21 | Running Applications | Once every 5 seconds | Small |
22 | Screen Status (ON/OFF) | On change | Small |
23 | Step Counter | up to 10 samples per second | Small |
24 | Step Detection | On change | Small |
25 | Touch event | On change | Small |
26 | User Presence |  On change | Small  |
27 | WIFI Network Connected to | On change | Small |
28 | WIFI Networks Available | Once every minute | Small |

*Table 2. SW sensors.*

No | QU Sensor | Estimated Frequency | Category |
|-------|--------|---------|---------|
29 | Time Diary questions | On change | Small|
30 | Time Diary confirmation | On change | Small|
31  | Time Diary answers | On change | Small|
32 | Task questions | On change | Small|
33 | Task confirmation | On change | Small|
34 | Task answers | On change | Small|

*Table 3. Questionnaire sensors.*

# Data collection
![SU2 Protocol](https://github.com/Gengis-Khan/SU2Dataset/edit/gh-pages/images/SU2_Protocol.png)
The data collection was conducted in an interdisciplinary framework, involving sociology and IT experts. The survey methodology adopted is a variant of the ESM. In our case, in addition to the self-reported question, data from the smartphone sensors were collected through an app called [iLog]().

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


You can use the [editor on GitHub](https://github.com/Gengis-Khan/SU2Dataset/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Gengis-Khan/SU2Dataset/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
