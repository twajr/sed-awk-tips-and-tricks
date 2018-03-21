# sed-awk-tips-and-tricks
Useful sed and awk scenarios and examples

## The Linux Stream EDitor (sed)
Good tutorial and reference here.
http://www.grymoire.com/Unix/Sed.html

### Basics
Reads as usual from STDIN to STDOUT and uses a regex to extract and/or modify contents of files.
```
cat file.txt | sed 's/Tom/Johnny/g' > file_new.txt
sed 's/Tom|tom/John/g' file.txt
```
