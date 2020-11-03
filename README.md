# INST216-Project-3
#### Group 32: Matthew Marston

## Plan of Action
According to the problem statement I must analyze a user log and generate automated reports. Each log contains a date, time, activity, server and user email id. To stay organized and keep track of what elements go with what logs, I believe dictionaries will be very useful. By using a nested dictionary I can refer to each log by their index and retrieve the date, time, etc. associated with it. This will also make it easy to run loops scanning whether a person has logged in 5 or more times, if they haven't logged out, or if they logged out more than they've logged in. If I find a hit, I can use a list or dictionary to log their information.  In addition, I will use functions for operations I use throughout the reports to simplify the process. With this in mind, all I will have left to do is format the output which I can easily do using f-strings, .join(), etc.

## Project Description
### Suspicious activities (suspicious_report.txt)

## If any user logs into any of the systems more than 5 times in a single day, or if the user logs into any of the systems even once between 12:00 am to 5:00 am, it is marked as suspicious behavior. 

You must report the total count of suspicious activities.
Suspicious behavior for a user on one day accounts for a total count of 1.
Hence, total cases will be a sum of all the suspicious days for all the users.
The total number of cases for each individual user will be the number of all the suspicious days for that user.
All the time, activity, and server information for the particular days for each user must be listed in the ascending order, sorted on the basis of time.
