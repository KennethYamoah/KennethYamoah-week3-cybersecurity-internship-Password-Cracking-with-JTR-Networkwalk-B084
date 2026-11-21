# Week 3 Cybersecurity Internship Project Report

## Title
Password Cracking with NetworkWalks

## Student
Kenneth Yamoah

## Course / Assignment Context
This project is part of a Week 3 cybersecurity internship exercise. It documents the recovery of the password for a protected PDF using a NetworkWalks password-cracking procedure. The exercise was performed in an authorized laboratory environment.

## Abstract
The project demonstrates a controlled password-auditing process. A PDF was protected with a Document Open Password, candidate passwords were tested using a supplied wordlist, and a successful match was found. The recovered password was `password1`. The result was verified by entering the password into the PDF prompt and opening the document.

## 1. Introduction
Weak passwords remain a common security risk because predictable credentials can often be recovered with automated guessing tools. Password-cracking exercises help cybersecurity learners understand password strength, credential risks, and responsible defensive practices.

In this exercise, NetworkWalks was used to test candidate passwords against a password-protected PDF. The result was recorded visually and verified by unlocking the target document.

## 2. Objectives
- Understand the purpose of authorized password auditing.
- Create or obtain a password-protected PDF.
- Use a candidate wordlist against the protected target.
- Record each attempt and identify the successful match.
- Verify the recovered password by opening the PDF.
- Present the final evidence clearly and responsibly.

## 3. Procedure

### 3.1 Prepare the Target
The target file was `My-Locked-PDF1.pdf`. The PDF was protected with a Document Open Password and could not be opened without the correct credential.

### 3.2 Prepare Candidate Passwords
A password wordlist was prepared or supplied with candidate values, including common passwords and the expected weak credential. Typical candidate values included:

```text
service
canada
hockey
killer
george
asdfgh
zxcvbn
qwertyuiop
111222
password1
```

### 3.3 Launch the NetworkWalks Password Attack
The protected PDF was loaded into the NetworkWalks password-cracking workflow. The candidate passwords were tested in sequence against the target password.

During the process, unsuccessful attempts were marked with a red cross. Each candidate was checked until the matching password was found.

### 3.4 Identify the Match
The password candidate `password1` produced a successful match:

```text
MATCH password1
```

A success screen was displayed, identifying `password1` as the PDF password.

### 3.5 Verify the Password
The recovered password was entered in the PDF **Document Open Password** prompt.

1. Open `My-Locked-PDF1.pdf`.
2. Enter `password1` in the password field.
3. Select **OK**.
4. Confirm that the PDF opens successfully.

## 4. Evidence

### Screenshot 1 — Protected PDF Password Prompt
This screenshot shows the protected PDF and the password prompt requesting a Document Open Password. The screen identifies `My-Locked-PDF1.pdf` as the target file.

![Screenshot 1](Screenshot%201.png)

### Screenshot 2 — Candidate Password Attempts
This screenshot shows the NetworkWalks-style cracking output. Several candidate passwords are tested and rejected, including `service`, `canada`, `hockey`, `killer`, `george`, `asdfgh`, `zxcvbn`, `qwertyuiop`, and `111222`. The successful match is `password1`.

![Screenshot 2](Screenshot%202.png)

### Screenshot 3 — Successful Password Result
This screenshot displays the result:

```text
PASSWORD CRACKED SUCCESSFULLY
password1
```

It states that the password should be entered into the PDF to unlock the file.

![Screenshot 3](Screenshot%203.png)

### Screenshot 4 — Completion Confirmation
This screenshot confirms successful completion of the internship exercise and displays the captured flag:

```text
networkwalks_flag1_itr_270521_1
```

![Screenshot 4](Screenshot%204.png)

## 5. Results
The password-cracking process successfully recovered `password1` as the Document Open Password. The success was verified by the displayed result, the password prompt, and the successful capture confirmation.

The attempt demonstrates that a short or predictable password can be discovered from a candidate wordlist. It also demonstrates the importance of using strong, unpredictable passwords and avoiding common password patterns.

## 6. Security and Ethical Considerations
This exercise must only be performed against systems or files that the tester owns or is authorized to assess. Password recovery should not be used to access third-party accounts or documents without permission.

Professional practice includes:
- Obtaining written authorization before testing.
- Limiting testing to the approved target and scope.
- Protecting recovered credentials.
- Reporting weak passwords through an authorized channel.
- Using strong passwords in real-world systems.

## 7. Recommended Defenses
- Use long, unique passwords.
- Use a password manager.
- Enable multi-factor authentication.
- Prohibit commonly used passwords.
- Apply account lockout or rate-limiting controls where appropriate.
- Monitor repeated authentication failures.

## 8. Limitations
A wordlist-based attack can only recover passwords that exist in, or are represented by, the candidate list. The duration and success of the process depend on the password strength, wordlist quality, target format, and available processing capability.

## 9. Conclusion
This Week 3 internship project demonstrated a controlled password-cracking exercise using NetworkWalks tools. The candidate search successfully recovered `password1`, and the result was documented and verified through the supplied evidence screens.