Objective
Extract human-readable text from the binary file data.txt and find the password after several = characters.
Commands Used
bash
Run
strings data.txt | grep "=="
Explanation
strings pulls printable characters from binary/non-text files
grep "==" filters for lines with double equals signs to isolate the password
Key Takeaways
Examining binary files
Using strings for embedded text
Combining filters with pipes
