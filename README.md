# nepal-livestock-analysis

The dataset used for this analysis is attached here:

- [production-of-cotton-in-nepal-by-district.csv](https://github.com/ankit-d-dhakal/nepal-livestock-analysis/files/9108126/production-of-cotton-in-nepal-by-district.csv)
- [production-of-egg-in-nepal-by-district.csv](https://github.com/ankit-d-dhakal/nepal-livestock-analysis/files/9108127/production-of-egg-in-nepal-by-district.csv)
- [rabbit-population-in-nepal-by-district.csv](https://github.com/ankit-d-dhakal/nepal-livestock-analysis/files/9108129/rabbit-population-in-nepal-by-district.csv)
- [wool-production-in-nepal-by-district.csv](https://github.com/ankit-d-dhakal/nepal-livestock-analysis/files/9108130/wool-production-in-nepal-by-district.csv)
- [yak-nak-chauri-population-in-nepal-by-district.csv](https://github.com/ankit-d-dhakal/nepal-livestock-analysis/files/9108131/yak-nak-chauri-population-in-nepal-by-district.csv)
- [horseasses-population-in-nepal-by-district.csv](https://github.com/ankit-d-dhakal/nepal-livestock-analysis/files/9108132/horseasses-population-in-nepal-by-district.csv)
- [milk-animals-and-milk-production-in-nepal-by-district.csv](https://github.com/ankit-d-dhakal/nepal-livestock-analysis/files/9108133/milk-animals-and-milk-production-in-nepal-by-district.csv)
- [net-meat-production-in-nepal-by-district.csv](https://github.com/ankit-d-dhakal/nepal-livestock-analysis/files/9108135/net-meat-production-in-nepal-by-district.csv)

# 1\. Data Understanding

The data is about livestock raised across Nepal based on
various districts/regions and the commodities produced by them. The
overall data is divided based on the products of meat, milk, egg, number
of animals, cotton and wools. All these data are separated in multiple
.csv file.


# 2\. Data Merging and Cleaning

## 2.1 Creating pandas dataframe for different dataset


Now, there are rows named as Total in different dataset so by verifying
we found out that the total is not actual total so it is removed from
dataset.


## 2.2 Performing Necessary cleaning

After looking deeply into dataset there were some necessary cleanings to
be done before merging dataset. The name of the districts were different
so the difference is identified with the function named
**find\_difference()** and all the names are renamed as same name.

After performing necessary cleaning all the dataframes are merged together on reference of district one by one to
form new final dataframe. Now all the necessary data analysis is
performed using this final merged dataframes.

# 3\. Exploratory Data Analysis

Here is the presentation of insights gained from the dataset with the
use of different analysis and visualization techniques.

## 3.1 Milk production analysis in Nepal

The dataset is represented in different subplots for further analysis
of milk production in different regions.

![image](https://user-images.githubusercontent.com/29594566/178894676-326b6203-977b-4498-97dd-d7cea55ea601.png)

![image](https://user-images.githubusercontent.com/29594566/178894697-b81ad0ab-0f1a-48c5-a739-502d066f4009.png)


All the subplots are divided into 5 different regions of Nepal i.e
eastern, central, western, mid-western and far-western regions. And the
data are divided based on three regions of Nepal which are Mountain
region, Hilly region and Terai region. Now looking into the data, we can
see that maximum number of milk is produced in western hills region of
Nepal and minimum number of milk produced is in mid-western mountain
region of Nepal. But the capacity of producing milk is high in
mid-western hills region of Nepal because number of milking cows and
number of buffaloes is higher in this region comparing to others.

Looking into 5 different regions wise we can see that C.region has the
highest number of milk produced whereas far-western region has low
number of milk produced.

## 3.2 Duck egg production in five regions of Nepal

![image](https://user-images.githubusercontent.com/29594566/178894855-2216506f-1370-43f3-aae1-d7a32cc3831e.png)

From above barplot we can see that the highest numbers of ducks is
present in farms of E.region area of Nepal but the egg production is
very less compared with total number of ducks. Second highest number of
ducks is in western region of Nepal but the egg production here is also
less compared to number of ducks present in farms. Also, skimming
through other regions the situation is same there higher number of ducks
but the egg production is very less.

So, in conclusion we can say that despite having maximum number of egg
producing duck the actual egg production is very less in every region of
Nepal.

## 3.3 Five Nepali regions' meat production analysis

![image](https://user-images.githubusercontent.com/29594566/178894978-45ce98fd-1fc6-4fa2-8719-164262d4f843.png)

Looking closely in above lineplot which is divided in five different
regions of Nepal. We can see that the total number of meat production
including all mutton, buff, chevon and chicken is high in central region
and the lowest is in far western region of Nepal. But looking closely in
particular meat we can see that mutton and chicken meat production is
highest in central region and chevon meat production is similar in all
regions of Nepal.

## 3.4 Nepal wool production in 5 regions

![image](https://user-images.githubusercontent.com/29594566/178895056-5749db35-b369-4581-8946-b2ba16446b83.png)

Interpreting data from above pie chart we can see that the 50% of wool
production is done in mid-western region of Nepal and lowest number
which is 9.74% of wool production is in central region of Nepal. Eastern
region of Nepal also has similar number of wool productions as central
region of Nepal. There is only difference of nearly 5% of production in
western region and far-western region of Nepal.

## 3.5 Three Nepali districts' cotton production study

![image](https://user-images.githubusercontent.com/29594566/178895112-870e7690-7947-4eb2-bc03-8ead717d381f.png)

Looking through the presentation of pointplot we can see that final
yield of cotton is higher in Banke district of Nepal whereas production
per land area is similar in all three districts of Nepal. But lowest
number of production is in Dang and Bardiya lies between Banke and Dang
in actual production of cotton.

So, we can see that despite having similar production numbers in all
three districts actual yield is good in Banke district.

## 3.6 Nepal horse population analysis

![image](https://user-images.githubusercontent.com/29594566/178895232-1e6ec9dd-1a84-41e8-a077-2b01afeefa67.png)

Looking through the presentation of pointplot we can see that maximum
number of horseasses is in mid-western region of Nepal whereas central
region of Nepal has the lowest number of horseasses comparing to other
regions. But the number of horseasses is similar in eastern and western
region of Nepal. And far-western region falls in second lowest category
in having number of horseasses.

## 3.7 Nepali district-by-district production analysis

![image](https://user-images.githubusercontent.com/29594566/178895407-b3b6cd20-ca26-41b1-b793-416fe4a87517.png)

The heatmap presents correlation between different data. If the colour
is dark then the correlation between two attributes is strong and if the
colour is light then the correlation between them is very weak. So, from
above heat map we can see that Total Meat production has strong
correlation with Total Milk produced whereas Total Milk produced has
very weak correlation with sheep wool produced.

## 3.8 Analysis of YAK/NAK/CHAURI populations in Nepal

![image](https://user-images.githubusercontent.com/29594566/178895497-9f18f7da-0843-4046-804a-8160b5b00521.png)

Above barplot represents the distribution of population of
yak/nak/chauri in different regions of Nepal. We can see that the number
of yak/nak/chauri is very high in eastern region whereas the number is
very less far-western region of Nepal. Second highest number falls in
mid-western region of Nepal and second lowest in central region of
Nepal. And the total population of western region lies between eastern
and mid-western region.
