# SAS-project
# perform data screening and generate reports for data with problems

#Suppose you are doing an epidemiological observational study to find risk factors for
#heart attack. Data are collected from medical charts and saved as SAS data sets. These
#data usually contain numerous errors, such as typos, missing records, inconsistent
#measurement units, etc. It is important to clean the data prior to doing any analyses. Some
#of these errors, e.g., data entry errors, are correctable after communication with the study
#site or contacts with study subjects. Thus, data screening is an important step in the
#conduct of a study. Problematic data are identified during data screening, and screening
#results are communicated to the study site to have the problems corrected. Data screening
#can be based on common sense and/or criteria specified in the study.

#The table below describes the
#contents of each data set. Please generate screening reports, one for each site. The
#screening reports contain data you would like to verify with the study sites. Use common
#sense when you screen the data. For example, you would like to verify with the site if
#you see a subject from the site is taller than 100 inches. Your report should be easy to
#read for people who do not know SAS, e.g. an RN in doctor’s office. 


##Data Set Content:
##we have six datasets: demog, hw, bp, glucose, lipid, misc

##demog: Demographic data 
 #including:

        * subject: subject ID
        * gender: Gender
            1:F: female
            2:M: male
        * dob: date of birth
        * doe: date of entering into the study
        * site: study site
            1: Arizona
            2: California
            3: New Jersey
            4: New York
            5: Texas
        * smoke: whether the subject smokes
            0: No
            1: Yes
        * drink: whether the subject drinks
            1: Never
            2: less than one drink per week
            3: 1-3 drinks per week
            4: 4-6 drinks per week
            5: one drink or more per day
        * marital: marital status
            1: Single
            2: Married
            3: Divorced
            4: Other
        * education: education received
            1: below high school
            2: high school graduate
            3: college graduate
            4: post-college 
            
##hw: Height and weight data.

#Note that height is measured only once 
#at the beginning of the study.

 #including:

        * subject: subject ID
        * dov: date of visit
        * height: height in inches
        * weight: body weight in pounds
        
##bp: Blood pressure data:
 #including:
 
        * subject: subject ID
        * dov: date of visit
        * sbp: systolic blood pressure
        * dbp: diastolic blood pressure
        
##glucose: Blood glucose data.
 #including:
        * subject: subject ID
        * dov: date of visit
        * glucose: fasting plasma glucose (mg/dL)
##lipid: Lipid data.
 #including:
        * subject: subject ID
        * dov: date of visit
        * tc: total cholesterol
        * tg: triglyceride
        * hdl: high density cholesterol
        * ldl: low density cholesterol

        
##misc: Other clinical data.       
        
        * subject: subject ID
        * dov: date of visit
        * pregnancy: whether the subject is pregnant
            0: No
            1: Yes
            9: N/A
        * exercise: does the subject exercise routinely in the past 3
        * months?
            0: No
            1: Yes
        * chd: any heart attack in the past 5 years?
            0: No
            1: Yes 
