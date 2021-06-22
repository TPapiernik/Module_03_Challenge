# Module 03 Challenge - Election Audit

## Project Overview
A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election.

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.
6. Calculate the total number of votes cast, by county.
7. Calculate the percentage of votes cast in each county.
8. Determine which county had the Largest Voter Turnout.

## Resources
- Data Source: election_results.csv
- Software: Python 3.7.6, Visual Studio Code 1.19.2

## Election-Audit Results
The analysis of the election show that:
- There were 369,711 votes cast in the election.
- The candidates were:
  -  Charles Casper Stockham
  -  Diana DeGette
  -  Raymon Anthony Doane
- The candidate results were:
  -  Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
  -  Diana DeGette received 73.8% of the vote and 272,892 number of votes.
  -  Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
- The winner of the election was:
  -  Diana DeGette, who received 73.8% of the vote and 272,892 number of votes.
- The counties where votes were cast were:
	- Jefferson
	- Denver
	- Arapahoe
- The county results were:
	- Jefferson County had 10.5% of the votes cast with 38,855 votes.
	- Denver County had 82.5% of the votes cast with 306,055 votes.
	- Arapahoe County had 6.7% of the votes cast with 24,801 votes.
- The county with the Largest Voter Turnout was:
	- Denver County, which had 82.5% of the votes cast with 306,055 votes.

## Election-Audit Summary

This audit was completed with this specific congressional election in mind.
Using the available data, votes were tallied according to County and
Candidate.

If a larger dataset was presented, for example, for elections conducted
in multiple congressional districts, this script could be modified to
tally results for that larger dataset as well. An additional section
could be added to the code to find the congressional districts listed,
and then perform this same analysis for each district in turn.

If different election types were listed in the same dataset, for instance,
both congressional races and a statewide gubernatorial race, the votes for
those elections could be tallied separately, according to which election
the votes were cast.
