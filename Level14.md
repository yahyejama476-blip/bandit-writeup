Objective
Send the bandit14 password to the service running on localhost port 30000.
Commands Used
bash
Run
cat /etc/bandit_pass/bandit14 | nc localhost 30000
Explanation
/etc/bandit_pass/ stores passwords for each level
nc (netcat) opens a raw TCP connection to the target port
The password is sent over the connection, and the service replies with the next password
Key Takeaways
Using netcat for TCP connections
Reading system-level credential files
