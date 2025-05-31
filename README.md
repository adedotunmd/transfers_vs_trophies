# Transfers vs Trophies
An Analysis of the transfer spending of EPL teams and comparison to trophies won and league position.

## Tools & Skills
- Microsoft Power BI
- Power Query
- M-Query
- Data Analysis
- Data Visualization
- Football Analytics

## Analysis

### Data Sources
24/25 Epl Transfers - https://www.transfermarkt.com/premier-league/einnahmenausgaben/wettbewerb/GB1

24/25 Epl league table - https://www.transfermarkt.com/premierleague/tabelle/wettbewerb/GB1#google_vignette

### Importing Data
24/25 Epl Transfers and 24/25 Epl league table data were imported using power query. 

### Cleaning
24/25 Epl Transfer data was renamed "transfers", columns were renamed to suit analysis
Renaming - Clubs got their names shortened for better visualization
Data Types - Money columns are converted from text to whole numbers
![image](https://github.com/user-attachments/assets/11cd70d0-de01-41d6-9aba-6025f603d604)

24/25 Epl league table data was renamed "epl_table", Clubs were also renamed to match "transfers" table
![image](https://github.com/user-attachments/assets/a92dda9e-616f-45b2-8450-17244c229fef)


### Data Preparation
A new column called "Outcome" was created in epl_transfer to display the outcome of the league positions in power query.

![image](https://github.com/user-attachments/assets/ac1f4c7c-a302-444a-9241-3e46212842ab)

The output:

![image](https://github.com/user-attachments/assets/494565bb-81b7-401f-aa27-513e7508dc6e)


epl_transfer table was cloned, columns were removed and a new column was created to show the teams that won trophies
![image](https://github.com/user-attachments/assets/e838ddb4-bb2f-4d57-8049-317ac964e9f9)

The output:

![image](https://github.com/user-attachments/assets/1901d7cf-a6c2-4593-a2a5-90e7b51d9149)



### Modelling:
Automatically derived Model made relationships with the position column. It was adjusted to the club column

Auto Model                                  |                      Adjusted Model
:------------------------------------------:|----------------------------------------|
![image](https://github.com/user-attachments/assets/e3be9f90-e16b-451e-b6d1-7322fc58be14)     |       ![image](https://github.com/user-attachments/assets/f4ac2140-e552-4e8b-8c67-86eeb0c69f71)

### Visualisation

The report comprises 3 pages

1. 24/25 EPL Transfer Table (Incomings)
2. Transfers vs League Position
3. Transfers vs Trophies


#### 24/25 EPL Transfer Table (Incomings)
![image](https://github.com/user-attachments/assets/8b03e161-e7a5-4e0f-b46c-7f49342ae0d6)

##### Key Insights:
- Brighton spent the most on transfers this season, followed by Chelsea, Man Utd and Man City.
- Liverpool spent the least on transfers


#### Transfers vs League Position
![image](https://github.com/user-attachments/assets/b20ec74e-134a-46c4-8611-7467b29c8515)

##### Key Insights:
- Liverpool won the league despite spending the least.
- Brighton spent the most and didn't qualify for any European competition.
- Man Utd spent 3rd highest and still had their worst season in over 4 decades.
- The relegated teams were heavy spenders as well.

#### Transfers vs Trophies
![image](https://github.com/user-attachments/assets/decce0c1-a803-49fb-9e0a-6fa131a9fe66)
- Chelsea was the only 200m + spender with a trophy this season. The other high spenders were trophyless
- 3 of the bottom 6 spenders added a trophy to their cabinet; Liverpool, Newcastle, Crystal Palace

## Conclusion
The financial gap between the big and small teams is fast closing so the advantage they once had is gone. Money won't be enough to guarantee success. Proper scouting and planning are more important than unlimited spending. FSG proves to have the best model for recruitment and this is evidenced by the EPL title win.



