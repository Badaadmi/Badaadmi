import random
import string

def generate_password(length=8):
    # Define the characters to be used in the password
    characters = string.ascii_letters + string.digits + string.punctuation

    # Generate a random password by selecting characters randomly
    password = ''.join(random.choice(characters) for _ in range(length))

    return password

# Generate a password with default length of 8 characters
password = generate_password()
print("Generated Password:", password)

# Generate a password with a specified length
password = generate_password(12)
print("Generated Password:", password)
