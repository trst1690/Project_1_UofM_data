# Analyzing Healthcare Services Using Patient ADI Ranks

## BACKGROUND
RoundtableRx runs Minnesota's Medication Repository. Their mission is to offer safe and affordable medication to Minnesotans in need, provide continuity of care, and reduce waste by redistributing unused medications. Currently, RoundtableRx partners with 22 local repository locations across MN to get unused medications into the hands of uninsured and underinsured Minnesota residents. RoundtableRx would like their patient population analyzed to see if they are positively impacting the lives of the most disadvantaged Minnesotans. 

The metric used to determine RoundtableRx's impact is ADI state rankings of their patient population. The Area Deprivation Index (ADI) is a tool used to classify neighborhood socioeconomic status at the local or state level. Factors that affect ADI ranks include standards of living, access to high-quality education, and adequate housing. Higher ADI ranks reflect a neighborhood's poor socioeconomic standing. ADI ranks can be used to assess health disparities, improve health outcomes, and provide more informed services to vulnerable neighborhoods. High ranks have been linked to diabetes and cardiovascular disease, increased utilization of health services, and earlier death. State ADI rankings are represented as a decile, ranging from 1 to 10.

Therefore, RoundtableRx's goal is to serve patients that have high state ADI rankings (5 or above). Being able to show success with this metric would be very powerful in applying for funding through grants and government assistance.

In addition to analyzing the RoundtableRx patient population, ADI rankings were further investigated to see if they can predict the quality of prenatal care received by Minnesotans.

## GOAL 
* Discuss RountableRx’s mission.
* Explain ADI rankings and connect them to health outcomes.
* To see if RountableRx is serving the most socioeconomically disadvantaged Minnesotans (high ADI ranks).
* Examine RoundtableRx patient ADI rankings vs MN population ADI rankings.
* Identify where in MN patients are located.
* Gain insight into how RoundtableRx can better serve Minnesotans.
## QUESTIONS
* What are the ADI rankings of RoundtableRx patients?
* What opportunities are there to improve the care that RoundtableRx offers?
* How many patients does Roundtable Rx have in each county?
* What regions of MN does RoundtableRX not serve and how does it impact access to services?
* Where in the state is RoundtableRx most successful in helping the most vulnerable patients? 
* What is the average ADI state rank per county? 
* How do ADI rankings of RoundtableRx patients compare to those of the general population of MN? 
* Is there a correlation between low ADI state rank and quality of prenatal care? 
## METHOD
* Step 1. Import RoundtableRx patient data, RoundtableRx local repository data, MN ADI rankings data, and MN 2020 prenatal data about quality of care received by the patients.
* Step 2. Use jupyter notebook/python/pandas to import and clean the data.
* Step 3. Merge RoundtableRx patient data and MN ADI rankings data to find the ADI ranks of patients.
* Step 4. Find the longitude, latitude, and county for all ZIP codes in the datasets using the Geoapify API.
* Step 5. Use matplotlib to create barcharts and pie charts to visualize the patient's ADI ranks and also to compare the average ADI ranks of patients with the average ADI ranks of the general population of the counties they reside in.
* Step 6. Use hvplot to create maps to show the location of repositories and patients.
* Step 7. Use matplotlib and scipy.stats (linregress) to create scatter plots and regression lines to find the correaltion between patient ADI rank and the quality of their prenatal care.

## ANALYSIS & CONCLUSION
Overall, RoundtableRx can be confident that they are helping the most disadvantaged Minnesotans. 70% of RoundtableRx's patients have an ADI rank of 5 or above and 45% have an ADI rank of 8 or above. The most common patient ADI state ranking is 10. These are all strong statements to make in support of gaining more funding through grants or government asssitance.

Patients are congregated around repository locations. One is exception is International Falls. This shows that, in general, patients only get the services of RoundtableRx if there is a local repository nearby. Local repositories nearby the Twin Cities seem to capture patients with lower ADI ranks, so expanding into greater Minnesota would increase the average ADI ranking of patients, improving this metric of success, and supporting requests for funding. RoundtableRx does not have any locations in NW and SW Minnesota and should focus on expanding into those territories, especially since they have high ADI ranks.

Comparing locations of patients and locations of local repositories, it’s interesting that Hennepin County has the most repositories but not the most patients. There is an opportunity for local repositories in Hennepin County to increase the amount of patients they serve. RoundtableRx could reach out to Hennepin County locations and see if they need more staff training or more resources to implement our services. Saint Louis County has the most patients, so RoundtableRx could look into what makes them so successful at identifying and serving patients that cannot afford their medications.

As RoundtableRx's patient poplation grows, the strength of the findings will also improve and we'd recommend that they rerun this analysis for updated results periodically to see if business decisions have resulted in improved patient ADI metrics. 

Since ADI rankings have been connected with poor health outcomes such as diabetes and cardiovascular disease, our group was interested to see if they correlate to quality of prenatal care. If they did, we'd expect the rates of inadequate prenatal care to increase with ADI rank and rates of intensive prenatal care to decrease with ADI rank. The corrolation value is very low in both regressions, therefore we can conclude that there is not a relationship between ADI rank and quality of prenatal care.

Sources:
* https://www.neighborhoodatlas.medicine.wisc.edu/
* https://www.health.state.mn.us/data/mchs/genstats/countytables/MNCountyHealthTables2020.pdf 
* https://www.roundtablerx.org/

