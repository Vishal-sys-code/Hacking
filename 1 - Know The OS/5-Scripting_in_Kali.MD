# Scripting in Bash (Kali Linux Version)

**_It might seem overlwhelming at first, but what will be doing is building an IP sweeper script. Basically, we will write an script that will ping all the IP address in the given range and filter out the IPs that responded and save it in a text file._**

```
#!/bin/bash
for ip in `seq 1-254`;do
ping -c 1 $1.$ip | grep "64 bytes" | cut -d "" -f 4 | tr -d ":" & 
done
```

* Write the above file as the ```ipsweep.sh``` file

* To run the file save the file and hit the below command
```
./ipsweep.sh [first three ranges of your IP]
```

Example: 
```
./ipsweep.sh 192.186.1
```