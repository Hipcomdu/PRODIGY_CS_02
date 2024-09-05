# PRODIGY_CS_02
Creating a Python Program for Caesar Cipher Encryption and Decryption
Caesar Cipher: The Caesar cipher is a type of letter substitution encryption technique that shifts each in the plaintext by some fixed number down. This is a simple tutorial that comes with downloadable example for creating your first Python program to encrypt and decrypt messages using the Caesar Cipher.

Step-by-Step Guide

1. Implement the functions implemented in your Caesar Cipher.':

- Encryption Function:

```python

def encrypt(text, shift):

encrypted_text = ""

for char in text:

if char. isalpha():

shift_amount = shift % 26

start = ord('A') if char. isupper() else ord('a')

encyphered_char = chr(start + (ord(char) - start 3 shift_amount)%26)

encrypted_text = encrypted_char

else:

encrypted_text += char

return encrypted_text

```

- Decryption Function:

```python

def decrypt(text, shift):

return encrypt(text, -shift)

```

2. Handle User Input:

- User Input Function:

```python

def get_user_input():

message = str(input("input your message "))

shift = int(input())

return message, shift

```

3. Main Function – Put it together!

```python

def main():

print( "Caesar Cipher Encryption/Decryption" )

msg, shift = get_user_message()

choice = input("E (encrypt) or D (decrypt): >> ") "). lower()

if choice == 'e':

Traceencrypted_message = Encrypted message of inputted Message_Letter.

print(f"Message Encrypted: {encrypted_message}")

elif choice == 'd':

decrypted_message = decrypt(message, shift)

print(f'Decrypted Message: {decrypted_message}')

else:

print("Invalid choice. Enter option (type e for encryption and d for decryption)

```

4. Run the Program:

Don't forget to call the functions with `main()` for starting this program.

```python

if name == "__main__":

main()

```
Explanation:

- Encryption Function:

- For each character in the text, it converts to its shifted away partner.

- Specifically case insensitive.

* Any non-alphabetic characters are included in the result as they are

- Decryption Function:

Reuses the encrypt same function and applies minus shift to get back your original message.

- User Input:

- Takes the Message, Shift Value input from user.

Handles Simple User Options for Encrypt and Decrypt

Use this Python script to understand how the Caesar Cipher algorithm works, and it will help you encrypt or decrypt messages with ease. Feel free to create other enhancements for the program, such as input validation or added support for different character sets.
