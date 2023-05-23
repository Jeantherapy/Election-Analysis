# Election-Analysis
## Election overview
 A Colorado Board of Elections has requested to complete the election audit of a recent local congressional election. The overview gives a comprehensive summary of the election results, highlighting the county with the highest turnout and the candidate who secured the most votes. Below is list of questions to be answered.

* 1 Calculate the total number of votes cast.
* 2 Get a complete list of candidates who received votes.
* 3 Calculatae the total number of votes each candidate received.
* 4 Calculate the total number of votes each candidate received.
* 5 Calculate the percentage of votes each candidate won.
* 6 Determine the winner of the election based on popular vote.
## Resources
  * Data Source: A csv file, election_results.csv
  * Software: python and VScode

## Election Results
### Total number of votes
-------------------------
* Total Votes: 369,711
-------------------------

### Candidates and Percentage of Votes:
-------------------------

* Charles Casper Stockham: 23.0% (85,213)

* Diana DeGette: 73.8% (272,892)

* Raymon Anthony Doane: 3.1% (11,606)

### The winner of the election based on vote received
-------------------------
* Winner: Diana DeGette
* Winning Vote Count: 272,892
* *inning Percentage: 73.8%
-------------------------
## Summary
The code provided performs an analysis of election results from a CSV file and generates a summary of the findings. Here is a summary of the code's functionality:

1. The code begins by importing the necessary dependencies and setting the file paths for the input data and output analysis file.

2. It initializes variables for tracking the total votes, candidate options, candidate votes, county options, county votes, and variables for tracking the winning candidate and county.

3. The code reads the CSV file using the `csv.reader` and skips the header row.

4. For each row in the CSV file, it increments the total vote count, retrieves the candidate name and county name from the row, and performs the following actions:
   - If the candidate name is not in the candidate options list, it adds the candidate name to the list and initializes their vote count to 0.
   - It increments the candidate's vote count by 1.
   - If the county name is not in the county options list, it adds the county name to the list and initializes its vote count to 0.
   - It increments the county's vote count by 1.

5. The code opens the output analysis file in write mode and starts writing the analysis results to it.

6. It begins by printing and writing the overall election results, including the total vote count and a header for county votes.

7. It enters a loop to calculate and print the county-specific results:
   - It retrieves the county vote count and calculates the percentage of votes for the county.
   - It prints and writes the county results to the terminal and analysis file.
   - It checks if the current county has a higher vote count and percentage than the previous winning county and updates the winning county variables if necessary.

8. After the loop, the code prints and writes the summary of the county with the largest turnout to the terminal and analysis file.

9. It then proceeds to calculate and print the percentage of votes for each candidate:
   - It retrieves the candidate vote count and calculates the percentage of votes for the candidate.
   - It prints and writes the candidate results to the terminal and analysis file.
   - It checks if the current candidate has a higher vote count and percentage than the previous winning candidate and updates the winning candidate variables if necessary.

10. Finally, the code prints and writes the summary of the winning candidate to the terminal and analysis file.

This code provides a comprehensive analysis of the election results, including the overall vote count, county-specific results, and candidate-specific results. It identifies the county with the largest turnout and determines the winning candidate based on the highest vote count and percentage. The results are both printed to the terminal and saved to a text file for further reference.