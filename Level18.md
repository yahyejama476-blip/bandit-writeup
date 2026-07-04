Objective
The .bashrc logs you out immediately — run commands before the shell loads.
Commands Used
bash
Run
ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme
# Or get a minimal shell:
ssh bandit18@bandit.labs.overthewire.org -p 2220 "bash --noprofile --norc"
Explanation
Any command appended to the SSH line runs before startup scripts
--noprofile --norc skips .bashrc entirely to get an interactive shell
Key Takeaways
Running commands over SSH directly
Bypassing shell startup scripts
