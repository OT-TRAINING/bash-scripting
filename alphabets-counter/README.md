WAP to find count of  alphabets in a file

if the content of file names.txt is  below
```
sandeep
ravinder
```

The outcome of script would be 
```
./findAlpabetCounts.sh names.txt
2 a
2 d
3 e
1 i
2 n
1 p
2 r
1 s
1 v
```
Add other capabilities

Find only vowels
```
./findAlpabetCounts.sh -f v names.txt
2 a
3 e
1 i
```
Find only consonants
```
./findAlpabetCounts.sh -f c names.txt
2 d
2 n
1 p
2 r
1 s
1 v
```