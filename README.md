# INST216-Project-3
#### Group 32: Matthew Marston

## Plan of Action
According to the problem statement I must analyze a user log and generate automated reports. Each log contains a date, time, activity, server and user email id. To stay organized and keep track of what elements go with what logs, I believe dictionaries will be very useful. By using a nested dictionary I can refer to each log by their index and retrieve the date, time, etc. associated with it. This will also make it easy to run loops scanning whether a person has logged in 5 or more times, if they haven't logged out, or if they logged out more than they've logged in. If I find a hit, I can use a list or dictionary to log their information.  In addition, I will use functions for operations I use throughout the reports to simplify the process. With this in mind, all I will have left to do is format the output which I can easily do using f-strings, .join(), etc.

## Project Description
### Suspicious activities (suspicious_report.txt)

If any user logs into any of the systems more than 5 times in a single day, or if the user logs into any of the systems even once between 12:00 am to 5:00 am, it is marked as suspicious behavior. 

You must report the total count of suspicious activities.
Suspicious behavior for a user on one day accounts for a total count of 1.
Hence, total cases will be a sum of all the suspicious days for all the users.
The total number of cases for each individual user will be the number of all the suspicious days for that user.
All the time, activity, and server information for the particular days for each user must be listed in the ascending order, sorted on the basis of time.

## Irresponsible behavior (irresponsible_report.txt)

The user is expected to logout every time he/she logs in to any of the systems. So if the user forgets to logout after logging in, it is considered an irresponsible behavior. To keep it simple, you can check if the number of logins is more than the number of logouts for a particular user on a given day, it can be tagged as an irresponsible activity.

You must report the total count of irresponsible activities.
Irresponsible activities for a user on one day account for a total count of 1.
Hence, total cases will be a sum of all the days when any user was irresponsible.
The total number of cases for each individual user will be the number of days when that particular user was irresponsible.
All the time, activity, and server information for the particular days for each user must be listed in the ascending order, sorted on the basis of time.

## System glitch (glitch_report.txt)

On the contrary to the previous behavior, if the system records more number of logouts than the number of logins for any user, we flag it as a system glitch as this is not practically possible.

You must report the total count of the system glitches.
Glitches for a user on one day account for a total count of 1.
Hence, total cases will be a sum of all the days when there was a glitch for any user.
The total number of cases for each individual user will be the number of days when that particular user faced a glitch.
All the time, activity, and server information for the particular days for each user must be listed in the ascending order, sorted on the basis of time.

##  Domain count (domain_report.txt)

A list of all the unique domains and the number of users registered within each domain.
NOTE: The domain name of a particular user can be found by checking the second part of their email-id.
NOTE: "Unique domains" mean that each domain name should occur only once in this list.

Example:

Email-ID:       sample.user@domain.abc
Name:           sample.user
Domain name:    domain.abc
