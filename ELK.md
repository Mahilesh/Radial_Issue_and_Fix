### Problem 1:- Data not invisble in kibana dashboard from 12 AM UTC noon. (On-premises + AWS)
App name:- heydude-connector 
Deployed through gitlab CI/CD in the host - lvsuatdockapp01 and 02 (both are on-premises servers)

> Fix:- Restarted td-agent.service
>
> systemctl restart td-agent.service

#### RCA :- Not found

### Problem 2:- Data is not flowing for all indexes named lvs-logstash-* (P2) (On-premises)
•	Problem: Graphite server (metrics.gspt.net) was down.

> Fix:-
> 1.	Restored the server lvsprdgptdb02.gspt.net (decommissioned 2 days prior). - SCTASK0477376
> 2.	ENABLED THE VIP that was disabled 1 day prior. - CTASK0052306

#### RCA :- Logstash processes configuration files in lexicographical order. Sequence matters.
