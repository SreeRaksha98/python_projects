# String Transformation code in Python 

Write a python code to capitalize string with following condition. Each string should be altered using the provided algorithm to produce the new sentence.

Conditions :
- The string's initial character shouldn't change.
- Take into account a letter that comes before it, say y, for each character after that, say x:
		- change x to uppercase if the English alphabet's y comes before it.
		- change x to lowercase if x in the English alphabet comes before y.
- The letter should be unchanged if both are equal.

```
str1 = 'ACdeFA /  SacHeEDea .ssfds'  
lst1 = ''
  
for i in range(len(str1)):  
    if i == 0 or (str1[i - 1] == ' ') or ((str1[i - 1] >= '!') and (str1[i - 1] <= '@')):  
        lst1 += (str1[i])  
    elif str1[i].capitalize() > str1[i - 1].capitalize():  
        lst1 += str1[i].capitalize()  
    elif str1[i].capitalize() < str1[i - 1].capitalize():  
        lst1 += str1[i].lower()  
    else:  
        lst1 += (str1[i])  
  
print(lst1)
```

## Example
### Example 1
* Input : `ACDefA SacHEdea`
* Expected output : `ACDEFa SaCHedEa`
### Example 2
* Input : `ACdeFA /  SacHeEDea .ssfds`
* Expected output : `ACDEFa /  SaCHeEdEa .SsfdS`


