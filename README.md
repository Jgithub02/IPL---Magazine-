# IPL-Magazine

# Problem Statement 
"Sports Basics" is a sports blog company that entered space recently. They wanted to get more traffic to their website by releasing a special edition magazine on IPL 2024. This magazine aims to provide interesting insights and facts for fans, analysts and teams based on the last 3 years' data. The chief editor Tony Sharma oversees this publication, and he believes in data analytics. He reached out to Peter Pandey, a journalist in his team who is a data-savvy cricket enthusiast.

# Steps Followed 
# 1. Data Loading into SQL 
Created a database called "ipl" using the following command

```
CREATE DATABASE IF NOT EXISTS "ipl";
```


# Data Exploration :
```
SELECT * FROM ipl.dim_players_summary;

select count(distinct(match_id)) from ipl.fact_bating_summary ; -- total match played in 3 years according fact_bating_summary table = 206


SELECT * FROM ipl.fact_bowling_summary;


select count(distinct(match_id)) from ipl.fact_bowling_summary ; -- total match played according fact_bowling_summary table = 206


SELECT * FROM ipl.fact_bowling_summary;


select count(distinct(match_id)) from ipl.fact_bowling_summary ; -- total match played according dim_match table = 206 
-- According to the fact_bating_summary table, fact_bolwling_summary table and dim_match table the match played in 3 years are same (206)


select  count(distinct(name)) from ipl.dim_players_summary; -- total palyers who played for 3 years = 292
```
