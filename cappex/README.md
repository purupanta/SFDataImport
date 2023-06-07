# Cappex data mapping and pipeline design

a. Special characters such as :, ', . ?, ... will be removed if exists from each attribute values <br />
b. Attribute values are trimmed <br />
c. bolds are "valuable" and "underlined" are required (or essential)<br />

|  FAId  | File Attributes                         | Data Types            | Default Value | Note |
| ------ | --------------------------------------- | --------------------- | ------------- | ---- |
| 01.    | Inquiry Product                         |                       |               |      |
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
| 18.    | <b>Major 1</b>                          |                       |               |      |
| 19.    | <b>Major 2</b>                          |                       |               |      |
| 20.    | <b>Major 3</b>                          |                       |               |      |
| 26.    | <b>Transfer Student Current College</b> |                       |               |      |
| 27.    | <b>College GPA</b>                      |                       |               |      |
| 21.    | <b>Foreign Address</b>                  |                       |               |      |
| 22.    | HS Name                                 |                       |               |      |
| 23.    | SAT Composite, Updated                  |                       |               |      |
| 24.    | SAT Composite                           |                       |               |      |
| 25.    | ACT Composite                           |                       |               |      |


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
