# Password-Generator
import random
import string

def generate_password(length=12):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

if __name__ == "__main__":
    password_length = int(input("Please enter the length of the password you want to generate: "))
    password = generate_password(password_length)
    print("Here is your Generated Password:", password)
