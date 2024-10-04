import random
import string

def generate_password(length=12):
    # Define the characters to choose from
    lowercase = string.ascii_lowercase
    uppercase = string.ascii_uppercase
    digits = string.digits
    special_chars = string.punctuation
    
    # Combine all characters
    all_chars = lowercase + uppercase + digits + special_chars
    
    # Ensure the password has at least one of each character type
    password = [
        random.choice(lowercase),
        random.choice(uppercase),
        random.choice(digits),
        random.choice(special_chars)
    ]
    
    # Fill the rest of the password length with random choices
    password += random.choices(all_chars, k=length - 4)
    
    # Shuffle the resulting password list
    random.shuffle(password)
    
    # Join the list into a string
    return ''.join(password)

# Generate and print a random password
if __name__ == "__main__":
    print("Random Password:", generate_password(12))
