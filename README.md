# Keyword-Search

You need to log in to Google first because, after all, we ask Google Trends for trending topics. For that, we need to import the method called TrendReq from the pytrends.request method:

## pytrends

Unofficial API for Google Trends

Allows simple interface for automating downloading of reports from Google Trends. Only good until Google changes their backend again :-P. When that happens feel free to contribute!

## Installation
pip install pytrends
## Requirements
Written for Python 3.3+
Requires Requests, lxml, Pandas

## API Methods
The following API methods are available:

Interest Over Time: returns historical, indexed data for when the keyword was searched most as shown on Google Trends' Interest Over Time section.

Historical Hourly Interest: returns historical, indexed, hourly data for when the keyword was searched most as shown on Google Trends' Interest Over Time section. It sends multiple requests to Google, each retrieving one week of hourly data. It seems like this would be the only way to get historical, hourly data.

Interest by Region: returns data for where the keyword is most searched as shown on Google Trends' Interest by Region section.

Related Topics: returns data for the related keywords to a provided keyword shown on Google Trends' Related Topics section.

Related Queries: returns data for the related keywords to a provided keyword shown on Google Trends' Related Queries section.

Trending Searches: returns data for latest trending searches shown on Google Trends' Trending Searches section.

Top Charts: returns the data for a given topic shown in Google Trends' Top Charts section.

Suggestions: returns a list of additional suggested keywords that can be used to refine a trend search.

## Top Charts
pytrends.top_charts(date, hl='en-US', tz=300, geo='GLOBAL')

### Parameters
date
Required
YYYY integer
Example 2019 for the year 2019 Top Chart data
Note Google removed support for monthly queries (e.g. YYYY-MM)
Note Google does not return data for the current year

# Keyword Interest By Region

Let’s see the terms that are popular in the region around the world. I will choose the term to search for as “Data Science”:

Values ​​are calculated on a scale of 0 to 100, where 100 is the most popular location as a fraction of the total searches for that location, a value of 50 indicates a location half as popular. Now let’s visualize the above search results to get better insights

# Keyword Research with Python for Daily Search Trends

Now let’s take a look at the top daily search trends around the world. To do this, we need to use the trending_searches () method


## Credits
Major JSON revision ideas taken from pat310's JavaScript library

https://github.com/pat310/google-trends-api
Connecting to google code heavily based off Stack Overflow post

http://stackoverflow.com/questions/6754709/logging-in-to-google-using-python
With some ideas pulled from Matt Reid's Google Trends API

https://bitbucket.org/mattreid9956/google-trend-api/overview
