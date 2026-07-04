Objective
Find the line in data.txt that contains the word millionth.
Commands Used
bash
Run
grep "millionth" data.txt
Explanation
grep searches for text patterns inside files
The pattern "millionth" returns only the matching line containing the password
Key Takeaways
Basic pattern searching with grep
Working with large text files
@@ -0,0 +1,23 @@
Level8.md
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
