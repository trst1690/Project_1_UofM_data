# Project_1_UofM_data

GOAL - To see if RountableRx  is serving patients as efficiently as possible.
RoundtableRx would like their patient population analyzed to see if they are positively impacting the lives of the most disadvantaged Minnesotans. RoundtableRx desires to study the utilization of their services in MN.
Discuss RountableRx’s mission.
Explain ADI rankings and connect them to health outcomes.
Examine RoundtableRx patient ADI rankings vs MN population rankings.
Identify where in MN patients are located.
Gain insight into how RoundtableRx can better serve Minnesotans.
QUESTIONS
What are the ADI rankings of RoundtableRx patients?
How do ADI rankings of RoundtableRx patients compare to those of the general population of MN? 
Where in the state is RoundtableRx most successful in helping the most vulnerable patients? 
What opportunities are there to improve the care that RoundtableRx offers?
What is the average ADI state rank per county? 
How many patients does Roundtable Rx have in each county?


METHOD
Step 1. Use RoundtableRx data to find the ADI ranks of patients. The Area Deprivation Index (ADI) is a tool used to classify neighborhood socioeconomic status at the local or state level. Higher ADI ranks reflect a neighborhood's poor socioeconomic standing.
Step 2. Get the MN 2020 prenatal data about quality of care received by the patients.
Step 3. Use Python(pandas) to import and clean the data.
Step 4. Merge the STATE ADIRANK data with the patient ADIRANK data.
Step 5. Find the Longitude and Latitude of the county zipcodes using the Geoapify API.
Step 6. Make barcharts and pie charts to compare the patients ADIRANKS and also to compare the average ADIRANKS of patients with the counties they reside in.
Step 7. Make mapplots to show the location of repositories and density of patients in the MN map.
Step 8. Make scatter plots and regression lines to find the correaltion between the ADIRANKS and the prenatal care.

CONCLUSION
We found that RountableRx is postively serving the disadvantaged community in Minnesota. Most of their patients have high ADTSTATE RANK. The RoundtableRx need mre repositories in northwestern, northeastern and southwestern areas. 

