#  WeRateDogs Dog exploration
## by Ibukun Irinyenikan

This project analysed data collected from WeRateDogs twitter account.
There were three sources  in which the data were gathered. The first dataset, 
twitter_archive_enhanced was collected in CSV format provided by Udacity. 
The second dataset was 
in a tab separated value (TSV) format. It was collected programmatically through a URL link provided 
by Udacity. The requests library was used to extract the data from the web. Thirdly, 
the third dataset 
was to be collected through twitter API. However, I collected the data from the json file provided by 
Udacity. The pandas read_json method was used to read the data to the dataframe.

The data was acccessed and cleaned for both quality and tidyness issues. 
I ensured that every single issue, both quality and tidiness issues 
highlighted above were cleaned. But before I started the cleaning process, 
I made a copy of the three datasets. and named them archive_clean, image_clean and tweet_clean.
After cleaning all data, I merged all the three datasets into a combined form. Then, all the columns 
that will not be useful for my exploration were dropped. I ended up having a total of 5 columns and 
1,666 rows of data.
This master dataset is stored as a CSV file called twitter_archive_master.csv.



## Summary of Findings

There are two groups of dogs explored in the analysis. I referred to one group of dogs as good dogs 
and the other group as bad dogs. The bad dogs are not really bad. It’s only for analysis purpose. I will 
explain further below.
Groups of Dogs:
• Good dogs in the analysis are dogs that are rated 10 and above.
• Bad dogs are dogs that are given ratings below 10

On exploration, I found that the there is a positive correlation between the total number of 
likes and retweets of dog tweets among dog lovers. dog lovers tend to retweet the dog tweets that they liked more. 
They are more likely to retweet a dog tweet when they like it.
There is also a positive correlation between the dog ratings and total number of likes among dog lovers. 
The higher the dog rating, the higher the number of likes.
Dog lovers liked Lakeland Terrier breed the most. 
Note that this record is only for dog lovers that hit the like button on Lakeland Terrier breed.

## Key Insights for Presentation
- Dog with high ratings tend to be liked and retweeted more by dog lovers.

  Dogs with low ratings are retweeted less by dog lovers.
  
- Dog lovers sentiment seem to agree with the ratings of the dog poster.

- It appears that if the dog rating is very low or below 10, it’s more likely to be retweeted and liked less by dog lovers.



## Limitation
- In this project, the retweet date of dogs ratings were not explored. 

- It’s important to know that the number of followers WeRateDogs have at the time of tweeting could 
 impact the number of likes and retweets.
 
- Dogs posted in 2016 and 2017 are more likely to have more likes than dogs posted in 2015. That’s 
 because the number of followers has multiplied over the years.
 
- Dogs posted in 2015 are more likely to receive low reactions because the account was created in the 
 same year. Hence, I couldn’t draw conclusions on such dogs.

##### PS: You can find the data wrangling and data exploration documentation in the wrangle_report and act_report file included with this project. 