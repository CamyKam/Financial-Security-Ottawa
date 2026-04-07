# Household Financial Security Sentiment in the Ottawa/Gatineau Region
This project looks at the survey responses from households in the Ottawa/Gatineau Region in regards to a specific question posted in various surveys from the government of Canada. Respondents were asked:
<br><b>"In the past 12 months, how difficult or easy was it for your household to meet its financial needs in terms of transportation, housing, food, clothing, and other necessary expenses?"</b>
* Very difficult
* Difficult
* Neither difficult nor easy
* Easy
* Very easy

This is part of the 'Making ends meet' indicator from the Government of Canada and is measured in selected iterations of the Canadian Social Survey (CSS), the Survey Series on People and their Communities (SSPC), the Survey Series on First Nations People, Métis and Inuit (SSFNPMI) and in the Canadian Housing Survey (CHS).

This data currently covers 2021-2024 and was obtained from OpenOttawa, who made it available through a custom data request to Statistics Canada.
(https://open.ottawa.ca/datasets/ottawa::financial-security/about)

<b>**Note on Data Quality</b>: 
Data quality assessments are conducted by Statistics Canada prior to releasing custom tabulations. This dataset contain data entries with the following advisory warning:'Please use estimate with caution and refer to the confidence interval to assess its quality.'

## Examining the Data
The dataset is a csv file with 13 columns that outlined what percentage of each group responded to each of the categories on the survey question. I filtered the data to only see the results in English. There are 16 group types in total and I decided to focus on a set of them to see what financial security sentiments are like between the age groups, gender, racialized vs non racialized, and education level.


<img width="479" height="260" alt="image" src="https://github.com/user-attachments/assets/4e7aae70-1fb8-4623-a671-05b1b4feb1ae" />
<img width="510" height="311" alt="image" src="https://github.com/user-attachments/assets/9fd55dae-9dfb-4389-b281-ff071acd6334" />

### Concerns on Data Quality (especially 2021)
As you can see below, there is 24 warnings for data records in 2021 alone which means we have to take the results of that year with a grain of salt knowing it may not be accurate when we examine at the group levels. When you look at the confidence levels (F95lcl & F95ucl) there are large ranges between the lower and upper confidence meaning the percentage value of that group could be actually higher or lower than listed. I could have chosen to leave 2021 out entirely, but since there is limited data covering less than 5 years, I chose to keep it.  <br/><br/>
<img width="340" height="108" alt="image" src="https://github.com/user-attachments/assets/60b207f9-9718-463e-a26a-f0ecbb4cf0d6" />
<img width="732" height="757" alt="image" src="https://github.com/user-attachments/assets/9abe2cdc-5bed-4dbb-bb80-d3b2bea07233" />

## Examining 'All Persons' Financial Sentiment Across Years
Before drilling down into each group, let's examine the overall sentiment using the category 'All Persons'. In the graphs below, we can look at the percentage of people that selected each survey choice over the span of 2021-2024.

For 2021 results, we have to be wary of data accuracy but overall we can see a trend that is happening in each selection.
For 'Very Easy or Easy to Meet', there was a drop in the percentage of households in 2023 that selected this option, but the average between 2022-2024 sits around 34-39%. It's also interesting to note that when compared to the other choices, a majority percentage of households are indicating that it's 'Very Easy or Easy to Meet' their financial needs.

On the flipside, the 'Very Difficult or Difficult' selection is growing in the percentage of households selecting this option.  <br/><br/>
<img width="1007" height="407" alt="image" src="https://github.com/user-attachments/assets/8a80ee52-2de4-4887-b34a-3865e66eda6e" />

## Examining Financial Security Sentiment Between Age Groups

Diving deeper into the data, we want to see 'who' is indicating that it's easy to meet their household needs versus who is finding that it's becoming more difficult. To do so, I've set up a series of pie charts to examine the percentage of each age groups that have selected these options and how it may have changed over the years.

### Percentage of Age Groups that Feel They Meet Financial Needs Easily 

Consistenly across all 4 years, the age group that found it most easy to meet their financial needs are those 65 years and older. This is then followed by the 55 to 64 years age group, though not as strongly consistent.

The lowest percent age group that selected this choice for multiple years is 35 to 44 years old.

<img width="920" height="716" alt="image" src="https://github.com/user-attachments/assets/b8b357ef-b0c7-443f-ab13-77da79f164f6" />

### Percentage of Age Groups that Feel They Meet Financial Needs Neither Easily nor Hard

There are slight flunctuations that occur in the percentage of each age group that selected this option, where they will go up and down between the years, but overall there are no dramatic increases/decreases for a specific age group making it feel more neutral.

<img width="1023" height="724" alt="image" src="https://github.com/user-attachments/assets/d1a8a91f-d3f1-4bfe-bc4a-d563c5f22147" />

### Percentage of Age Groups that Feel They Meet Financial Needs with Difficulty

The age group that selected this sentiment the most and consistently across the 4 years are those 35 to 44 years old. The 65 years and older group and the 55 to 64 years old group see the least amount of percentage change throughout the years. 

<img width="945" height="723" alt="image" src="https://github.com/user-attachments/assets/752ba9f1-8fa7-450d-b6ec-8ea5e666ccf5" />

## Examining Financial Security Sentiment Between Genders

Next we'll look at the sentiment between genders indicated as 'Women+' and 'Men+'. It's important to highlight that the percentage of both gender categories added up will not equal 100%, as it may not include any other gender types that could have been indicated by the respondents under the survey option 'Or please specify' when asked 'What is your gender?'

On an overview level, Women+ have consistently found it more difficult to meet financial needs compared to Men+ over the years. However, there is an upward trend in the increasing percentage of Men+ that are finding it 'Very Difficult or Difficult' as well, with an interesting observation that both gender categories started to converge at 2024.

However, for both gender categories especially with Men+, a majority percentage of them indicate it's 'Very Easy or Easy' for their household to meet its financial needs compared to the percentage that responded with the other options.


<img width="1116" height="400" alt="image" src="https://github.com/user-attachments/assets/e38aa44e-0dc3-4a16-b7c9-fc4f8966876c" />

## Financial Security Sentiment Based on Education Level

Next up we'll see the breakdown percentage of respondants that selected each survey option according to their education level. There are 4 summarized categories that are based on the highest certificate, diploma or degree that the respondant had completed:
*  University above bachelor's level
*  Post-secondary certificate or diploma below the bachelor's level
*  High school diploma or below
*  Bachelor's degree

### % That Feel They Meet Financial Needs Easily - Education

For those that completed university above a bachelor's level, the percentage of them finding it easy to meet their financial needs has been decreasing over the 4 years, where by 2024 the percentage is the same as those who have just a bachelor's degree.

For majority of the years, the group with the smallest percentage of respondants that feel they meet financial needs easily are those that only have a post-secondary certificate or diploma below the bachelor's level.
<img width="995" height="835" alt="image" src="https://github.com/user-attachments/assets/665660de-237d-4a31-8707-457ee2fd7528" />

### % That Feel They Meet Financial Needs Neither Easily nor with Difficulty - Education

In 2021 and 2022, there were distinguishable differences in the percentages between the different levels of education, though starting in 2023 the gap between the levels had started closing and by 2024 they now all fall within a 31-35% range. It appears that there weren't any large percentage of a specific group based on educational level that held this sentiment more than others. 

<img width="1026" height="797" alt="image" src="https://github.com/user-attachments/assets/b457f64d-997b-4004-9044-d86baea940b8" />

### % That Feel They Meet Financial Needs with Difficulty - Education

From 2021 to 2024, all groups saw a degree of increase in the percentage of respondants indicating that they feel they meet financial needs with difficulty. The largest increase in percentage was seen in those with a Post-Secondary certificate or diploma below the bachelor's level, with 40% of them indicating difficulty in 2024.

The group with an educational level above a bachelor's level saw a large jump from 2022 to 2023, going up 8% in the percentage of respondents, while the percentage of people with high school diploma or below feeling financial difficulty remains relatively the same from 2022-2024.

<img width="995" height="843" alt="image" src="https://github.com/user-attachments/assets/cba88b2f-8df4-4c7e-ad7d-95405ec1addb" />

## Meeting Financial Needs for those Racialized vs Not Racilaized

Finally, the last group category we'll take a look at is those who are racialized (visible minority) compared to those who are not and see what the differences may be between these groups in their sense of financial security.

Those that find it 'Very easy or easy' to meet financial needs are predominantly Not Racialized; this is 38-45% from 2022-2024 compared to 23-26% of Racialized respondents feeling the same. Contrastly, those that found it neither easy nor difficulty or very difficult were predominantly racialized, though it's of interest to note how percentage of both groups are starting to overlap in feeling 'very difficult/difficult' in 2024. 

<img width="1223" height="440" alt="image" src="https://github.com/user-attachments/assets/a651e0e9-b064-4237-9a80-591e30f5e73e" />

## Conclusion

Summarizing the findings, there are some areas of note when examining the characteristics of respondents against the response option they chose when answering the survey question: 
"In the past 12 months, how difficult or easy was it for your household to meet its financial needs in terms of transportation, housing, food, clothing, and other necessary expenses?"

Those that answered 'Very Easy or Easy' were likely to be at least one of these categories:
* 65 years and older
* Male+
* Not Racialized
* Educational level obtained is Bachelor's or Above

Those that answered 'Very Difficult or Difficult' were likely to be at least one of these categories:
* 35 to 44 years old
* Women+
* Racialized
* Educational level obtained is Post-Secondary certificate or diploma below the bachelor's level, or High School Diploma

Though the majority percentage of respondants in total indicate that it's very easy/easy for their household to meet its financial needs, there was a  approximate 13% drop from 2021 to 2022 and another drop in 2023 before it saw a slight increase in 2024. As for the percentage of respondents that indicate it was very difficult/difficult, there's been an upward trend from 2021. This implies that after 2021, more households were finding it to be difficult to meet their financial needs or no longer found it as easy compared to previous years.

For the 65 years and older age group, this was the group with the highest percentage of respondents that found it easy to meet financial needs. I personally speculate that this is a group that's most likely to be retired and may have had years to accumulate wealth to support their current lifestyles. Their houses and cards could also potentially be paid off at this point, thus reducing a large part of reoccurring debt. 

Those that fall in the Women+ category made up a larger percentage of respondents that found it financially difficult in comparison to Men+, though it is interesting to note that by 2024, both groups were close to being the same percentage size. This similar overlap also occurred when examining racialized and not racialized groups. Though there was a gap between the two groups in 2022 and 2023, by 2024 both groups had similar percentages of respondents finding that it was financially difficult for them. The trend can be interpreted as households in total feeling more financially strained regardless of gender or racial background.

When examining education levels,the percentage of those that had a university education above a bachelor's level started becoming on par with those with a bachelor's degree in terms of respondents feeling that it was less easier to meet financial needs over the years. Despite having an education higher than a bachelor's, it does not seem like it made meeting financial needs any easier. However, for those that only have a Post-Secondary certificate or diploma below the bachelor's level or a high school diploma, they are consistently feeling more financial difficulty than those with higher education.

Overall a majority of respondents in the Ottawa/Gatineau region find it's very easy/easy to meet their household needs. However, looking at the trend from 2021-2024, there is a growing sentiment over the years of respondents finding it less easier to meet their household needs, so this sentiment could change in the next couple of years. The percentage that answer 'neither easy nor difficult' seems to remain in a consistent range while there is a growing trend of respondents finding it to be difficult. Though Women+ and those who are racialized have been in more financial difficulty throughout the years, their counterparts are starting to bear the same sentiment implying that everyone regardless of gender and race are feeling the same financial pressure. Those that are 35 to 44 years old feel the most financial difficulty, though the 45-54 year olds and 15-34 year olds follow closely behind making a population of those under 55 years old. I would be interested in seeing how this data develops over the next couple of years in a post-covid environment, along with the current rise of AI, political tensions, and job layoffs.






