# FinalPeerEvaluation
A Peer Evaluation System that compiles relative scores for students.

The system works by gathering information from a spreadsheet (generated by a google form), then compiling peer reviews by team member in each team.  The Team average is calculated, and a relative score is calculated for each student based on the team average.  For example, if the team average is 4.3, and a student review average is 4.0, their relative score is 0.93.  

1. Setup a Google Form [similar to this one](https://docs.google.com/forms/d/e/1FAIpQLSffAJ7zvew-gWxjKDbC9K7qLpyXIX3uMhezwJIBoZeSEusz_g/viewform?usp=sf_link).  If you modify the order or types of questions asked, the associated script will need to be modified.

2. Post a copy of the form to your courses, modifying to include the correct student names, which you can copy and paste from the course roster.

3. After the deadline, download a *.csv version of the responses.  You'll need to save the file as an *.xlsx.  

4. Install [Python 3.x](https://www.python.org/) and [Openpyxl](https://openpyxl.readthedocs.io/en/stable/). Download the Peer Analysis Script. 

5.  Make sure the script and excel file are in the same directory.  Edit the script line 
```
Analysis = PeerAnalysis("Peer Evaluation SP18.xlsx")
```

6. The output will be written to a csv file given in the `Analysis.writeout("FSE100A_PeerScales.csv")` line.  
