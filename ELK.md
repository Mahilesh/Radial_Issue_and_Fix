### Problem 1:- Data not invisble in kibana dashboard from 12 AM UTC noon. 
App name:- heydude-connector 
Deployed through gitlab CI/CD in the host - lvsuatdockapp01 and 02 (both are on-premises servers)

> Fix:- Restarted td-agent.service
>
> systemctl restart td-agent.service

#### RCA :- Not found
