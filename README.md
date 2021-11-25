# Election_Analysis
A quantitative look into this election's votes using Python and VS Code

Overview of Election Audit

  The purpose of this analysis was to output the following results from this election: the total number of votes; broken down into the number of votes for each county specifically, the county with the largest turnout, each candidate’s voter county and lastly, the final count for the winner of the election.
  
  The code formulated for each of the above listed calculations will allow the election commission to see figures in numerical form as well as percentage for each candidate and each county. This data also makes it simpler for the election commission to display the results visually, i.e., a pie chart for votes for received in each county. 
  
Election Audit Results

-	Election Results: 369,711
  To derive the total number of votes as show above, each row was read in the election_results.csv file and added to the total count of votes.

-	 County Votes:
Jefferson: 10.5% total votes: 38855
Denver: 82.8% total votes: 306055
Arapahoe: 6.7% total votes: 24801

   To derive the total number of votes for each individual county, a county dictionary was initialized at the beginning of our code.

![image](https://user-images.githubusercontent.com/93355719/143370732-253fb1e9-2d39-44de-a4fd-9dcf7a59d715.png)

This dictionary was later used in conjunction with the “county” variable to output the number of votes calculated for each county i.e., = votes. Once the total number of votes was calculated for each county, we could then calculate the percentage. This was done by using the following calculation for the [1] variable in each row:  “votes” by “total_votes” x 100(%).

-	Largest County Turnout: Denver

  The largest county turnout would be the county with the highest number of votes. This was calculated by using the “.format” function to replace the placeholder in the string with the “largest_county” (“Python format() Function”, Python String format() Method (w3schools.com)).


-	Candidate Votes
Charles Casper Stockham: 23.0% (85,213)
Diana DeGette: 73.8% (272,892)
Raymon Anthony Doane: 3.1% (11,606)

  The number of candidate votes were calculated using the “candidate_votes” dictionary established at the beginning of the code. To calculate the percentage amount for each of the candidates’ votes, the “.get” function is used to obtain the votes for each of the candidate names (“Python Dictionary get() Method”, Python Dictionary get() Method (w3schools.com)).


-	Winner: Diana DeGette
Winning Vote Count: 272,892
Winning Percentage: 73.8%

	The calculation for the winner’s results was determined by comparing the “votes” and “vote_percentage” to the “winning_count” and the “winning_percentage”.

Election Audit Summary

  The framework of this election analysis is quite versatile, as with a few changes made to the data, this can be used for other elections too. For example, by altering the “election_results.csv” file and our txt file used with another set of election data; we can easily generate results for other counties and candidates. Also, when obtaining the county and candidate name from each row, if there are other variables, we can alter the position the variable is at in that row. 
  
  For example: 
![image](https://user-images.githubusercontent.com/93355719/143371244-18360ecb-3242-4808-880a-605c61d069cb.png)
