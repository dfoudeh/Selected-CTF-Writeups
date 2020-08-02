
# Password Crack 3

```
7adebe1e15c37e23ab25c40a317b76547a75ad84bf57b378520fd59b66dd9e12

This one needs to be in the flag format first...
```

We can use hashcat with a custom rule to format the passwords we are trying
`^{ ^F ^T ^C ^s ^r ^o ^t ^s ^a ^c $}`

^ appends a character to the front of the string, $ to the end. We create a file called rule and run hashcat with the options

`hashcat -m 1400 sha256 wordlist.txt -r rule --force`

which gets us the flag

`7adebe1e15c37e23ab25c40a317b76547a75ad84bf57b378520fd59b66dd9e12:castorsCTF{theformat!}`
