### Create a Session fine collector utility, via this utility we should be able to fine people who came late for meeting. The logic of fine collection is below
- Total fine is 10 multiplied by total students in the batch i.e if there are 30 people total fine is 300 Rs
- Fine will be calculated in percent of delay i.e
- If 2 person came late & each one is late by 5 minute then both of them will be fined 50% of total fine money(300) i.e 150 Rs each
- If 3 person came late by 5, 10 & 15 minutes then the respective fine will be 16%, 33%, 50%

### Now the utility will have below behavious
```
./fineCollector -a attendance -n sandeep -t 10:25 
./fineCollector -a attendance -n ravinder -t 10:29 
./fineCollector -a attendance -n surabhi -t 10:35 
./fineCollector -a attendance -n udit -t 10:40 
./fineCollector -a attendance -n anurag -t 10:45 
./fineCollector -a attendance -n mehul -t 10:30 
```
### This should calculate fine
```
./fineCollector -a calculate
Total Fine -> 10*6 -> 60 Rs
People who are fined
Surabhi -> 16% ->  9.6
Udit -> 33% ->  19.8
Anurag -> 50% ->  30
```

### This should generate an HTML report
```
./fineCollector -a htmlReport
```

