# IT Helpdesk Dashboard Analysis

This repository contains an IT Helpdesk Dashboard analysis focused on identifying operational inefficiencies within an IT ticketing system and proposing actionable solutions. The dataset comprises approximately 97,000 rows of IT tickets, detailing various issues and their attributes. Here's the link to the interactive Power BI Dashboard [Link](https://app.powerbi.com/view?r=eyJrIjoiZThhZTkxZWUtOTA3ZC00YzhiLThiMTAtMDJmMzc5M2ZjOTFjIiwidCI6IjAzNWEyYzY4LTc2YjQtNGViYS1hMTVhLWNiYmNhOTY4NjhjZCJ9)

Context:
The IT manager tasked me with analyzing the ticketing system to uncover inefficiencies, with the goal of reducing resolution times, enhancing customer satisfaction, and improving overall service quality.

Dataset:  
Tickets Table: Includes columns for date, ticket ID, priority, severity, issue type, agent ID, satisfaction rating, request category, and resolution time.  

IT Agents Table: Contains agent ID, full name, email, and date of birth (DOB).

Feature Engineering:
To enhance the analysis, I derived the following:  
- An age column calculated as 2025 minus the year of birth from the DOB column.  

- An independent date table to support robust time-series analysis.

Analysis:
The dataset was well-structured, requiring minimal cleaning. Using DAX, I created key measures to evaluate performance, including:  
- Total tickets  

- Average satisfaction rating  

- Average resolution time  

- Total agents  

- Tickets resolved within the Service Level Agreement (SLA) threshold of ≤3 days

Insights:  
- Ticket Volume: A total of 97,000 tickets were analyzed, with 39,000 system-related, 29,000 login access, 20,000 software, and 10,000 hardware-related tickets.  

Key Performance Indicators (KPIs):  
- 50 agents handled 97,000 tickets.  

- Average resolution time: 4.55 days.  

- SLA compliance: 48.2% of tickets resolved within ≤3 days.  

- Average satisfaction rating: 4.10/5.

Ticket Categories:  
- IT Requests (75% of tickets) and IT Errors (25%).  

- System and hardware tickets had the longest resolution times, averaging 7.50 days for system tickets, with only 11% SLA compliance (10,600 tickets resolved within ≤3 days).  

- Login access tickets had the fastest resolution time (0.33 days, ~7 hours) and the highest SLA compliance (99%) across both categories.

Trends:  
- Ticket volume grew steadily from 13,000 in 2016 to 29,000 in 2020.  

- Ticket priority distribution: 36,000 high, 16,000 medium, 17,000 low, and 29,000 unassigned.  

- Longer resolution times correlated with lower satisfaction ratings.

Agent Performance: Identified the top 5 and bottom 5 agents by satisfaction ratings and tickets handled.

Recommendations:  
1.Category-Specific SLAs: Implement stricter SLAs for system and hardware tickets to address prolonged resolution times, which may negatively impact satisfaction ratings.  

2.Agent Training: Provide targeted training for agents handling system and hardware tickets to improve efficiency and SLA compliance.  

3.Priority Refinement: Review and standardize the ticket prioritization process, as 29,000 unassigned tickets suggest inconsistencies.  

4.Process Optimization for Login Access: Replicate the efficient processes used for login access tickets across other categories to boost overall performance.  

5.Performance Monitoring: Regularly track agent performance and provide feedback to sustain high satisfaction ratings and resolution efficiency.

Conclusion:
This analysis reveals key inefficiencies in the IT helpdesk, particularly with system and hardware tickets dragging down resolution times and satisfaction. By targeting these areas with specific SLAs & training we can significantly boost performance. 
