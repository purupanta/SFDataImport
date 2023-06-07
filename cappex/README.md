# Cappex data mapping and pipeline design


a. Special characters such as :, ', . ?, ... will be removed if exists from each attribute values <br />
b. Attribute values are trimmed <br />
c. bolds are "valuable" and "underlined" are required (or essential)<br />

|  FAId  | File Attributes                         | Data Types            | Default Value | Note |
| ------ | --------------------------------------- | --------------------- | ------------- | ---- |
| 01.    | <b>Inquiry Product</b>                  |                       |               |      |
| 02.    | <b>First Name</b>                       |                       |               |      |
| 03.    | <b>Last Name*</b>                       |                       |               |      |
| 04.    | <b>Email Address*</b>                   |                       |               |      |
| 05.    | <b>Birth Date</b>                       |                       |               |      |
| 06.    | <b>Gender</b>                           |                       |               |      |
| 07.    | <b>Address1</b>                         |                       |               |      |
| 08.    | <b>Address2</b>                         |                       |               |      |
| 09.    | <b>City</b>                             |                       |               |      |
| 10.    | <b>State</b>                            |                       |               |      |
| 11.    | <b>Zip Code</b>                         |                       |               |      |
| 12.    | <b>Country</b>                          |                       |               |      |
| 13.    | <b>Primary Phone</b>                    |                       |               |      |
| 14.    | <b>Ethnicity - Fixed List</b>           |                       |               |      |
| 15.    | <b>Expected HS Graduation Date</b>      |                       |               |      |
| 16.    | <b>HS GPA</b>                           |                       |               |      |
| 17.    | <b>CEEB Code</b>                        |                       |               |      |
| 18.    | <b>Transfer Student Current College</b> |                       |               |      |
| 19.    | <b>College GPA</b>                      |                       |               |      |
| 20.    | <b>Foreign Address</b>                  |                       |               |      |
| 21.    | <b>Major 1</b>                          |                       |               |      |
| 22.    | <b>Major 2</b>                          |                       |               |      |
| 23.    | Major 3                                 |                       |               |      |
| 24.    | HS Name                                 |                       |               |      |
| 25.    | SAT Composite, Updated                  |                       |               |      |
| 26.    | SAT Composite                           |                       |               |      |
| 27.    | ACT Composite                           |                       |               |      |


FAId	File Attributes	Data Types (MaxSize)	Possible Values	Default Value	Note
1	Inquiry Product	string(50)	"""Cappex"" 
""Greenlight""
""Cappex Greenlight""
""Cappex Transfer"""	"Cappex"	
2	First Name	string(100)			
3	Last Name	string(100)			Last Name and Email Address are required fields
4	Email Address	string(100)			Last Name and Email Address are required fields
5	Birth Date	Date		null	
6	Gender	Char	"M", "F", null	null	
7	Address1	string(255)		null	
8	Address2	string(255)		null	
9	Foreign Address	string(255)		null	
10	City	string(50)		null	
11	State	string(50)		null	
12	Zip Code	string(20)		null	
13	Country	string(50)		null	
14	Primary Phone	string(20)		null	
15	Ethnicity - Fixed List	string(100)		null	
16	Expected HS Graduation Date	Date		null	
17	HS GPA	string(6)		null	
22	CEEB Code	string(10)		null	
26	Transfer Student Current College	string(255)		null	
27	College GPA	string(6)		null	
23	Major 1	string(255)		null	
24	Major 2	string(255)		null	
25	Major 3	string(255)		null	
18	SAT Composite, Updated	string(6)		null	
19	SAT Composite	string(6)		null	
20	ACT Composite	string(6)		null	
21	HS Name	string(255)		null	
![image](https://github.com/purupanta/SFDataImport/assets/56935340/ff89a94a-caa4-42e7-a0c1-e82dbd309b1b)



<!--
<table> 
  <tr><th><b><u>Test Head</u></b></th></tr> 
  <tr><td>Test Data</td></tr> 
</table>
In same order as original file:
===============================
Inquiry Product
First Name
Last Name
Email Address
Birth Date
Gender
Address1
Address2
Foreign Address
City
State
Zip Code
Country
Primary Phone
Ethnicity - Fixed List
Expected HS Graduation Date
HS GPA
SAT Composite, Updated
SAT Composite
ACT Composite
HS Name
CEEB Code
Major 1
Major 2
Major 3
Transfer Student Current College
College GPA
-->
