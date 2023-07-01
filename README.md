# KPOP_Girl_Group
I looked into the popularity of Kpop Girl Groups. I used data sets from Kaggle and some I found online in general.

To practice SQL and PowerBI, I chose to analyze Kpop Girl Groups because their music is popular worldwide.

I ran sql queries to ask the following questions.

What year did each girl group debut?
How many groups are there per studio?
How many groups are still active?
Results

In researching and analyzing the data i found more girl groups were popular after 2010.
There were more studios that I expected with the top studios having a maximum of 6.
I was surprised how many groups are no longer active.
The sql queries are below.

--This query displays each company group status organized by status without duplicates.

Select
distinct company,
active

from kpop_girl_group
order by active

--This query displays each girl group by debut year with their studio name labeled.
select
company,
name,
debut
from kpop_girl_group
order by debut
