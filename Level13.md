Objective
Use the provided SSH private key to log into bandit14 without a password.
Commands Used
bash
Run
cat sshkey.private
# Save locally as bandit14.key then:
chmod 600 bandit14.key
ssh -i bandit14.key bandit14@bandit.labs.overthewire.org -p 2220
Explanation
-i specifies an identity (private key) file
chmod 600 is required — SSH rejects keys with loose permissions
Key-based authentication replaces password login
Key Takeaways
SSH key-based authentication
Private key permission requirements
