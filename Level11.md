Objective
Decode text encoded with ROT13 Caesar cipher in data.txt.
Commands Used
bash
Run
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
Explanation
tr translates or substitutes characters
ROT13 shifts every letter 13 places forward in the alphabet
The mapping A-Z → N-ZA-M and a-z → n-za-m reverses the shift
Key Takeaways
Simple substitution ciphers
Character translation with tr
