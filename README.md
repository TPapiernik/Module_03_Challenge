# Module 03 Challenge - Election Audit

## Project Overview
A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election.

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes and percentage of votes each candidate received.
4. Determine the winner of the election based on popular vote.
5. Determine the counties in which votes were cast.
6. Calculate the total number of votes cast, by county, and the percentage of votes cast in each county.
7. Determine which county had the Largest Voter Turnout.

## Resources
- Data Source: election_results.csv
- Software: Python 3.7.6, Visual Studio Code 1.19.2

## Election-Audit Results
The analysis of the election show that:
1. There were 369,711 votes cast in the election.
2. The candidates were:
	-  Charles Casper Stockham
	-  Diana DeGette
	-  Raymon Anthony Doane
3. The candidate results were:
	-  Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
	-  Diana DeGette received 73.8% of the vote and 272,892 number of votes.
	-  Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
4. The winner of the election was:
	-  Diana DeGette, who received 73.8% of the vote and 272,892 number of votes.
5. The counties where votes were cast were:
	- Jefferson
	- Denver
	- Arapahoe
6. The county results were:
	- Jefferson County had 10.5% of the votes cast with 38,855 votes.
	- Denver County had 82.5% of the votes cast with 306,055 votes.
	- Arapahoe County had 6.7% of the votes cast with 24,801 votes.
7. The county with the Largest Voter Turnout was:
	- Denver County, which had 82.5% of the votes cast with 306,055 votes.

The Analysis Code to accomplish the stated Tasks requested in this analysis
was written in Python. It was written so as to provide output simultaneously
to the Terminal for immediate review, and to a text file on disk for storage
and later review. A quick glance of the identical outputs for these results can be seen below in
[Additional Resources](https://github.com/TPapiernik/Module_03_Challenge#additional-resources): Figure 1 for Terminal Output, and Figure 2 for File Output.

## Election-Audit Summary

This audit was completed with this specific congressional election in mind.
Using the available data, votes were tallied according to County and
Candidate, and output accordingly.

If a similar election was conducted, and a larger dataset was presented
where there were more Counties listed and more Candidates who received
votes, the current version of the code would take this into account without
modification. This is owing to the fact that the data is internally stored in a
Dictionary Data Structure. Each new row of input data is compared one-by-one
to see if the County or Candidate on that row is already present in the Dictionary.
If not, it is added accordingly and included in the analysis.

As a test of this functionality, the analysis source code was copied and modified
as `PyPoll_Challenge_TEST.py`, and the original `election_results.csv`
source file was copied and renamed `election_results_TEST.csv`.

To `election_results_TEST.csv`, beginning on line 100, 100,000 sample votes were added for ***TEST COUNTY*** and ***TEST CANDIDATE***, under ***Ballot ID: 0000000***. The analysis was re-run to output `election_results_TEST.txt`.

To see how these TEST VOTES affect the results, a screenshot of `election_results_TEST.txt` can be seen below in [Additional Resources](https://github.com/TPapiernik/Module_03_Challenge#additional-resources): Figure 3.

If a more complex election audit situation were to be taken into consideration, for instance if the dataset
also included statewide votes for Governor or Senator, the code would have to be modified
accordingly in order so that these votes would be tallied correctly according
to election rules.

One way to take this into consideration would be to add an additional Boolean `Statewide?` column to the `election_results.csv` Input File. The vote on a given row could be checked in an if statement and added to a separate set of Statewide Candidates and Votes Dictionaries. For further classification, a `Race Type` String Categorical column could also be added to take into account agreed-upon inputs such as **Congress**, **Senate**, **Governor**, etc. and these votes could be tallied separately by category.


## Additional Resources

Figure 1: Terminal Output Sample

![Figure 1](analysis/terminal_output.png "Figure 1: Terminal Output Sample")

Figure 2: File Output Sample

![Figure 2](analysis/file_output.png "Figure 2: File Output Sample")

Figure 3: Test Output for Additional County and Additional Candidate

![Figure 3](analysis/file_output_TEST.png "Figure 3: File Output TEST Sample")
