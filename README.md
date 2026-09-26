# NETWORKWALKS-RUTUJA-B083-WK3-PM1-PM2-PASSWORD-CRACKING-WITH-JTR-NW-TOOLS
NETWORKWALKS Week 03 – Password Cracking with JTR &amp; Network Tools


PASSWORD CRACKING WITH JTR & NETWORK TOOLS

Building an authorized password recovery and security assessment framework combining offline hash extraction via John the Ripper and browser-based dictionary attacks via Networkwalks utilities.

<img width="1230" height="1279" alt="01" src="https://github.com/user-attachments/assets/c87c5404-b695-477b-8033-8449b3dff4bf" />



⚠️ Liability & Educational Disclaimer

This project is created strictly for educational, cybersecurity training, and authorized laboratory purposes as part of the NETWORKWALKS Week 03 cybersecurity program.

The password recovery and password-cracking techniques demonstrated in this project, including the use of John the Ripper (JTR), Johnny GUI, and Networkwalks tools, must only be used on files, systems, accounts, or data that you own or have explicit permission to test.

The author does not support or encourage unauthorized access, credential theft, privacy violations, or any illegal activity.

All passwords, PDF documents, hashes, and other materials used in this laboratory exercise are intended for controlled educational testing. The techniques demonstrated should not be applied to real-world systems without proper authorization.

The author and project contributors are not responsible for any misuse, damage, data loss, unauthorized access, or legal consequences resulting from the information contained in this repository.

Use these techniques responsibly, ethically, and only within authorized environments.




📝 Project Overview

This project demonstrates the process of password recovery and password cracking using John the Ripper (JTR), Johnny GUI, and Networkwalks tools in a controlled cybersecurity laboratory environment.

The objective of this project is to understand how password-protected PDF documents can be assessed for password strength and how password hashes can be extracted and processed using password-cracking tools.

The project covers different stages of the password recovery process, including:

- Identifying password-protected PDF documents.
- Extracting password hashes from the authorized test files.
- Preparing hash files for password-cracking analysis.
- Using John the Ripper (JTR) to perform password recovery.
- Using Johnny GUI as a graphical interface for JTR.
- Using Networkwalks tools for the assigned password-cracking exercise.
- Verifying recovered passwords in the authorized laboratory files.
- Documenting the complete process with screenshots and observations.

The practical exercise helps demonstrate important cybersecurity concepts such as password security, hashing, password strength, wordlists, brute-force/dictionary-based attacks, and the importance of strong passwords.

All activities in this project are performed strictly within an authorized educational lab environment for cybersecurity learning and awareness.




🧰 Tools & Technologies

Tool / Technology| Category| Description
John the Ripper (JTR)| Password Cracker| Open-source multi-format password recovery tool supporting various hashes.
Johnny GUI| Graphical Interface| Graphical point-and-click interface wrapper for John the Ripper.
Networkwalks Hash Calculator| Web Utility| Browser-based utility used to extract crackable "$pdf$" format hashes.
Networkwalks Password Cracker| Web Cracker| Online dictionary attack tool for evaluating credential strengths.




⚙️ Methodology & Execution

Method 1: Password Cracking with John the Ripper & Johnny GUI (Applied to Multiple Locked PDFs)

- JTR & Johnny Download: Downloaded John the Ripper and the Johnny GUI setup package ("johnny-2.2-win.zip") from the official Openwall website, mirror links, or the course Google Drive folder.


<img width="1599" height="899" alt="02" src="https://github.com/user-attachments/assets/261ccfad-ec4d-45dd-b26b-3a246accf8f4" />


- Application Installation: Located and ran the Johnny installer setup file ("johnny-installer.exe") from the "Downloads" folder to install Johnny on the Windows PC.

<img width="1599" height="875" alt="03" src="https://github.com/user-attachments/assets/93adcc6a-9c3f-47b8-a025-383280f044a3" />



- Binary Path Configuration: Configured Johnny by navigating to "Settings" and mapping the executable path to "john.exe" inside the JTR run folder.


<img width="1599" height="845" alt="04" src="https://github.com/user-attachments/assets/d4c57b4b-bc55-413a-931d-41bec80b1875" />


- PDF Hash Extraction: Uploaded each of the authorized locked PDF files ("My Locked PDF1.pdf", "My Locked PDF2.pdf", and "My Locked PDF3.pdf") sequentially to an authorized PDF hash extractor to obtain their respective hash values.


<img width="921" height="502" alt="05" src="https://github.com/user-attachments/assets/74ad833d-7706-4b01-84d7-25201c0367a4" />

  
  - Extracted the individual hash values for "My Locked PDF1.pdf", "My Locked PDF2.pdf", and "My Locked PDF3.pdf".

- Hash File Preparation: Pasted each extracted hash into Notepad, ensured no extra leading characters remained, and saved them respectively as "hash1.txt", "hash2.txt", and "hash3.txt".

- Attack Initialization: Opened Johnny, selected "Open password file" to load each hash text file sequentially ("hash1.txt", "hash2.txt", and "hash3.txt"), and initiated the process using "Start new attack".

- <img width="927" height="491" alt="06" src="https://github.com/user-attachments/assets/0a2b6df8-5087-440e-92ca-59120d006fb8" />
  Cracking password for my hash for my locked PDF1
  

  <img width="1079" height="568" alt="07" src="https://github.com/user-attachments/assets/c2e8adc6-9f27-4eb3-aef1-d59d108ba314" />
For My locked PDF2


<img width="1079" height="575" alt="08" src="https://github.com/user-attachments/assets/407e7d4c-7405-4b0e-b701-992554bfd85c" />
For locked PDF3


Method 2: Password Cracking with Networkwalks Tools (Applied to Multiple Locked PDFs)

- Hash Calculator Access: Opened the browser-based Networkwalks Hash Calculator utility.

- <img width="1079" height="587" alt="09" src="https://github.com/user-attachments/assets/de23e6ad-17b8-4eca-9f10-ca3a6654ab63" />


- File Upload & Parsing: Uploaded each of the authorized target locked PDF files ("My Locked PDF1.pdf", "My Locked PDF2.pdf", and "My Locked PDF3.pdf") to the Hash Calculator one by one to generate their crackable hash formats.

  <img width="1079" height="577" alt="10" src="https://github.com/user-attachments/assets/4b70aafe-2353-4140-b24d-ad1695167510" />

  - Extracted the individual hash values for each authorized PDF.

- Hash String Retrieval: Copied the complete generated hash strings for each respective PDF document.

- Dictionary Attack Execution: Navigated to the Networkwalks Password Cracker, entered the extracted hashes for the authorized files sequentially, selected the available dictionary option, and started the password-recovery process.
- 
<img width="1080" height="872" alt="WhatsApp Image 2026-09-27 at 4 42 25 AM" src="https://github.com/user-attachments/assets/ff541bbb-5087-45cf-b88c-bac9e12f0443" />
  Figure  handling wordlist and custom upload for My locked PDF1
  


  <img width="1080" height="876" alt="WhatsApp Image 2026-09-27 at 4 42 42 AM" src="https://github.com/user-attachments/assets/d47cf318-d8d5-4d18-b309-4033d3afcc22" />
FOR My locked PDF2



<img width="1080" height="881" alt="WhatsApp Image 2026-09-27 at 4 42 55 AM" src="https://github.com/user-attachments/assets/7f1fb051-84b0-4bf0-8c9b-6f99c3bedd0d" />
For My locked PDF3




Common Step: Document Unlocking (Applicable to Both Methods)

- Document Unlocking: After a password was successfully recovered for an authorized laboratory file, the recovered password was entered into the corresponding PDF reader to verify that the protected PDF could be opened successfully.
- 
<img width="1280" height="651" alt="WhatsApp Image 2026-09-27 at 4 43 18 AM" src="https://github.com/user-attachments/assets/40d8a9d1-1057-4cfa-ba39-031a49fd8489" />
Successfullu unlocked My locked PDF1


<img width="1280" height="654" alt="WhatsApp Image 2026-09-27 at 4 43 18 AM (1)" src="https://github.com/user-attachments/assets/d5e7e2fd-8c48-4600-8b8f-3154a9a07309" />
Successfullu unlocked My locked PDF2


<img width="1280" height="654" alt="WhatsApp Image 2026-09-27 at 4 43 19 AM" src="https://github.com/user-attachments/assets/7e062b8f-9049-4496-8958-19d863f3f147" />
Successfullu unlocked My locked PDF3

- The successful results were documented using screenshots for the project report.

All activities were performed only on authorized educational laboratory files and systems.




⚠️ Problems Faced & Solutions

- Initial Access Denied Error: During Method 2, the first target file ("My Locked PDF1.pdf") displayed an "ACCESS DENIED" message along with an “Exhausted wordlist. No match” status.

- Wordlist Limitation: The default built-in wordlist was insufficient because it did not contain a large enough set of possible passwords or the required password variant.

- Custom Wordlist Resolution: The issue was resolved by using the custom wordlist option with a larger authorized lab wordlist. This provided additional password candidates and allowed the password-recovery process to continue successfully.

- Verification: After the password was recovered, it was entered into the corresponding authorized PDF to verify that the document could be opened successfully.





💡 Lessons Learned

- Gained practical understanding of password cracking and password recovery techniques in a controlled cybersecurity laboratory environment.

- Learned how John the Ripper (JTR) can be used to perform password recovery against supported password hashes.

- Understood the purpose and use of Johnny GUI as a graphical interface for John the Ripper.

- Learned how to extract and prepare PDF password hashes for further security testing.

- Understood the role of wordlists and dictionary-based attacks in password recovery.

- Learned that the effectiveness of a password-cracking attempt depends heavily on the quality and coverage of the wordlist being used.

- Gained experience using Networkwalks Hash Calculator and Networkwalks Password Cracker for the assigned laboratory exercise.

- Learned how to troubleshoot issues such as “Access Denied” and “Exhausted wordlist. No match” during the exercise.

- Understood the importance of using strong, unique passwords to reduce the risk of dictionary-based password attacks.

- Developed better awareness of ethical and responsible cybersecurity practices, including performing security testing only on systems and files for which proper authorization has been provided.



📌 Key Security Concepts & Takeaways

- Encryption vs. Hashing: Encryption is a two-way reversible function for data protection, whereas hashing is a one-way mathematical function used for verification.

- Password Vulnerability: Short or common patterns (such as dictionary words or simple character strings) can be compromised in minutes via automated dictionary attacks.





🔗 Resources

- John the Ripper – Official Website
  "https://www.openwall.com/john/" (https://reference-url-citation.invalid/1)

- John the Ripper – Official GitHub Repository
  "https://github.com/openwall/john" (https://reference-url-citation.invalid/2)

- John the Ripper – Official Documentation
  "John the Ripper Documentation" (https://reference-url-citation.invalid/3)

- John the Ripper – Official Downloads / Packages
  "John the Ripper Packages" (https://reference-url-citation.invalid/4)

- Johnny – Official GitHub Repository
  "Johnny GUI" (https://reference-url-citation.invalid/5)

- Openwall Wordlists
  "Openwall Wordlists" (https://reference-url-citation.invalid/6)



👤 Author

Rutuja Medhekar

Cybersecurity Intern at NETWORKWALKS



🗂️ Project Information

Program Name: Cybersecurity at Networkwalks
Week: 03
Project: Password Cracking with JTR & Network Tools
Repository: GitHub
  
