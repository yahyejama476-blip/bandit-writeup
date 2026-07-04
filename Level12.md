Objective
Convert the hex dump data.txt back to binary, then repeatedly decompress multiple archive layers until plaintext is found.
Commands Used
bash
Run
mkdir /tmp/bandit12 && cd /tmp/bandit12
cp ~/data.txt .
xxd -r data.txt > data
file data

# Repeat as needed:
mv data data.gz && gunzip data.gz
mv data data.bz2 && bunzip2 data.bz2
tar xf data
Explanation
xxd -r reverses a hex dump into raw binary
file identifies the compression/archive type
Work in /tmp because the home directory is read-only
Layers alternate between gzip, bzip2, and tar formats
Key Takeaways
Hex dump conversion
Identifying file types
Handling nested compression/archives
