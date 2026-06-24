# Relations in Database

## Types of Relations

1. One to One
<img width="207" height="50" alt="image" src="https://github.com/user-attachments/assets/53bc19b5-d171-4ace-a1b1-c7c8779196b8" />

2. One to Many

<img width="208" height="50" alt="image" src="https://github.com/user-attachments/assets/aad56e2e-c327-4bd8-9e47-bc8e00ccc9a4" />

3. Many to Many

<img width="148" height="50" alt="image" src="https://github.com/user-attachments/assets/b59d6d54-1326-4e0f-9963-f1923e572e59" />

4. Many to One

<img width="148" height="50" alt="image" src="https://github.com/user-attachments/assets/5f91a716-173f-4edd-800e-202932968d5a" />

### One - One

<table>
<tr>
<td>

Car Brand
| ID  | Brand |
|---|---|
| 001 | BMW |
| 002 | Tesla |
| 003 | Audi |

</td>

<!-- Empty space column for distance -->
<td style="width: 50px;"></td> 
<td>
  
Car Number Information 
| ID | Brand_id(Chasing) | Number Plate
|---|---|---|
| A | 002 |  |
| B | 001 |  |
| C | 003 |  |

</td>
</tr>
</table>
