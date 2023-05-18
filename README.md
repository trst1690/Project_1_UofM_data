# Analyzing Healthcare Services Using Patient ADI Ranks

## BACKGROUND
RoundtableRx is a non-profit organization that runs Minnesota's Medication Repository. Their mission is to offer safe and affordable medication to Minnesotans in need, provide continuity of care, and reduce waste by redistributing unused medications. Currently, RoundtableRx partners with 22 local repository locations across MN to allocate unused medications to uninsured and underinsured Minnesota residents. RoundtableRx would like their patient population analyzed to see if they are improving the lives of the most disadvantaged Minnesotans. 

The metric used to determine RoundtableRx's impact is ADI state rankings of their patient population. The Area Deprivation Index (ADI) is a tool used to classify neighborhood socioeconomic status at the local or state level. Factors that affect ADI ranks, include standards of living, access to high-quality education, and adequate housing. Higher ADI ranks reflect a neighborhood's poor socioeconomic standing. Organizations can utilize ADI ranks to assess health disparities, improve health outcomes, and provide more informed services to vulnerable groups. High ADI ranks are linked to diabetes and cardiovascular disease, increased utilization of health services, and earlier death. State ADI rankings are denoted as a decile, ranging from 1 to 10.

RoundtableRx's goal is to serve patients that have high state ADI rankings of 5 or above. Being able to show success with this metric would be very powerful in applying for funding via grants and government aid and improve service delivery.

In addition to analyzing the RoundtableRx patient population, ADI rankings were further investigated to determine whether ADI rank impacts the quality of prenatal care received by Minnesotans.

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
Overall, RoundtableRx can be confident they are helping the most disadvantaged Minnesotans. 70% of RoundtableRx's patients have an ADI rank of 5 or above, and 45% have an ADI rank of 8 or above. The most common patient ADI state ranking is 10. These are all strong statements to make in support of gaining more funding through grants or government assistance.

Most patients are clustered around the repository locations. One exception is International Falls. Patients from International Falls may commute long distances to receive medication, revealing that proximity of repositories impact patient access to RoundtableRx services. Local repositories near the Twin Cities seem to capture patients with lower ADI ranks, so expanding into greater Minnesota would increase the average ADI ranking of patients, improving this metric of success and supporting requests for funding. RoundtableRx does not have locations in NorthWestern and SouthWestern Minnesota and should focus on expanding into those territories, especially since they have a high ADI rank. RoundtableRx should consider transportation and medication delivery services to benefit new patients that live in remote communities. 

When comparing the locations of patients and local repositories, we discovered that Hennepin County had the most repositories but the fewest patients. This is an opportunity for the local repositories in Hennepin County to increase the number of patients they serve. RoundtableRx can connect with Hennepin County repository locations to see if they need more staff training or resources to implement health services. Saint Louis County has the most patients, so RoundtableRx could look into what makes them successful at identifying and serving patients that cannot afford their medications.

As RoundtableRx's patient population grows, the strength of the findings will also improve. We recommend that they periodically rerun this analysis for updated results to see if organization decisions have resulted in improved patient ADI metrics. We recommend that RoundtableRx  conduct qualitative research, such as surveys and interviews, to identify the health needs of Minnesotans in NorthWestern and SouthWestern regions. 

Since Studies support that ADI rankings are associated with poor health outcomes such as diabetes and cardiovascular disease, we investigated ADI rankings and the quality of prenatal care to uncover any correlation. If there was a correlation, we expected the rates of inadequate prenatal care to increase with ADI rank and rates of intensive prenatal care to decrease with ADI rank. The correlation value of ADI and prenatal care was less than 0.2 in both regressions. Therefore, we conclude that there is no relationship between ADI rank and the quality of prenatal care. 


Sources:
* https://www.neighborhoodatlas.medicine.wisc.edu/
* https://www.health.state.mn.us/data/mchs/genstats/countytables/MNCountyHealthTables2020.pdf 
* https://www.roundtablerx.org/

