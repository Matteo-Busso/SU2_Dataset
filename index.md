# Dataset Description
The dataset is composed by three sources of data: (i) Online questionnaire (synchronic); (ii) Time Diaries (Diachronic); Sensor data (Diachronic).

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
![TD_Labels v2](https://github.com/Gengis-Khan/SU2Dataset/edit/gh-pages/images/TD_Labels%v2.png)

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


No || SW Sensor | Estimated Frequency | Category |
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


No | HW Sensor | Estimated Frequency |  Category |
1 | Accelerometer | up to 10 samples per second | Big| 
2 | Gyroscope | up to 10 samples per second | Big |
3 | Light | up to 10 samples per second | Big|
4 | Location | Once every minute | Small |
5 | Magnetic Field | up to 10 samples per second | Big |
6 | Pressure | up to 10 samples per second | Big |

# Data collection
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
