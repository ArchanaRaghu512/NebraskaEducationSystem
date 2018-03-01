Data Cleaning Documentation

## Data description 

> This Data set contains a multitude of information. There are 10 files in total, I am not sure if all of them are needed for analysis, but it depends on what questions someone would ask. Contained inside is information regarding Nebraska schools from the 2015-2016 year. There is information regarding Attendance Rate, Dropout Rates, Teacher information (general info, not specific personal info), and test scores around Math, Reading, Science, Writing. This information could be used to evaluate the success of Nebraska Schools, and determine which schools are more successful than others.

## Dataset Licensing Information

The Terms and Conditions page seems to be inactive on the main page, so no specific information regarding data usage could be found. I also checked the Privacy policy at "http://nep.education.ne.gov/privacy-policy/" and it gives a 404 error. There was nothing else I could find that would give me specific information in this general area. However, The Nebraska Department of Education is responsible for this data, which is a branch of the Nebraska Government, so I decided to go to the Nebraska.gov/policies page and found the following.

"Use of Site Information

Nebraska.gov (“Company”) is not responsible if information made available on this site is not accurate, complete or current. The material on this Site is provided for general information only and should not be relied upon or used as the sole basis for making decisions without consulting primary, more accurate, more complete or timely sources of information. Any reliance on the material on this Site is at your own risk. This Site may contain certain historical information. Historical information necessarily is not current and is provided for your reference only. We reserve the right to modify the contents of this Site at any time, but we have no obligation to update any information on the Site. You agree that it is your responsibility to monitor changes to the Site.

You may access, copy, download, and print the material contained on the Site for your personal and non-commercial use, provided you do not modify or delete any copyright, trademark or other proprietary notice that appears on the material you access, copy, download or print. Any other use of content on the Site, including but not limited to the modification, distribution, transmission, performance, broadcast, publication, uploading, licensing, reverse engineering, transfer or sale of, or the creation of derivative works from, any material, information, software, products, or services obtained from the Site, or use of the Site for purposes competitive to the Company, is expressly prohibited. You agree to abide by all additional restrictions displayed on the Site as they may be updated from time to time. The Company neither warrants nor represents that your use of materials on this Site will not infringe rights of third parties not affiliated with the Company, and your use of such materials is at your own risk.

You may not use contact information provided on the Site for unauthorized purposes, including marketing. You may not use any hardware or software intended to damage or interfere with the proper working of the Site or to surreptitiously intercept any system, data or personal information from the Site. You agree not to interrupt or attempt to interrupt the operation of the Site in any way. The Company reserves the right, in its sole discretion, to limit or terminate your access to or use of the Site at any time without notice. Termination of your access or use will not waive or affect any other right or relief to which the Company may be entitled at law or in equity.""

## Dataset Questions

We first created a list of questions that we could possibly answer with this data set. We then posted those questions to the Class and waited for feedback. Some of the feedback helped us revise some of our questions while others added to the list of questions. We realize that we might not be able to answer all questions with the data, but as we clean up the data we will be able to determine which questions are feasible to answer. The list below contains all the questions we collected. 

•	Does the percentage of teachers with a master’s degree have an impact on standardized test scores?

•	Are students more likely to graduate from Urban or Rural schools?

•	Are students more likely to drop out of school from Urban or Rural schools?

•	Does certain ethnic background have higher or lower standardized test scores compared to all students?

•	Have test scores increased or decreased over the last few years?

•	Which demographics have seen increases or decreases?

•	According to test scores, what school is the top performer? How does that relate to the school’s budget?

•	According to test scores, what school is the least performer? How does that relate to the school’s budget?

•	Which gender has the maximum rate of dropouts?

•	Which race/ethnicity has the maximum dropout rate?

•	Are the math scores reason for dropout’s rate?

•	What is the ratio of male and female students in each school?

•	The rate of teachers with master’s degree increased?

•	Increase or decrease in teacher’s salary considering urban Vs rural schools?

•	Free lunch statistic Additional Data is available
        [Link](https://www.education.ne.gov/dataservices/data-reports/)

•	English Language Learners require smaller classes and more budget, higher educated teachers

•	Age group of dropouts (use grade instead)

•	Categorize data by county (perhaps District location instead)

•	Is the attendance rate directly proportional to the Dropout rate?

•	Is the attendance rate directly proportional to the ELL Percentage?

## System and Hardware Information

The following configurations were done using Microsoft Excel 2013 version (15.0.4963.1000) using a Windows 10 PC with Intel Core i7-4790 CPU @ 3.60 GHz, with 16 GB of RAM and a 64bit Operating System.

## DATA SETS

## SET 1

[Link to Set 1](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Set%201.xlsx)

### Dataset Creation Process

**Step 1)** First Download the Excel files from [Link](https://github.com/ArchanaRaghu512/ISQA8086-Team1/tree/master/Deliverables/DataCleaningDocumentation/Original%20Datasets)

- [Download “Nebraska School Information Part 1.xlsx”](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Original%20Datasets/Nebraska%20School%20Information%20Part%201.xlsx)

- [Download “Nebraska School Information Part 2.xlsx”](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Original%20Datasets/Nebraska%20School%20Information%20Part%202.xlsx)

- Save to Desktop for easy retrieval

**Step 2)** Open the two files you downloaded to your desktop
- “Nebraska School Information Part 1.xlsx” contains the following tabs
- Attendance Rate, Cohort, Dropouts, ELL, NeSA Math
- “Nebraska School Information Part 2.xlsx” contains the following tabs
- NeSA Reading, NeSA Science, NeSA Writing, Teacher

**Step 3)** Before you do anything else on “Nebraska School Information Part 1.xlsx” go to File, then Save As. Name your ne file “Super Nebraska School Information”

**Step 4)** First verified all column headers in excel tab “NeSA Math”, “NeSA Reading”, “NeSA Science”, “NeSA Writing”, contained all the same column headers, in the same order.

1.	Type

2.	DataYears

3.	County

4.	District

5.	School

6.	Agency Name

7.	Subject

8.	Grade_Code

9.	Category

10.	AYP Group

11.	Standard Code

12.	Standard

13.	Standard Correct Percent

14.	Student Count

15.	DataAsOf

**Step 5)** All tabs appear to have the same data, so to make the Data easier to manager will combine the data from “NeSA Math”, “NeSA Reading”, “NeSA Science”, “NeSA Writing” into one.

1) In Excel file “Super Nebraska School Information”, towards the bottom of the file click the “+” to create a new Tab

[Screenshot 1](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/1.png)

2) The new tab should say “Sheet 1”. Double click on “Sheet 1”, rename the tab to “NeSA Data”.

3) Click on tab “NeSA Math” left mouse click on cell A1, then press CTRL+SHIFT+END on the keyboard. This will activate cell A1 to O290497.

4) While the range is still active press CTRL+C on the keyboard to copy the selected contents.

5) Click on tab “NeSA Data”, left mouse click cell A1, press CTRL+V on keyboard to paste the data into the new sheet.

6) Go to “Nebraska School Information Part 2.xlsx”, Click on tab “NeSA Reading” left mouse click on cell A2, then press CTRL+SHIFT+END on the keyboard. This will activate cell A2 to O145217.

7) While the range is still active press CTRL+C on the keyboard to copy the selected contents

8) Go Back to “Super Nebraska School Information”, and on tab NeSA Data left mouse click in column A of the next blank row (should be cell A290498) and press CTRL+V to paste the data.

9) Repeat process f-h for “NeSA Science” and “NeSA Writing” making sure to always paste the data into new rows and not to overwrite current rows. 

**Step 6)** While both files (“Super Nebraska School Information” and “Nebraska School Information Part 2.xlsx”) are open go to “Nebraska School Information Part 2.xlsx” and right mouse click on tab “Teachers” you will see the following menu

[Screenshot 2](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/1.1.png)
 
Left mouse click on “Move or Copy…”

[Screenshot 3](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/1.2.png)

Change the To Book: section to “Super Nebraska School Information”, highlight “move to end” and click the check box for “Create a copy” (should look like the image above). This will move a copy of the Teacher data so that you have all Data in 1 File. 

**Step 7)** Close “Nebraska School Information Part 2.xlsx”, do not save any changes in case something gets screwed up and we have to start over. From here on we are going to try and work with “Super Nebraska School Information”

**Step 8)** While on “Super Nebraska School Information” right click on the tab name “NeSA Math” and select the option to delete, then you will confirm that you want to delete. 

**Step 9)** enough changes have happened take a moment to save your document. 

**Step 10)** since a majority of question have to do with trends let’s look at how many years of test scores we have. 

1) Click on the “NeSA Data” tab to activate that worksheet. 

2) Make sure you can see cell A1. Left mouse click row 1 (click the #1 on screen) to highlight the first row. 

3) Then we will want to add filters so we can quickly view our data. On the “HOME” menu tab there is a button that looks like the image below. Click on it, and select “Filter” to add filters on your Column Headers.
 
[Screenshot 4](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/1.3.png)

4) If done correctly your column headers will have a small box with a downward arrow. See image below to confirm. 
 
[Screenshot 5](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/1.4.png)

5) Do this same process for all other Tabs of data (Attendance Rate, Cohort, Dropouts, ELL, Teachers) A few tabs might already have filters applied, so skip the tabs that do. 

**Step 11)** Save your work.

**Step 12)** Filter Subject column to "Writing", calculate the maximum value (7.44)

**Step 13)** In column P enter a formula that takes the Standard Correct Percentage and divide that by 7.44. This will take the values and make a percentage value score that will match the other Subjec score values.

**Step 14)** Copy column P and paste the values into the Standard Correct Percent column.

**Step 15)** Once again save your work.

### Meta Data

This dataset has 15 columns with 120,350 records. The following is a list of attribute definitions.

• Type: Values are “DI”, “SC”, and “ST”. This identifies if the row belongs to District, School, or State.

• DataYears: This is the school year the exam was taken.

• County: This is the county code the school is located. 0 is assigned to Districts and State records.

• District: Is the number assigned to the different school districts throughout Nebraska. 0 is assigned to State records. 

• School: is the numeric code that is assigned to different Schools in Nebraska.

• Agency Name: this is the name of the institution at the different levels State, District, School.

• Subject: This is the subject that students were given an exam. Values are “Mathematics”, “Science”, “Reading”, and “Writing”

• Grade_Code: This represents the student’s current year in school. Values are 3, 4, 5, 6, 7, 8, and 11.

• Category: This represents a collection of the type of AYP Group. For example Gender is a category representing the AYP Groups of Male and Female. Values are “All Students”, “Gender”, “Misc/Other” , ”Mobile”, “Race/Ethnicity”.

• AYP Group: This is the subclass to Category to further classify students in a particular Category. 

• Standard Code: This is the numeric code that represents Standard. Values are 1, 2, 3, 4.

• Standard: This represents a subsection of the Subject that is being tested. For example Math has four standards associated with it, they are “Number Sense”, “Geometric”, “Algebraic”, and “Data Analysis”. Each Subject has different Standard.

• Standard Correct Percent: This value represents the percent of questions that were correctly answered.

• Student Count: This is the count of the number of students that were given the exam.

• DataAsOf: This is the date the values were recorded by Nebraska Department of Education. 

#### Identified Data Issues and Resolution

Since the filters have been applied to all the column headers if you click on the dropdown arrow you can view a list of all the values in that column. Items that should be given attention are the following:

• Blank: this means that a cell is empty and is missing data

• 0: zero could mean that data might have not been recorded, but need to check other variables to see if the value is legit.

• -1: In database management this usually represents that data was not recorded. A -1 could be a correct value, if it is in context, however out of context probably means nothing was recorded. 

#### Accounting for the items listed above the following items were identified. 

**Issue:** DataYears only contains values for the school year 2015-2016. 

**Resolution:** This means that any questions regarding exams in a time series will not be feasible.

**Issue:** County contains 0, but that is because those records are associated with District or State results. 

**Resolution:** Decided to leave these values as is because removing the record removes State or District results that could be used for analysis.

**Issue:** District contains 0, but that is associated with State records.

**Resolution:** Decided to leave these values as is because removing the record removes State results that could be used for analysis.

**Issue:** School: contains 0, but those records are associated with State and District records.

**Resolution:** Decided to leave these values as is because removing the record removes State or District results that could be used for analysis.

**Issue:** Standard Correct Percent: Contains -1, 0, and blank values. 

**Resolution:** Looking at the -1 values, the Student Count also contained -1 values so that confirms that no data was collected for those records. These rows can be removed from the data set, since they are meaningless. Unfortunately this removes 480,562 records of the 669312 total records. 

**Resolution:** Looking at the blank records there are student counts, however since percent correct is the Y value needed for analysis these records do us no good and can also be removed. These records account for 68,400 of the entire sample.

**Resolution:** Looking at the 0 values there appears to be Student Count, this would suggest exams were give, but no questions were answered correctly. Decided to leave these values because we cannot prove they are not correct. 

### Questions we can answer with Data

• Does certain ethnic background have higher or lower standardized test scores compared to all students?

• According to test scores, what school is the top performer?

• According to test scores, what school is the least performer? 


## SET 2

[Link to Set 2](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Set%202.xlsx)

### Dataset Creation Process

> To form this dataset, we have taken common rows and fields (Type, School year, County, District, Agency name) and two unique fields i.e. attendance rate and Dropout rate from two excel sheets (“Attendance rate” and “Dropout rate”). 
We figured that the Dropout Rate sheet had information for the state and district type and for the year 2010 – 2016. Whereas the attendance rate had details for state, district, Learning community and Northern Tier between the year 2001 – 2016.
So, we had to filter the details on common rows and fields.

### Dataset Name: Attendance Rate Sheet & Dropout Rate

**Step 1:** Select the Type ST using the data filter option available in excel as mentioned earlier. 

[Screenshot 1](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/2.png)

**Step 2:** The next criteria is the year. We selected the year that is common in both the sheet i.e.from 2010 -2016.  

[Screenshot 2](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/2.1.png)

**Step 3:** The similar way we had filtered the type “DI” which is district, the year and had copied the filtered data to the new spreadsheet.   

**Step 4:** Merge the fields filtered from both the sheets into the new sheet.  

**Step 5:** And then added the unique columns attendance rate and dropout rate into it.   

### Meta Data

This dataset has 7 columns with 1,245 records. The following is a list of attribute definitions.  

• Type: Values are “DI”, “SC”, and “ST”. This identifies if the row belongs to District, School, or State. 

• School Year: This is the school year the data was collected. 

• County: This is the county code the school is located. 0 is assigned to Districts and State records. 

• District: Is the number assigned to the different school districts throughout Nebraska. 0 is assigned to State records.  

• Agency Name: This is the name of the institution at the different levels State, District, School. 

• Dropout Rate: This is the percentage of students that drop out of school. 

• Attendance Rate: This is the percentage of students who are attending school. 

### Identified Data Issues and Resolution 
**Issue:** The column “School” contained values “0”. 

**Resolution:** It had no impact so we removed the column from the dataset. 

**Issue:** The “Year” Column had values like 20102011. 

**Resolution:** We reformatted it to the following format “2010 – 2011”. 
	
### Questions we can answer with Data

> We can we can interpret how the Attendance rates affect the dropout rates

## SET 3

[Link to Set 3](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Set%203.xlsx)
	
### Dataset Creation Process

> To form this dataset, we have taken common rows and fields from two excel sheets (“Teachers” and “Dropout rate”) and two unique fields i.e. Percentage of Teachers with Master’s Degrees and Dropout rate.
We figured that the Dropout Rate sheet had information for the state and district type and for the year 2010 – 2016. Whereas the “Teachers” sheet contains details for state, district and school between the year 2011 – 2016.
So, we had to filter the details on common rows and fields.

### Dataset Name: Teacher & Dropout Rate sheet.

**Step 1:** Select the Type ST using the data filter option available in excel as mentioned earlier.

[Screenshot 1](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/3.png) 

**Step 2:** The next criteria is the year. We selected the year that is common in both the sheet i.e. from 2011 -2016.

[Screenshot 2](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/3.1.png)

**Step 3:** Repeat the same process on “Dropout rate” sheet 

**Step 4:** After filtering the type and year, copy the filtered value into a sheet. Omit the unrelated columns.

**Step 5:** Add the Dropout rate from “Dropouts” Sheet and “Percentage of teachers with Master’s Degree” from teacher’s sheet to the new sheet.
	
### Meta Data

This dataset has 7 columns with 993 records. The following is a list of attribute definitions. 

• Type: Values are “DI”, “SC”, and “ST”. This identifies if the row belongs to District, School, or State. 

• School Year: This is the school year the data was collected. 

• County: This is the county code the school is located. 0 is assigned to Districts and State records. 

• District: Is the number assigned to the different school districts throughout Nebraska. 0 is assigned to State records.  

• Agency Name: This is the name of the institution at the different levels State, District, School. 

• Percentage of Teachers with Master’s Degrees: This is the percent of teachers who have received a Master’s Degree.  

• Dropout Rate: This is the percentage of students that drop out of school. 

### Identified Data Issues and Resolution 

**Issue:** The column “School” contained values “0”.

**Resolution:** It had no impact so we removed the column from the dataset.

**Issue:** The “Year” Column had values like 20102011.

**Resolution:** We reformatted it to the following format “2010 – 2011”.	

### Questions we can answer with Data

> We can interpret whether the Percentage of teachers with Master’s degree at each school have an impact on the dropout rates

## SET 4

[Link to Set 4](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Set%204.xlsx)

### Dataset Creation Process

To form this dataset, we have taken the excel sheet “Cohort” and kept all the fields. The dataset is clean and filtering wasn’t required.
	
### Meta Data

This dataset has 11 columns with 113,790 records. The following is a list of attribute definitions. 

• Type: Values are “DI”, “SC”, and “ST”. This identifies if the row belongs to District, School, or State. 

• School Year: This is the school year the data was collected. 

• County: This is the county code the school is located. 0 is assigned to Districts and State records. 

• District: Is the number assigned to the different school districts throughout Nebraska. 0 is assigned to State records.  

• School: is the numeric code that is assigned to different Schools in Nebraska. 

• Agency Name: This is the name of the institution at the different levels State, District, School. 

• Graduation Cohort: This represents a year of graduation. 

• Cohort year: This is a numeric code that is associated with Graduation Cohort. 

• Description: This is a student demographic (i.e. Male, Female, Ethnicity) 

• Graduation Count: This is the total count of students graduating 

• Graduation Percentage: This is the percentage of students that are graduating. 

### Identified Data Issues and Resolution 

**Issue:** The “Year” Column had values like 20102011.

**Resolution:** We reformatted it to the following format “2010 – 2011”. 

**Issue:** The column “Graduation Pct” wasn’t clear.

**Resolution:** Renamed it to “Graduation Percentage” for better understanding.**

**Issue:** There are certain values “-1” contained in “Graduation count” and “Graduation Percentage”.
	
### Questions we can answer with Data

> We can interpret which group or category of students have the highest or lowest Graduation count

## SET 5

[Link to Set 5](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Set%205.xlsx)

### Dataset Creation Process

> To form this dataset, we have taken the excel sheet “ELL” and “Dropouts”. WE have kept all the common fields and two unique fields “ELL” and “Dropout Rate”.
We figured that the Dropout Rate sheet had information for the state and district type and for the year 2010 – 2016. Whereas the “ELL” had details for state, district and school between the year 2011 – 2016.
So, we had to filter the details on common rows and fields.

### Dataset Name: ELL & Dropout Rate sheet.

**Step 1:** Select the Type ST using the data filter option available in excel as mentioned earlier.

[Screenshot 1](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/5.png)

**Step 2:** The next criteria is the year. We selected the year that is common in both the sheet i.e. from 2011 -2016.

[Screenshot 2](https://github.com/ArchanaRaghu512/ISQA8086-Team1/blob/master/Deliverables/DataCleaningDocumentation/Screenshots/5.1.png)

**Step 3:** Repeat the same process on “Dropout rate” sheet.

**Step 4:** After filtering the type and year, copy the filtered value into a sheet. Omit the unrelated columns.

**Step 5:** Add the Dropout rate from “Dropouts” Sheet and “ ELL Percentage” from ELL sheet to the new sheet 

### Meta Data

This dataset has 7 columns with 993 records. The following is a list of attribute definitions. 

• Type: Values are “DI”, “SC”, and “ST”. This identifies if the row belongs to District, School, or State. 

• School Year: This is the school year the data was collected. 

• County: This is the county code the school is located. 0 is assigned to Districts and State records. 

• District: Is the number assigned to the different school districts throughout Nebraska. 0 is assigned to State records.  

• Agency Name: This is the name of the institution at the different levels State, District, School. 

• ELL Percentage: This is the percent of students that are English Language Learners. 

• Dropout Rate: This is the percentage of students that drop out of school. 

### Identified Data Issues and Resolution 

**Issue:** The column “School” contained values “0”.

**Resolution:** It had no impact so we removed the column from the dataset.

**Issue:** The “Year” Column had values like 20102011.

**Resolution:** We reformatted it to the following format “2010 – 2011”.

### Questions we can answer with Data

> We try to interpret whether the percentage of ELL in a school affect the dropout rate or not.


