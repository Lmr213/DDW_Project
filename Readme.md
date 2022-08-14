# Fuzzing test

## Using the fuzzing test tool - Wfuzz
### Using the commoned line to install Wfuzz and execute the test:
### Install Wfuzz
```
sudo pip3 install wfuzz
```
### download the wordlist
for our project we used SecLists from https://github.com/danielmiessler/SecLists

### start testing
```
wfuzz
```
### test certain function on the website
```
wfuzz -c -z file,full file path that in SecList folder that you want to use for testing -d "parameter1=value1&parameter2=FUZZ" https://ascenda-hotel-booking.herokuapp.com/login
```
### Examples:
```
wfuzz -c -z file,/Users/lmr/SecLists/Fuzzing/4-digits-0000-9999.txt -d "email=768@qq.com&password=FUZZ" https://ascenda-hotel-booking.herokuapp.com/login
```
```
wfuzz -c -z file,/Users/lmr/SecLists/Fuzzing/SQLi/Generic-SQLi.txt -d "email=768@qq.com&password=FUZZ" https://ascenda-hotel-booking.herokuapp.com/login
```



