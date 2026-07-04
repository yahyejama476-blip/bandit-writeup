Objective
Find the only unique line in data.txt — every other line appears exactly twice.
Commands Used
bash
Run
sort data.txt | uniq -u
Explanation
sort groups identical lines together
uniq -u prints only lines that occur exactly once
The pipe | sends output from one command to the next
Key Takeaways
Sorting and deduplicating text
Using command pipelines
uniq flags for unique/duplicate filtering
