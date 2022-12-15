# Emoji converter in Python 

Write a python code to append the emoji at the end of the input based on the special character the user has given as input.

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
>good morning :)
good morning 😊 
```

### Example 2
```
>Bad day :(
Bad day 😒
```


