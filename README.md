---
title: "<b style = 'color : #79CDCD; font-size: 75px;'> <center> ***Vaccine Attitudes***  </b> </center>" 
subtitle: "<b style = 'color : #79CDCD; font-size: 35px;'> <center> *FCB2021 *</b> </center>"
author: "Pablo Egaña & Naroa Beristain"
date: "02/12/2021"
output: 
  prettydoc::html_pretty:
    theme: hpstr
    highlight: github
    toc: yes 
    toc_depth: 2
lang: en-UK
---

# **Introduction**
<div><img src="coronavirus.jpg" width="200px" align="right"></div>

In late 2019, some cases of atypical pneumonia were reported in Wuhan, China. A few days later, it was discovered that this was due to the appearance of a new coronavirus called SARS-CoV-2, which causes COVID-19 disease. Due to the high speed of its spread, it spread throughout the world rapidly, making it an international health emergency and later a pandemic. However, in recent months different vaccines have been developed that can reduce the likelihood of infection, as they attribute some immunity to the virus to the patient.

However, not everyone wants or can access vaccination, as part of the population does not believe that vaccination is efficient and there are countries that do not have the necessary resources. Therefore, because this has generated great social controversy, we have decided to develop this work, to see if really the attitude towards vaccination is related to the mortality rate.

# **Objectives and Hypothesis**
The main objective of this website is to answer the question posed ('Are attitudes to COVID-19 vaccinations in a country associated with the mortality rate on that country, observed during the COVID-19 pandemic?') in a rational and consistent manner based on the comparison of the data analysed. For this we have collected data from different countries of the world (United States, Spain, Japan...) on: 

* The mortality rate. 

* The attitude of the population towards COVID-19 vaccination.

Our hypothesis was as follows: We believe that the attitude of the population towards COVID-19 vaccination is directly related to a country’s mortality rate. This is due to the fact that if a country is against the main measure of protection against the virus, it will surely disagree with the other preventions taken to eradicate the virus( use of mask, hydroalcoholic gel, social distance...), and therefore, the mortality rate will increase rapidly.

# **Abstract**
Are attitudes to COVID-19 vaccinations in a country associated with the mortality rate on that country, observed during the COVID-19 pandemic? This question has been the main way to guide the research we have carried out, which is based on the analysis of mortality data and the attitude towards vaccination. After carrying out this project, together with its graphs and tables, we have been able to observe that the country where the mortality rate is highest is Japan and Germany, while in the last places are Singapore and Australia. On the other hand, we find a more positive attitude towards vaccination in the countries of Japan and the United Kingdom, while a large part of the German and American population is against it, making the latter two countries the most negative to the vaccine.

Using these data we have been able to verify that although it is true that there is a certain relationship between mortality and attitude towards vaccination, this has not seemed to be the only factor influencing the number of deaths. A clear example of this has been that of the Japanese country where, despite their positive attitude towards vaccination, they have achieved a much higher mortality rate than in most of the countries analyzed.

# **Methodology**
To carry out our project, we first download and unzip with GitBash the data provided and put it together in the same directory. Then, we introduced the topic explaining our objectives and hypotheses, and we began to analyze the data of the countries that interested us:

- Australia
<div><img src="vaccinepng.png" width="200px" align="right"></div>
- Japan

- Singapore

- Germany

- Spain

- United Kingdom

- Canada

- United States

First we did it with the different files that explained the vaccine attitudes of the population. To do this, using the command table, we collect the different responses of the population (No answer, Strongly Agree, Agree, Neither agree or disagree, Disagree or Strongly Disagree). Then we calculated the percentage of each of the answers given, and with this data we made 2 vectors. Finally, we joined the two vectors by means of a pie command achieving a foot chart that made the results much more visible.
```
pie(country, labels= c("%(no answer)", "%(strongly agree)", "%(agree)", "%(neither agree or disagree)", "%(disagree)", "%(strongly disagree)"), main= "Country", sub="Vaccine Attitudes", col= c("gray", "green4", "green", "yellow", "orangered", "red3"))
```
Secondly, we did something similar with the data of death rate, where we grouped all the deaths of each country by months and put them together in a different chart for each country by the plot function.

```
plot(x, y, type ="l", col = "red", points(x, y, bg="green"), main ="Country", sub = "Deaths per 100000 inhabitants", xlab="Months", ylab="Death rate)
points(x, y, pch=8, cex=1 ,bg="green")
```

Instead, here to achieve comparable data between all countries, we looked for the population of each of them and put all the data in deaths per 100000 inhabitants following the formula: Death rate per 100000 inhabitants: 

- (total deaths in the country 100000) / country’s population

Third, we create 2 bar graphs using the bar plot command and a table to compare the data in the conclusion.
```
barplot(deaths, main="Vaccine Attitudes", horiz=TRUE, names.arg=c("Australia", "Japan", "Singapore", "Germany", "United Kingdom", "Spain", "United States", "Canada"), cex.names=0.8, col = c("#FFF68F", "#FFA07A", "#B4EEB4", "#E0EEE0", "#B0E2FF", "#FFDEAD", "#96CDCD", "#EEAEEE")) 
barplot(attitudes, main="Vaccine Attitudes", horiz=TRUE, names.arg=c("Australia", "Japan", "Singapore", "Germany", "United Kingdom", "Spain", "United States", "Canada"), cex.names=0.8, col = c("#FFF68F", "#FFA07A", "#B4EEB4", "#E0EEE0", "#B0E2FF", "#FFDEAD", "#96CDCD", "#EEAEEE"))
```
In the first of the graphs, we compare the average mortality rate data of each country, in which we group all the average deaths per 100000 inhabitants in all 2020. In the second of the graphs, we also calculated the average of the responses on the different opinions that people have about COVID-19 vaccination. In the final table, we made three columns, in which we put the country, the deaths in 2020 per 1000000 inhabitants and the average responses on the different attitudes towards the COVID.

Finally, with the help of all the graphs created above, we began to write our work country by country, introducing the epidemiological situation in this and comparing the different data shown in the graphs. Finally, in the conclusion, we make a comparison of all the countries to discover if our main hypothesis was true, and if really those countries that record more deaths, are against immunization.

# **Analysis of the data and Results**
## <span style = 'color : gray;'> 1. *Australia* </span>
<div><img src="Australia.png" width="150px" align="right"></div>

The COVID-19 pandemic in Australia began on January 25 2020 in the city of Melbourne, Victoria, by a man from Wuhan, China, positive for COVID-19. On 20 March, Australia closed all its borders, and on 21 March, rules of social estrangement and closure of "non-essential" services began. 

The first wave began, as we can see on the chart, in late March or early April. Months later, there was a second wave, larger than the first one, in which there were more than 7000 active cases. In the graph we can see how from June there is an increase in deaths that reach their peak in the month of August (46 deaths per 100000 inhabitants), where they begin to fall until stabilizing in the month of October.

<div><img src="Australia VA.png" width="475px" align="right"></div>
<div><img src="Australia PDR.png" width="300px" align="left"></div>

The first chart shows the deaths that occurred in each month of 2020 in Australia. We can clearly appreciate the presence of two waves: 

- The first one was between the months of March and May, in which they began to take measures against its propagation. 
- A second major wave which reached the peak of the pandemic in the country between June and October 2020. 

On the other hand, the pie chart shows the different attitudes of the population towards COVID-19 vaccination. We can see that although the majority of the surveyed did not answer, between those who did it, the majority were in favour of vaccination, although there was also a large part of disagreement.

Therefore, if we make the average of the deaths per 100000 inhabitants of the country, it will give us 42.11 people. On the other hand, the general attitude towards vaccination in the country is 2.66. Because of this, we can say that the majority of the population is in favour of the immunisation programme. In conclusion, we see that the mortality rate is quite low, and that the majority of the population is in favor of the vaccine, so we can see that in this country our hypothesis of the greater population in favor of the vaccine, the lower mortality rate, is correct.

## <span style = 'color : gray;'> 2. *Japan* </span>
<div><img src="jappng.png" width="150px" align="right"></div>

The COVID-19 pandemic in Japan arrived on January 16 2020 from China, when a resident of Kanagawa Prefecture traveled recently to Wuhan tested positive for COVID-19. On February 27, 2020, various measures were taken such as the closure of all Japanese schools until early April to help contain the virus. 

The first wave originated in early 2020 in January. This is represented in the graph by the peak that is over 105 deaths per 100000 inhabitants. After this major outbreak the cases seemed to stabilize for a while during the spring and summer months. However, as we can see in the graph, at the end of the year there was a resurgence increasing the number of deaths, which would reach their maximum in the month of December (105 deaths per 100000 inhabitants).

<div><img src="Japan VA.png" width="425px" align="right"></div>
<div><img src="Japan PDR.png" width="350px" align="left"></div>

The first chart 1 shows the deaths that occurred in each month of 2020 in Japan. In this is clearly seen the presence of two peaks: 

- The first one was in the first month of the year, so, in which measures began to be taken at the end of February. 

- A second major wave in which the peak of the pandemic was reached in the country. This occurred at the end of the year, in the month of December.

On the other hand, the pie chart shows the different attitudes of the Japanese population towards COVID-19 vaccination. We can see that although the majority of surveyed did not respond,  between those who did it, the majority were in favour of vaccination, although there was also a large part that did not care and a smaller part that disagreed. 

Therefore, if we make the average of the deaths per 100000 inhabitants of the country, gives us that this was 91.54 people. On the other hand, the general attitude towards vaccination in the country is 2.6. Because of this we can say that the majority of the population is in favour of the immunisation programme. However, we see that the mortality rate is quite high, but that the majority of the population is in favor of the vaccine, so we can say that this country does not meet our hypothesis of greater population in favor of the vaccine, lower mortality rate.

## <span style = 'color : gray;'> 3. *Singapore* </span>
<div><img src="sinpng.png" width="150px" align="right"></div>

The COVID-19 pandemic in Singapore began on 23 January 2020. The first cases were mainly imported until local transmission began to develop in February and March. In response to the first wave of COVID-19, Singapore announced on 3 April 2020 a set of preventive measures collectively called the "circuit breaker lockdown". 
 
The first wave originated in early 2020 in January. This is represented in the graph by the peak that is over 36 deaths per 100000 inhabitants. After this major outbreak the cases seemed to stabilize in the rest of the year since although there is a slight variation in the cases all remain around the 30.

<div><img src="Singapore VA.png" width="425px" align="right"></div>
<div><img src="Singapore PDR.png" width="350px" align="left"></div>

The first chart 1 shows the deaths that occurred in each month of 2020 in Singapore. In this is clearly seen the presence of a single wave: 

- It occurs in January. However, when putting prevention measures in place, the cases go down. 

The pie chart, on the other hand, shows the different attitudes of the population of Singapore towards COVID-19 vaccination. We can see that although the majority of polled did not respond,between those who did it, the majority were either in favour of vaccination or did not care. On the contrary, a smaller part disagreed about being vaccinated.

Therefore, if we make the average of the deaths per 100000 inhabitants of the country, gives us 32.22 people. On the other hand, the general attitude towards vaccination in the country is 2.7. Because of this we can say that the majority of the population is in favour of the immunisation programme. Thanks to these data, we can see that the mortality rate is quite low and that the majority of the population is in favour of the vaccine. In this way we deduce that in this country our hypothesis of greater population in favor of the vaccine, lower mortality rate, is fulfilled.

## <span style = 'color : gray;'> 4. *Germany* </span>
<div><img src="gerpng.png" width="100px" align="right"></div>

The COVID-19 pandemic in Germany began on January 27 2020 in the region of Baviera, by a man coming from Wuhan, China, positive for COVID-19. On March, Germany took some social distancing measures such as forbidding groups of more than 2 people or closing all the non-essential shops.

The first wave began, as we can see on the chart, in March.  Months later, there was a second wave, similar to the first one. In the graph we can see how from October there is an increase in deaths that reach their peak in the month of November (118.93 deaths per 100000 inhabitants), that maintained in the month of December too.

<div><img src="Germany VA.png" width="425px" align="right"></div>
<div><img src="Germany PDR.png" width="350px" align="left"></div>

The first chart shows the deaths that occurred in each month of 2020 in Germany. We can clearly appreciate the presence of two waves: 

- The first one was between the months of March and May, in which they began to take measures against its propagation. 

- A second similar wave which reached the peak of the pandemic in the country between October and December 2020. 

On the other hand, the pie chart shows the different attitudes of the population towards COVID-19 vaccination. We can see that although the majority of the surveyed did not answer, between those who did it, the most common answer was 1(strongly agree), although there was also a large part of disagreement.

Therefore, if we make the average of the deaths per 100000 inhabitants of the country, it will give us 97.85 deaths. On the other hand, the general attitude towards vaccination in the country is 2.84. Because of this we can see that although the majority is in favour of vaccination there is a large part of the population that is against it. The part that is against vaccination is greater in this country than in most of those we have analyzed, so we have deduced that its high mortality rate is partly due to this attitude of rejection of vaccination by a large part of the population. It should also be borne in mind that Germany is a country that has been fighting against the pandemic without confining its population, leading to an increase in the number of deaths in the country. That’s why we believe that it is of vital importance that a population is in favour of vaccination, in order to eradicate the pandemic.

## <span style = 'color : gray;'> 5. *Spain* </span>
<div><img src="spapng.png" width="100px" align="right"></div>

The COVID-19 pandemic in Spain began with a first diagnosis in the Gomera Island on 31 January 2020, when a German tourist tested positive for COVID-19, while the first known death occurred on 13 February. In the face of the rapid spread of the virus, on 14 March it was declared a state of alarm limiting the free movement of citizens to essential acts, which ultimately resulted in the confinement of the population to their places of residence.

The first wave originated in March and lasted until April, reaching the maximum number of deaths (130 deaths per 100000 inhabitants). After this major outbreak the cases seemed to stabilize in the rest of the year until November where there was another peak due to the second wave, which reached a value of 103 deaths per 10000 inhabitants.

<div><img src="Spain VA.png" width="425px" align="right"></div>
<div><img src="Spain PDR.png" width="350px" align="left"></div>

The first chart 1 shows the deaths that occurred in each month of 2020 in Spain. In this is clearly seen the presence of a single wave: 

- The first one was between the months of March and April, in which they began to take strict measures against its propagation. 

- A second major wave, which reached another high value of the pandemic in the country, was in November 2020.  

The pie chart, on the other hand, shows the different attitudes of the Spanish population towards COVID-19 vaccination. We can see that although the majority of respondents did not answer, between those who did it, the majority were in favour of vaccination. This has come in sharp contrast to the few who were not in favour of vaccinations or who did not care.

Therefore, if we make the average of the deaths per 100000 inhabitants of the Spanish country, that gives us 85.83 people. On the other hand, the general attitude towards vaccination in the country is 2.66. Because of this we can say that the majority of the population is in favour of the immunisation programme. However, we see that the mortality rate is quite high, but that the majority of the population is in favor of the vaccine. For this reason Spain is not one of the countries that meets our hypothesis of greater population in favor of the vaccine, lower mortality rate.

## <span style = 'color : gray;'> 6. *United Kingdom* </span>
<div><img src="UKpng.png" width="100px" align="right"></div>

The COVID-19 pandemic in the UK began on January 31 2020 in the region of Newark, when about 10 people who assisted a party tested positive for COVID-19. On February, the UK started an information campaign in order to raise the awareness of the population. On March, the UK’s government introduced the first restrictions in order to control the spread of the COVID-19 which involved aspects such as people’s freedom of movement or education.

The first wave began, as we can see on the chart, in April, where they reached the peak of the cases(130.19 deaths per 100000 inhabitants). After the months of April and May, in June there was a sharp decline in cases, causing the end of this first wave . Months later, there was a second wave, lighter to the first one between the months of October and December.

<div><img src="United Kingdom VA.png" width="425px" align="right"></div>
<div><img src="UK PDR.png" width="350px" align="left"></div>

The first chart shows the deaths that occurred in each month of 2020 in the UK. We can clearly appreciate the presence of two waves: 

- The first one was between the months of April and June, in which they began to take measures against its propagation and lockdown was enforced. This wave reached the peak of the pandemic in the country

- A second smaller wave in the country between October and December 2020. 

On the other hand, the pie chart shows the different attitudes of the population towards COVID-19 vaccination. We can see that although the majority of the surveyed did not answer, between those who did it, the vast majority answered 1(strongly agree), there was also a minor part who answered 5(strongly disagree).

Therefore, if we make the average of the deaths per 100000 inhabitants of the country, it will give us 83.95 deaths. On the other hand, the general attitude towards vaccination in the country is 2.24. Because of this, we can say that the majority of the population is in favour of the immunisation programme. It is obvious that when the COVID-19 started extending from the country, most people wanted to eradicate it, so measures and recommendations were correctly followed by the population, and the mortality rates declined in the following months. In conclusion, we see that the mortality rate is quite low once the first wave passed, and that the majority of the population is in favor of the vaccine, so in this country our hypothesis of the greater population in favor of the vaccine, the lower mortality rate, is correct.


## <span style = 'color : gray;'> 7. *Canada* </span>
<div><img src="canpng.png" width="150px" align="right"></div>

The COVID-19 pandemic in Canada was confirmed on 27 January 2020, after an individual who had returned to Toronto from Wuhan tested positive. Until March, all cases were related to recent travel to a country with a substantial number of cases. However, the first case of community broadcasting in Canada was confirmed on 5 March, so in the middle of the same month, they took severe measures including closing schools and entertainment venues along with restricting border access.

As we can see in the graph, the first wave began in March, however in April there is a decrease in deaths , which we could attribute to the measures taken. A month later, in May, the maximum number of deaths per 100000 inhabitants was reached (82 per 100000 inhabitants). After the month of May, between June and July, there was a sharp decline in cases, causing the end of this first wave. In the rest of the year there were two other significant peaks, that of August, and that of November.

<div><img src="Canada VA.png" width="425px" align="right"></div>
<div><img src="Canada PDR.png" width="350px" align="left"></div>

The first chart shows the deaths that occurred in each month of 2020 in Canada. We can clearly appreciate the presence of one waves: 

- The first wave occurred between the months of March and May, but given the measures taken the cases dropped in the first months of summer. 

- This wave reached the peak of the pandemic in the country There were other cases in August and November.

On the other hand, the pie chart shows the different attitudes of the Canadian population towards COVID-19 vaccination. We can see that although the majority of the polled did not answer, between those who did it, the vast majority answered 1(strongly agree), there was also a considerable part of society who was against this measure against the spread of the virus.

Therefore, if we make the average of the deaths per 100000 inhabitants of the country, it will give us 67.02 deaths. On the other hand, the general attitude towards vaccination in the country is 2.75. Because of this, we can say that most of the population agree on being vaccinated. To conclude, we can see that the country’s general positive attitude towards vaccination has a positive influence on the mortality rate since this is much lower than in other countries.

## <span style = 'color : gray;'> 8. *United States* </span>
<div><img src="eeuupng.png" width="150px" align="right"></div>

The COVID-19 pandemic in USA began on January 21 2020 in the state of Washington, when a man coming from Wuhan, China, tested positive for COVID-19. In March, US  took some social distancing measures such as confinement or closure of non-essential shops.

Due to the big dimensions of the country, the quantity of deaths varies a lot, as in some regions the situation may improve, while in others enworse. However, we can see that the worst months were February, April, May, August, October and December(the worst with 98.33 deaths per 100000 inhabitants).

<div><img src="United States VA.png" width="425px" align="right"></div>
<div><img src="US PDR.png" width="350px" align="left"></div>

The first chart shows the deaths that occurred in each month of 2020 in USA. Even if it is really variated, we can distinguish 3 main waves: 

- The first one was between the months of April and May, in which they began to take measures against its propagation. 

- A second similar wave in August.

- A third wave, which reached the peak of the pandemic in the country between the months of October and December. 

On the other hand, the pie chart shows the different attitudes of the population towards COVID-19 vaccination. We can see that although the majority of the surveyed did not answer, the vast majority was opposed to vaccination, being the most common answer 5(strongly disagree) and the general attitude towards immunization 3.48.

Therefore, if we make the average of the deaths per 100000 inhabitants of the country, it will give us 85.19 deaths. On the other hand, the general attitude towards vaccination in the country is 3.48. Because of this, we can say that most of the population is against getting vaccinated. To conclude, we can see that the country’s general negative attitude towards vaccination has a great effect on the number of deaths in the country, which is one of the tallest we’ve analyzed. 

# **Conclusions**
<div><img src="Conclusionoficial.png" width="800px" align="left"></div>
<div><img src="Conclusionchart2.png" width="800px" align="left"></div>

| Countries      | Death rate | Vaccine Attitudes |
|----------------|------------|-------------------|
| Australia      | 42.1       | 2.66              |
| Japan          | 91.54      | 2.6               |
| Singapore      | 32.22      | 2.7               |
| Germany        | 97.85      | 2.84              |
| Spain          | 85.83      | 2.66              |
| United Kingdom | 83.95      | 2.24              |
| United States  | 85.19      | 3.48              |
| Canada         | 67.02      | 2.75              |

If we analyze all the data obtained, we can verify that the countries with the majority of their population in favor of the vaccine are those that have the least excess of mortality, such as Australia or Singapore. On the other hand, those countries that are not in favour of the vaccine tend to have higher excess mortality. However, there are also exceptions such as the Japanese country, which is one of the most vaccination-friendly countries, but has a high level of mortality.

This has led us to think that while the attitude of people is of great importance in trying to slow down the spread of the virus, there are also other factors that we have not taken into account but that are influential in the spread of the pandemic, such as the resources available to each country. On the other hand, many of the surveyed in most of the countries did not answer the question when they were asked for their opinion of the vaccine. So a really good way to improve the research would be to try to survey as many people as possible, in order to achieve more reliable results. However, despite other factors influencing the spread of the pandemic, we believe that the only way to finally eradicate the virus is for there to be an awareness-raising population and in favour of vaccination.

# **Bibliography**

These are the links we have used in order to get the information:

- [COVID-19 Excess of Mortality data](https://github.com/Financial-Times/coronavirus-excess-mortality-data)

- [Vaccine attitudes data](https://github.com/YouGov-Data/covid-19-tracker)

- [COVID-19 pandemic in Australia](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_Australia)

- [COVID-19 pandemic in Japan](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_Japan)

- [COVID-19 pandemic in Singapore](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_Singapore)

- [COVID-19 pandemic in Germany](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_Germany)

- [COVID-19 pandemic in Spain](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_Spain)

- [COVID-19 pandemic in United Kingdom](https://en.wikipedia.org/wiki/COVID-19_pandemic_in__the_United_Kingdom)

- [COVID-19 pandemic in United States](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_the_United States)

- [COVID-19 pandemic in Canada](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_Canada)
