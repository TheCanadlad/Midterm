**November 8th,2024**<br>
**CMN4100 Digital Journalism**<br>
**Tyler Beauchesne**<br>
**Presented to Jean-Sébastien Marier**<br>

# Midterm Project: Exploratory Data Analysis (EDA)

# ReadMe.MD


## 1. Introduction

I will analyze the City of Ottawa's 2024 Service Requests report for a potential story. The City of Ottawa is the source and they collected the data through tracking Bylaw cases and calls. I will analyze the number of calls completed or canceled per Bylaw service in the city. I want to see which sectors are the most successful and which ones are the least successful when it comes to finishing requests. I think this is a great topic to pick as I want to evaluate the numbers on these polls as much as possible. Then once I have the answer to my question from a statistical standpoint, then I will take it to another level. I will investigate why the reasoning behind these numbers are and get professionals to comment on what the solution can be to fix these problems. Their advice will play a big role into this story as much as the data. With all of these factors, I will be able to form a well-written and coherent story. 

## 2. Getting Data

I got the data from going directly to the City of Ottawa site. I downloaded the CSV and uploaded it to the Google sheet I created for this project. There are about 12 rows and 274,310 columns in the report to fully analyze the data. The first column is the case number and the eighth one is ward which are ordinal values. The fifth one is called type and sixth one is called description which are nominal values (Government of Canada, Statistics Canada, 2021).The data does not look clean to me as each column has a distinctive purpose but some are placed in odd areas. For example, the status column is the second column of the spreadsheet. It comes before the type and description columns which I believe should be in front of the status column. This is because it would make more sense to myself as I analyze it. Also the channel section should not be at the end and should actually be before status as well. That way, analyzing all the details that I need will be a lot easier. I noticed on the spreadsheet that some cells had addresses on it and others did not. That column feels very useless if all the calls do not have the address information and should be removed. Why do the columns looks so misarranged? Spreadsheet: https://docs.google.com/spreadsheets/d/1VTvOq304Aeky0OwXe_cIC7r9bvxyxcl7YfZKEVyHUGI/edit?usp=sharing

![](Datasheet.png)<br>
*Figure 1: This is the Data on Google Sheets.*

## 3. Understanding Data

The dataset, a 311 call log for service requests in the current year, offers a comprehensive view of city services. Each record includes details such as service type, status, dates, location, ward, and the channel through which the request was submitted. With 274,308 records and 11 columns, the data provides insights into the city's operational demands and efficiencies. 

### 3.1. VIMO Analysis

The VIMO analysis showed me a lot of interesting things. The volume was quite a lot for this data sheet as with 274,308 rows, it provided a large sample of service requests, capturing various service types across multiple city wards. The key columns in this datasheet include Type, Status, and Ward. The Channel column shows request submission methods, which also provides volume-based insights into resident engagement through each method(Government of Canada, 2021). The intensity captured the request density across service types, locations, and wards. For example, identifying the wards with a high number of requests may suggest those are the areas with higher service needs. The temporal trends show that the momentum assesses how requests change over time, showing the seasonality or shifts in demand. By analyzing the Opened Date and Closed Date sections, I can identify periods with increased requests such as snow removal in the winter. If “Bylaw Services” requests peak during the summer due to the increased outdoor activities, the city can pre-emptively allocate resources to meet these seasonal demands. The opportunity that I saw was that there could be some operational improvement. The opportunity highlights potential enhancements in service processes, such as improving response times. Calculating request resolution times by comparing the Opened Date and Closed Date columns can reveal efficiencies or delays. If web-submitted requests have faster resolution times than phone submissions, the city could encourage the web-based requests to streamline operations.

Support your claims by citing relevant sources. Please follow [APA guidelines for in-text citations](https://apastyle.apa.org/style-grammar-guidelines/citations).

**For example:**


### 3.2. Cleaning Data

All of the columns have been loaded as objects due to having mixed or missing values in their cells in fields like Latitude and Longitude.  That is a lot of work for this for a statistic that does not matter as much so I just deleted them to make it easier on myself. There was also a lot of white space I had to remove to make the chart look nicer. I froze the top row to make sorting the data by date easier as the top row was not moviing as much (Marier). 

![](Cleanup.png)<br>
*Figure 1: This is the clean data on Google Sheets.*

### 3.3. Exploratory Data Analysis (EDA)

The VIMO analysis and data cleaning steps I took revealed that the dataset have a lot of operational insights but required a careful handling of the missing values and categorical encoding to maximize the usefulness of the data. Certain wards may experience a higher concentration of requests compared to others, indicating that the areas where resource allocation might need proper adjustment to meet demand equitably. This data highlights a lot of potential for optimizing request channels and reducing resolution times by focusing on web-based submissions. These findings that come from the data could guide policy decisions to improve the city services, address the areas with the highest service demand, and potentially streamline operations for a more efficient response to residents’ needs. 

![](pivottable.png)<br>
*Figure 2: This pivot table shows how much more simplified the data can be*

I created a pivot table to count the number of requests per Type. This setup highlights the distribution of request types and their resolution statuses, allowing us to identify categories with high numbers of unresolved cases. 


![](chart.png)<br>
*Figure 3: This exploratory chart shows the frequency in each sector*

I created a bar chart for the data to analyze the number of calls. Some of the things that I found in the chart was that "Garbage and Recycling" and "Bylaw Services" had the highest number of requests, with “Garbage and Recycling” achieving the highest rate. Categories with a high proportion of unresolved cases may need additional resources. I created a bar chart to visualize the request types by volume.  The chart revealed that some types, like “Garbage and Recycling and Bylaw Services”, are used more than others. This finding also suggests that areas where service process improvements could reduce the open cases. The calculated difference between Opened Date and Closed Date could reveal the average handling times by request type which is an interesting concept to research. The long resolution times may highlight the inefficiencies in certain services. By analyzing the request density by ward, we can identify the areas with high service demand and assess whether these areas receive proportionate service attention. I was examining the correlation between request resolution time and the submission channel could suggest that promoting certain channels like web requests might streamline service handling. What I learned here is that Garbage and Recycling was the biggest issue in the city and that some cases just get closed with no follow-up. The cases that are closed with no resolution is the one that warrented an investigation.

## 4. Potential Story

The potential story here is to identify the types of calls that Bylaw receives and evaluate why some calls gets finished and others do not. The story is very interesting to me because you would hope that Bylaw would resolve every call as much as possible. So, if a call cannot be resolved then I need to find out what aspects stop some of them from being completed. This article by CTV News Ottawa is a good source for me as it explores how the workload for bylaw requests has grown in the last year. As stated before, some of the wards have been experiencing a higher volume of requests than other wards. This has to indicate that some areas might need adjustment to how resources are being used to meet the expected demand. I want to also look at holidays to see if the volume of calls increase by a lot with this CTV News Ottawa story as a source as a start. I would like to interview people who work for Bylaw or represent them for this story. I think their insight into this would be the most valuable for this topic as some of them had to deal with these calls directly.

## 5. Conclusion

My thought process when finishing this assignment was that it was going to be difficult and timely. However, if I had the right mindset, then I would be able to complete the assignment to the best of my ability. The most challenging part of the assignment was completing the understanding data section of the assignment. Not just because of the word length but because of how complicated the process was for me. I struggled with the process when doing this assignment, so I tried to find as much help as possible. I used ChatGPT as an analysis tool. It was meant to help with my understanding with the process of data analysis as I had a hard time with it. It was also challenging to go through each part of the assignment as a gap in my knowledge with missing two or three things but I got them all in the end. The most rewarding aspect was figuring out how to clean the data myself as it felt like such an achievement. I have struggling with this all year and it felt good to finish. I have identified the gaps in my knowledge when it comes to data cleaning and sorting, but I was able to figure it out with some help. I could have gone to my professor about my difficulty before using AI and that is something I will work on for next time.

## 6. References

Eltherington, W. (2024, July 2). Ottawa bylaw receives over 100 complaints for fireworks, noise on Canada day. CTV News Ottawa. https://ottawa.ctvnews.ca/ottawa-bylaw-receives-over-100-complaints-for-fireworks-noise-on-canada-day-1.6948664 
Government of Canada, S. C. (2021, October 22). Data journey. Government of Canada, Statistics Canada. https://www.statcan.gc.ca/en/wtc/data-literacy/journey 
Government of Canada, S. C. (2021, October 22). Data journey. Government of Canada, Statistics Canada. https://www.statcan.gc.ca/en/wtc/data-literacy/journey
Government of Canada, Statistics Canada. (2021, September 2). Statistics: Power from data! https://www150.statcan.gc.ca/n1/edu/power-pouvoir/toc-tdm/5214718-eng.htm 
Marier, J.-S. (n.d.). Cleaning Data in Google Sheets. YouTube. https://youtu.be/Gr5FdvNf0I0 
OpenAI. (2024). ChatGPT [Large language model]. https://chatgpt.com 
Raymond, T. (2024, May 18). Workload concerns could prompt call for more bylaw officers in Ottawa. CTV News Ottawa. https://ottawa.ctvnews.ca/workload-concerns-could-prompt-call-for-more-bylaw-officers-in-ottawa-1.6892348


# git config --global user.email "beauchesne.tyler@gmail.com"
# git config --global user.name "TheCanadlad" 