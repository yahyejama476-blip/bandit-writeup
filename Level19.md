Objective
Run the setuid binary bandit20-do to execute commands as bandit20.
Commands Used
bash
Run
ls -l bandit20-do
./bandit20-do cat /etc/bandit_pass/bandit20
Explanation
The s permission bit means the program runs as its owner (bandit20), not the caller
This lets you read the password file normally restricted to bandit20
Key Takeaways
Setuid/setgid permissions
Privilege escalation via file permissions
