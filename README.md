# transfers_vs_trophies
An Analysis of the transfer spending of EPL teams and comparison to trophies won


Data Sources
24/25 Epl Transfers - https://www.transfermarkt.com/premier-league/einnahmenausgaben/wettbewerb/GB1

24/25 Epl league table - https://www.transfermarkt.com/premierleague/tabelle/wettbewerb/GB1#google_vignette

Importing Data
24/25 Epl Transfers and 24/25 Epl league table data were imported using power query. 

Cleaning
24/25 Epl Transfer data was renamed "transfers", columns were renamed to suit analysis
Renaming - Clubs got their names shortened for better visualization
Data Types - Money columns are converted from text to whole numbers
![image](https://github.com/user-attachments/assets/11cd70d0-de01-41d6-9aba-6025f603d604)

24/25 Epl league table data was renamed "epl_tabl, Clubs were also renamed to match "transfers" table
![image](https://github.com/user-attachments/assets/a92dda9e-616f-45b2-8450-17244c229fef)


Data Preparation
A new column called "Outcome" was created in epl_transfer to display the outcome of the league positions in power query.
![image](https://github.com/user-attachments/assets/bd321aa9-4431-4663-994d-565b1fb4b3ab)

The code is 

= if [Position] = 1 then "Winner"

else if [Position] >= 2 and [Position] <= 5 then "Ucl"

else if [Position] = 6 then "Europa"

else if [Position] = 7 then "Conference"

else if [Position] >= 18 then "Relegated"

else "Others"
![image](https://github.com/user-attachments/assets/494565bb-81b7-401f-aa27-513e7508dc6e)


epl_transfer table was cloned, columns were removed and a new column was created to show the teams that won trophies
![image](https://github.com/user-attachments/assets/21fca646-8dcf-472c-a221-56c096d11ba4)

![image](https://github.com/user-attachments/assets/1901d7cf-a6c2-4593-a2a5-90e7b51d9149)



Modelling
Auto Model made relationships with the position column. It was adjusted to the club column
Auto model 
![image](https://github.com/user-attachments/assets/e3be9f90-e16b-451e-b6d1-7322fc58be14)


Corrected Model 
![image](https://github.com/user-attachments/assets/7bd9e0e8-6460-43bb-b8c2-27682d55c3de)


