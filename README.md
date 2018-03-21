# sed-awk-tips-and-tricks
Useful sed and awk scenarios and examples

## The Linux Stream EDitor (sed) and AWK
Good tutorial and reference here for sed:
http://www.grymoire.com/Unix/Sed.html
and awk:
http://www.grymoire.com/Unix/Awk.html

### sed Basics
Reads as usual from STDIN to STDOUT and uses a regex to extract and/or modify contents of files. Command format is:
```
sed [command][delimiter]text[delimiter]text[delemiter] [flags]
sed s :Tom:John:g file.txt
sed (s)ubstituion :Tom:John:(g)lobal
```

```
cat file.txt | sed 's/Tom/Johnny/g' > file_new.txt
sed 's/Tom|tom/John/g' file.txt
```
