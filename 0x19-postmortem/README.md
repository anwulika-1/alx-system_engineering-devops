![images (5)](https://github.com/anwulika-1/alx-system_engineering-devops/assets/111018929/d23bc861-d2ef-4279-84ca-1d56e3e4b497)
![images (6)](https://github.com/anwulika-1/alx-system_engineering-devops/assets/111018929/c4b57282-67e6-4ce0-b5fd-507a5198d675)


https://medium.com/@anwulikahappinex/issue-summary-78bb8e90dcbd


Issue Summary
From 10:30 PM to 8:30 AM, Company B experienced an outage on Cloud B that affected www.companyB.com due to a prescheduled reboot that ended in failure. The points of failure are coming from the rebooting of the load balancer or cache server. The Security Team issued a maintenance update and a reboot notification to a major Cloud B server on May 2, 2023 for a window of 5hours (10:30 to 3:30 AM). 

Timeline (all times in Pacific Time)
9:30 PM: Reboot begins
10:30 PM: Outage begins
11:26 PM: Alerts sent to teams
12:30 AM: Lead SRE silenced all subsequent alerts due to server behavior being “normal”
1:30 AM: Server down and customers can’t reach the site

Root Cause
At 5:26 AM, the reboot of the load-balancer or cache server continued to fail. The secondary server did not come back up for for 3 hours. We did not expect the scheduled reboot to affect our systems. 

Corrective and Preventative Measures
In the last 3 days, we’ve made an internal review and analysis of the outage. The following measures are actions the team will follow for prevention and to improve response times in the future.
The database server provider during the performance degradation could have alerted teams the down server . It was updated to their systems to prevent further issues in the future are done accordingly.
