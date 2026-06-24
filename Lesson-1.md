# Introduction to DBMS and SQL

## DBMS -> Relations DBMS -> Keys -> SQL

### DBMS -> Database Management System

##### _Structured Data:_
Tabular Data
You can find a particular data from a id  at a particular address, 
everything in order Ascending/Descending or any order
              
| Header 1 | Header 2 | Header 3 |
| --- | --- | --- |
| Row 1, Col 1 | Row 1, Col 2 | Row 1, Col 3 |
| Row 2, Col 1 | Row 2, Col 2 | Row 2, Col 3 |

##### _Unstructured Data:_
Image, Video
 no particular address, 
 no ordering  no rows and colums
 to perform set of opeerations itis difficult

 ##### Structured Database:
 Relational Database

              
<table>
<tr>
<td>

Customer Name
| ID  | Name |
|---|---|
| A | Carie |
| B | Jane |

</td>

<!-- Empty space column for distance -->
<td style="width: 50px;"></td> 
<td>
  
Customer Age 
| ID | Age |
|---|---|
| A | 30 |
| B | 36 |

</td>
</tr>
</table>

Same Customer as same id

### Keys

- #### Super Key 
  - Set of all combinations to identify uniquely a row/tuple

| S-ID | Name | Age | Phone
|---|---|---|---|
| 1 | Jane | 36 | 12345 |
| 2 | Laura | 25 | 56789 |

- #### Candidate Key 
  - Subset of Super Key ( Not Null)

| Super Key | Candidate Key |
| --- | --- |
| All Possible | Minimum Possible ombinations |
| Combinations | to identify uniquely |
| (s_id,Name,Phone) | (s_id)
| | (Name, phone_no) |

If we add age in name and phone it will become super key then it will not be minimum so not candidate key

- #### Primary Key 
 - Unique Identifier ( Not Null ) ( No Repetitions )
 - Only one Primary key
 - Primary Key is Subset of Candidate Key

| s_id |
| --- |
| 1 | 
| 2 |
| 3 |

$\text{Primary Key} \subseteq \text{Candidate Key} \subseteq \text{Super Key}$

<img width="324" height="295" alt="image" src="https://github.com/user-attachments/assets/0ef9d8e6-3f74-49a6-bda1-dd7524e31884" />

- #### Unique Key:
 - All Unique value
 - It can be null
e.g.
 CNIC -> Unique
 Childern -> CNIC No. -> Null

- #### Foriegn Key
  - a column (or set of columns) in one table that links to the primary key (or a unique key) in another table
 <table>
<tr>
<td>

Customer Name
| ID  | Name |
|---|---|
| A | Carie |
| B | Jane |
  |
  >
  Primary Key
  
</td>

<!-- Empty space column for distance -->
<td style="width: 50px;"></td> 
<td>
  
Customer Order
| ID | Price | Dine-in/ Take away | Age |
|---|---|---|---|
| A | 30 | D | 21 |
| B | 36 | T | 26 |
| B | 46 | T | 26 |
| A | 56 | D | 21 |
  |
  >
  Foriegn Key


</td>
</tr>
</table>
