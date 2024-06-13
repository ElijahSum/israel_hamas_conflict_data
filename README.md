# israel_hamas_conflict_data
The repository contains data on the conflict between Israel and Hamas, which began on October 7, 2023. The data contains complete information about the bombing of Israel, israeli civilian and military deaths. Unfortunately, it is impossible to create similar dataset on Palestinian data due to the lack of information sources.

# Data Description
## Air Alarms (Tseva Adom) data
**air_alarms_bombardments.csv** contains data on all air alerts declared in Israel from 2021 to April 2024, which allows you to compare the intensity of attacks before and after the outbreak of the conflict on October 7, 2023. 


***Tseva Adom** stands for a Hebrew name of Israeli Air Alarms notification system*.


The data was obtained using the scraping of the official [Tseva Adom website](https://www.tzevaadom.co.il/en/).


- Most of the missile alerts are announced due to the launch of rockets from Gaza into Israel. Recently, air alerts have also been announced in the event of drone infiltration.
- In most cases, an air alert is announced simultaneously in several towns and villages that may be hit by a missile attack. The **attack_number** column contains information about unique attacks.
- In total, from May 2021 to April 2024, there were 2,382 unique rocket attacks, drone infiltrations, etc. At the same time, the alarm was announced 16,272 times in different cities.
- The data includes different levels of aggregation and contains information both on the region of the air alert and on a specific city, village and district.


## Civilian Casualties Data
**civilian_casualtes.csv** contains data on Israeli civilian casualties from October 7, 2023 to May 11, 2024. 

The data was obtained using the scraping of the official [Ministry of Foreign Affairs website](https://www.gov.il/en/pages/swords-of-iron-civilian-casualties). 

- The data contains columns indicating the name, age, nationality, city of origin of the deceased, date and place of murder (with geographical coordinates).
- In addition, for cases where the death of civilians was learned much later, the revealed column indicates the date of the appearance of information about the death of a person.
- The data is standardized and ready for use.

*Unfortunately, the data does not contain information about the gender and some other demographic characteristics of the deceased (for example, the subethnic group of Jewish origin). I will be very glad if you can help with filling in this information and offer a Pull Request.*

## the Israel Defence Forces (IDF) casualties
**idf_casualties.csv** contains information on all losses of the Israeli armed forces from October 7, 2023 to May 15, 2024.

The data was obtained using the scraping of the official [Swords of Iron IDF Casualties website](https://www.gov.il/en/pages/swords-of-iron-idf-casualties). 

- The data contains the name, age, city of origin of the deceased, as well as their military rank, date of death.
- In some cases, the official website indicates that the military belonged to the reserve. In order to control whether the deceased was a reservist, I use the binary variable **is_reservist**.
- The data is standardized and ready for use.


I will be glad to receive feedback from you.
