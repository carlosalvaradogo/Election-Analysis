# Election Audit

## Overview of Election Audit

### Complete an audit of a hypothetical local congressional election:

1. Calculate total votes.
2. Obtain list of all unique candidates.
3. Calculate number of votes received by each candidate.
4. Calculate "3." as a percentage of "1.".
5. Determine the winner of the election.
6. Obtain the list of all unique counties.
7. Calculate the number of votes received from each county.
8. Determine the county with most votes submitted.
9. Calculate "7." as a percentage of "1."

### Resources

- Data source: election_results.csv

- Software: Python 3.9.7 and Visual Studio Code 1.60.0

## Election Audit Results

-How many votes were cast in this congressional election?
 - Total votes: 369,711

-Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct:        
 -  Jefferson: 10.5% (38,855)
 -  Denver: 82.8% (306,055)
 -  Arapahoe: 6.7% (24,801)

-Which county had the largest number of votes?
 - Denver

-Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct:        
 - Charles Casper Stockham: 23.0% (85,213)
 - Diana DeGette: 73.8% (272,892)
 - Raymon Anthony Doane: 3.1% (11,606)

-Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
 - The winner of the hypothetical election was Diana DeGette with 272,982 total votes received, which are 73.8% of the total vote count.

## Election Audit Summary

Two ways in which the election commision can modify PyPoll_Challenge.py script to adapt it to diferent elections are:

1. Modifying the following command such that a different data source (for any other election) may be accomodated, insofar as the data source is in ".csv" format:

```
# Open the election results and read the file.
with open(file_to_load) as election_data:

    file_reader = csv.reader(election_data)
```

2. Modifying the following commands such that different a different message may be printed on a text file, depending on the interests of any given election:

```
    with open(file_to_save, "w") as txt_file:

        # Print the final vote count to the terminal.
        election_results = (
            f"\nElection Results\n"
            f"-------------------------\n"
            f"Total Votes: {total_votes:,}\n"
            f"-------------------------\n")
        print(election_results, end="")
```

