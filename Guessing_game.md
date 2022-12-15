# Guessing game in Python 

Write a python code to guess the number form 0 - 9

Conditions :
- The user will be given 3 chance.

```
secret_number = random.randint(0, 9)  
chance = 0  
  
while chance < 3:  
    guess = int(input("Enter the number : "))  
    if guess == secret_number:  
        print(f"answer is correct!! you won the game")  
        break  
 else:  
        print("Try again!!")  
    chance +=1  
else:  
    print("BAD LUCK :(")  
    print(f'The secret number is {secret_number}')
```

## Example
### Example 1
```
Enter the number : 2
Try again!!
Enter the number : 5
Try again!!
Enter the number : 1
Try again!!
BAD LUCK :(
The secret number is 7
```

### Example 2
```
Enter the number : 3
Try again!!
Enter the number : 0
answer is correct!! you won the game
```


