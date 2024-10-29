
# Random Secure Password Generator 🔒

This Python script generates a secure password with a mix of uppercase, lowercase letters, digits, and special characters. 

## 📄 Code Explanation

```python
import random
import string

def generate_password(length=12):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for i in range(length))
    return password

print(f"secure password: {generate_password()}")

```
## 📋 Step-by-Step Breakdown

 1.  **Imports**
 
`random` and `string` libraries.
`random` selects random characters, while `string` provides character sets (letters, digits, and punctuation).

 2.  **Function**

  Generates a password of default length **12 characters** (modifiable by passing a different length).
    Combines all **letters**, **digits**, and **symbols** for high security.
    
 3.  **Password Creation**
 
Combines `string.ascii_letters`, `string.digits`, and `string.punctuation` into `characters`.
Uses a **list comprehension** to pick `length` random characters from `characters`, forming the password.

4.  **Output**
Prints the generated password labeled as `"secure password:"`.

## 🚀 Example Output
```python
secure password: &Zr9@eYq2#Pw
```

 > TIP: Customize the `length` parameter to control password length as needed!
 
 ## 📦 How to Run

 1.  Clone this repository or copy the code.
 2.  Run the script in a Python environment:
	 - ```python passgen.py```


