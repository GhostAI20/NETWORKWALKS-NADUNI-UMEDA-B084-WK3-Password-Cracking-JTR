# NETWORKWALKS - Week 03 - Password Cracking with John the Ripper

- **Name:** Naduni Umeda
- **Batch:** B084
- **Module:** NETWORKWALKS - WK3

## Overview
- This project shows 2 ways to crack passwords
- Activity 01 - Kali Terminal + John the Ripper
- Activity 02 - Web Tools

---

## Activity 01 - Kali Terminal (PDF Password Cracking)

### Tools Used:
- Kali Linux
- pdf2john
- John the Ripper
- Google Drive + Firefox

### What I Did:
- First I tried to find the PDF file inside Kali, but I could not find it
- Then I uploaded the PDF from Windows to Google Drive
- Then I opened Firefox inside Kali and downloaded the PDF from Google Drive
- After that I could use pdf2john

### Steps:
- Used `pdf2john` to extract hash from PDF
- Saved hash to `hash.txt`
- Used John the Ripper with `rockyou.txt` wordlist
- Successfully cracked the PDF password

### Errors I Faced & How I Fixed:
- **Error 1:** PDF file not found in Kali
    - **Fix:** Uploaded PDF from Windows to Google Drive, then downloaded it in Kali using Firefox
- **Error 2:** `pdf2john` command error
    - **Fix:** Checked file path again and ran command with correct file name
- **Error 3:** John the Ripper did not start / wordlist not found
    - **Fix:** Used correct path for `rockyou.txt` and ran again

### Screenshots:

- Step 01 - pdf2john:
![01-pdf2john](activity-01-kali-terminal/01-pdf2john.png)

- Step 02 - Error:
![02-error](activity-01-kali-terminal/02-error.png)
![02-error.1](activity-01-kali-terminal/02-error.1.png)

- Step 03 - Fix:
![03-fix](activity-01-kali-terminal/03-fix.png)
![solution](activity-01-kali-terminal/solution.png)


- Step 04 - Cracked:
![04-cracked](activity-01-kali-terminal/04-cracked.png)

- Step 05 - Show Password:
![05-show](activity-01-kali-terminal/05-show.png)

- Step 06 - Congratulations:
![06-congratulations](activity-01-kali-terminal/06-congratulations.png)

- Step 07 - Congratulations Full:
![07-congratulations-full](activity-01-kali-terminal/07-congratulations-full.png)

---

## Activity 02 - Web Tools (Hash Cracking)

### Tools Used:
- Online Hash Calculator
- Online Hash Cracker

### Steps:
- Calculated hash using Hash Calculator
- Pasted hash into Cracker tool
- Found the original password
- Entered password and got Congratulations + Flag

### Screenshots:

- Step 01 - Hash Calculator:
![01-hash-calculator](activity-02-web-tools/01-hash-calculator.png)

- Step 02 - Cracker:
![02-cracker](activity-02-web-tools/02-cracker.png)

- Step 03 - Password Found:
![03-password-found](activity-02-web-tools/03-password-found.png)

- Step 04 - Enter Password:
![04-enter-password](activity-02-web-tools/04-enter-password.png)

- Step 05 - Congratulations:
![05-congratulations](activity-02-web-tools/05-congratulations.png)

---

## Key Learning
- Weak passwords can be cracked easily with wordlist attacks
- PDF protection alone is not enough if password is weak
- Always use strong, unique passwords
- Troubleshooting is part of hacking - file path, tools, errors check karanna ona

## Repository Structure
- `activity-01-kali-terminal/` - Kali screenshots
- `activity-02-web-tools/` - Web screenshots + hash.txt
- `README.md` - This file
