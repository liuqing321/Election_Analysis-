# Election_Analysis

## Purpose of the Election Audit 

To assist two employees from board of election, we are going to automate the process of counting the votes for each candidate by using Python. Additionally, we will automate the process of calculating the voter turnout for each county and the percentage of votes from each county out of the total count. Finally, all the calculation results alone with the highest turnout will be printed on the .txt file. 

## Election Result

![Result](https://user-images.githubusercontent.com/88631769/133356218-e45c4f26-1d75-43e8-b383-cf47e726d911.PNG)


- Total votes were cast in this congressional election. 

	
	The total votes cast in this this congressional election is 369,711. 


- The breakdown of the number of votes and the percentage of total votes for each county in the precinct.
     
	
	
	Jefferson: 10.5% (38,855)

	Denver: 82.8% (306,055)

	Arapahoe: 6.7% (24,801)


- The county with the largest number of votes. 
    
	
	
	The largest county Turnout is Denver. 



- The breakdown of the number of votes and the percentage of the total votes each candidate received.


	Charles Casper Stockham: 23.0% (85,213)

	Diana DeGette: 73.8% (272,892)

	Raymon Anthony Doane: 3.1% (11,606)


- The candidate won the the election. 
   

	The winner is Diana DeGette. Her winning vote count is 272,892 and her winning percentage is 73.8%. 



## Election-Audit Summary
  
    
- By changing the value for "file to load" and "file to save", the script could be used to process any file that has the same data frame as "election-results.csv". No matter how many candidates or counties are in the new file. The two "if-statements" will help the board of election add new value in the candidate list and the county list. 
 	
		#Add a variable to load a file from a path.
    	file_to_load = os.path.join("Resources", "election_results2021.csv")
    	#Add a variable to save the file to a path.
    	file_to_save = os.path.join("analysis", "election_report2021.txt")


- The output that going to be printed on the .txt file could be changed. For example, we could add or change the state information in the script below, 

      	# Print the final vote count (to terminal)
    	election_results = (
        	f"\n Election Results - Maryland\n"
        	f"-------------------------\n"
        	f"Total Votes: {total_votes:,}\n"
        	f"-------------------------\n\n"
        	f"County Votes:\n")
    	print(election_results, end="")

 		txt_file.write(election_results)
    
