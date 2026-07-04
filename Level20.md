Objective
Start a listener on a local port, let the setuid service connect back and verify your password, then receive the next password.
Commands Used
bash
Run
# Terminal 1 (listener):
nc -l -p 12345 < /etc/bandit_pass/bandit20

# Terminal 2 (run the suid binary):
./suconnect 12345
Explanation
nc -l -p listens for incoming connections on the chosen port
suconnect connects to your listener, checks the password, and returns the next one on success
Key Takeaways
Reverse connections / bind shells
Two-way network verification
Using netcat as a listener
