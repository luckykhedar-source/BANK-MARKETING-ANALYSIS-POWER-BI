\# DAX Measures



\## Total Clients



```DAX

Total Clients =

COUNTROWS(FactCampaign)



Subscribed Clients =

CALCULATE(

COUNTROWS(FactCampaign),

FactCampaign[y] = "yes"

)



Subscription Rate % =

DIVIDE(

[Subscribed Clients],

[Total Clients],

0

)



Average Balance =

AVERAGE(FactCampaign[balance])



Housing Loan % =

DIVIDE(

CALCULATE(

COUNTROWS(FactCampaign),

FactCampaign[housing] = "yes"

),

[Total Clients],

0

)



Personal Loan % =

DIVIDE(

CALCULATE(

COUNTROWS(FactCampaign),

FactCampaign[loan] = "yes"

),

[Total Clients],

0

)



Average Campaign Contacts =

AVERAGE(FactCampaign[campaign])



Average Contact Duration =

AVERAGE(FactCampaign[duration])





\---

