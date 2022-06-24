The problem statement :

Caesar Cipher (caesar.sh)

A Caesar cipher is a simple substitution cipher in which each letter of the plain text is substituted with a letter found by moving n places down the alphabet. For example, assume the input plain text is the following:

abcd xyz
If the shift value, n, is 4, then the encrypted text would be the following:

efgh bcd
You are to write a utiliy that accepts two arguments, a plain-text message and a number of letters to shift in the cipher. The function will return an encrypted string with all letters transformed and all punctuation and whitespace remaining unchanged

./caesar.sh -e "abcd xyz" 4
output:
efgh bcd

You can also update the above utiliy as a caesar cipher decoder 
./caesar.sh -d "efgh bcd" 4

output:
abcd xyz
