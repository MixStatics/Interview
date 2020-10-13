# Interview





SELECT	PatientTable.Fname. 
	PatientTable.Lname, 
	PatientTable.Age, 
	PatientTable.COF1,	PatientTable.DC1,	PatientTable.DDesc1, 
	PatientTable.COF2,	PatientTable.DC2,	PatientTable.DDesc2, 
	PatientTable.COF3,	PatientTable.DC3,	PatientTable.DDesc3, 
	PatientTable.COF4,	PatientTable.DC4,	PatientTable.DDesc4,
	PatientTable.COF5,	PatientTable.DC5,	PatientTable.DDesc5, ....... (for the number of diagnosis) ,
				PatientTable.P1,	PatientTable.PDesc1,
				PatientTable.P2,	PatientTable.PDesc2,
				PatientTable.P3,	PatientTable.PDesc3,
				PatientTable.P4,	PatientTable.PDesc4,
				PatientTable.P5,	PatientTable.PDesc5, ....... (for the number of procedures) ,
	ResultTable.Path1,	ResultTable.PathResult1,
	ResultTable.Path2,	ResultTable.PathResult2,
	ResultTable.Path3,	ResultTable.PathResult3,
	ResultTable.Path4,	ResultTable.PathResult4,
	ResultTable.MRI_Image,	ResultTable.MRI_ResultText.
	ResultTable.CT_Image,	ResultTable.CT_ResultText

FROM PatientTable LEFT JOIN TestResults 
   ON CONCAT(PatientTable.Fname, ' ' , PatientTable.Lname, ' ' , PatientTable.BDate) 
	= CONCAT(ResultTable.Fname, ' ' , ResultTable.Lname, ' ' , ResultTable.BDate)




USER STORY  Questions:  

1. If you had more time, what would you change or focus more time on?

If I had more time and also access to the appropriate systems I would have completely finished the application to demonstrate rather than only joining the data sources.  Furthermore, as my application details, I am more of data manager and research analyst than programmer, and in particular I am very aware of the clinical issues from my biomedical science background. Furthermore my answers to the application questionnaires indicate that I have not used particular software developmental methods since starting my recent Doctoral thesis work in 2015. So while I am able to manage and understand the medical information projects I would need more time for developing applications with particular programming languages that I have not used.

2. Which part of the solution consumed the most amount of time?

The parts of the solution that consumed a lot of time included understanding the details of what was required. When reading the advertisement I understood that the position was for the lead developer for both data research and operational data. So rather than an IT person I had expected the role to focus on the medical and analytical issues (including research analysis) and so a biomedical science and hospital performance knowledge would be relevant. The lead person could then discuss with the IT staff the appropriate systems, which I am very adaptable to as my work history demonstrates.  On the other hand this exam / test appears to be more about programming rather than examining the clinical issues etc.

3. What would you suggest to the customer that they may not have thought of in regards to their request?

There are a few things in the design of this project that may have some issues. One is the readmissions. So as an example if we just rely on name and birth date to ID the episode on patient episode may be connected with others with regards tot he ICD coding or pathology testing. Even the imaging may be outdated and need redoing, for example. So the linking should include the dates of the activities or the admission number to link the patient information and the DRG / ICD codes for example.  Other things of interest could include admission type (emergency etc) and discharge type (if the patient has been discharged) as well as readmissions (particularly emergency readmission within a set time period for the same diagnosis). As well the outpatient data, including allied health follow up, would be significant in some cases, such as diabetes etc.
