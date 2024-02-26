# Adjust Home-Test

1. How many lines in this file?
```
$ wc -l file.txt 
98 file.txt
```
If we only need the number to use it in another command:
```
$ wc -l < file.txt
98
```

2. How many “Z” Characters in this file ?
```
$ grep -o 'Z' file.txt | wc -l
44
```

3. Find on which line is “Junior”, “Platform” and “Engineer”,not case sensitive.
```
$ grep -inoE "junior|platform|engineer" file.txt
28:PlatForm
65:Junior
88:EngineeR
```

4. Change “Junior” to “Senior”
```
 sed -i 's/Junior/Senior/g' file.txt
```
