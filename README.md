
# SHA-1 Password Cracker  

This Python script attempts to find the plaintext password that matches a given SHA-1 hash by comparing it against a list of potential passwords stored in a text file.  

## How It Works  

1. The user inputs a SHA-1 hash to crack.  
2. The script reads potential passwords from the `passwords.txt` file.  
3. Each password is hashed using SHA-1 and compared to the input hash.  
4. If a match is found, the corresponding plaintext password is displayed.  

## File Structure  

- `password_cracker.py`: The main script containing the SHA-1 cracking logic.  
- `passwords.txt`: A text file containing a list of potential passwords to try. Each password should be on a new line.  

## Requirements  

- Python 3.x  

## Usage  

1. Clone or download the repository.  
2. Place your potential passwords in a file named `passwords.txt` in the same directory as the script.  
3. Run the script:  

    ```bash
    python password_cracker.py
    ```  

4. Enter the SHA-1 hash you want to crack when prompted.  

    Example:  

    ```bash
    Enter the SHA1 for crack: 5baa61e4c9b93f3f0682250b6cf8331b7ee68fd8
    Password found: password
    ```

## Example `passwords.txt`  

```plaintext
password
123456
qwerty
letmein
admin
```

## Contributions  

This project is **100% developed by me**, but you are welcome to use it, learn from it, and contribute to its development!  

### How to Contribute  

1. **Fork the repository**:  
   Click the "Fork" button in the top-right corner of this repository's GitHub page.  

2. **Clone your fork**:  
   ```bash
   git clone https://github.com/<your-username>/sha1-password-cracker.git
   cd sha1-password-cracker
   ```  

3. **Create a new branch**:  
   ```bash
   git checkout -b feature-your-feature-name
   ```  

4. **Make your changes**:  
   Update the code, fix bugs, or add new features.  

5. **Commit your changes**:  
   ```bash
   git add .
   git commit -m "Add your detailed commit message here"
   ```  

6. **Push your branch**:  
   ```bash
   git push origin feature-your-feature-name
   ```  

7. **Create a pull request**:  
   Go to the original repository on GitHub, click the "Pull Request" tab, and submit your changes for review.  

## Limitations  

- This script uses a brute-force approach, so it is limited by the size of the `passwords.txt` file and the computational resources available.  
- It can only crack SHA-1 hashes for which the plaintext password exists in `passwords.txt`.  

## Disclaimer  

This script is intended for educational purposes only. Do not use it for unauthorized or malicious activities. Always ensure you have permission to test or audit password security.  

---

### Author  

- **Name:** Bharat Garsondiya
- **Email:** bgarsond@uoguelph.ca
