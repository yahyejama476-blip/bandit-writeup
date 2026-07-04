Objective
Scan ports 31000–32000, connect to the SSL port, submit the password, and retrieve an RSA private key.
Commands Used
bash
Run
nmap -p 31000-32000 localhost
openssl s_client -connect localhost:31790 -quiet < /etc/bandit_pass/bandit16
# Save output as bandit17.key then:
chmod 600 bandit17.key
ssh -i bandit17.key bandit17@bandit.labs.overthewire.org -p 2220
Explanation
nmap scans the port range to find open services
One port uses SSL; submitting the password returns a private key
Fix permissions before using the key for SSH
Key Takeaways
Port scanning with Nmap
Combining scanning, TLS, and key auth
