# Exp 5 - Metasploit for Reconnaissance
## T.Mnaikandan
## 212224110037
## AIM:
To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:
Install kali linux either in partition or virtual box or in live mode

### Step 2:
Investigate on the various categories of tools as follows:

### Step 3:
Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:

Find out the ip address of the attackers system

### OUTPUT:

<img width="565" height="359" alt="image" src="https://github.com/user-attachments/assets/c0b64fb6-504a-4d9f-b3f6-2b1e30c1fca4" />


## Invoke msfconsole

### OUTPUT:

<img width="480" height="471" alt="image" src="https://github.com/user-attachments/assets/b05c908d-0937-4e4e-9c54-6eddc44026e8" />


Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

<img width="615" height="585" alt="image" src="https://github.com/user-attachments/assets/55848b04-9236-48be-bdf8-2eedc7e0b0c1" />


## Port scanning:

### msf > nmap -sT 192.168.1810/24-p1-1000
<img width="403" height="229" alt="image" src="https://github.com/user-attachments/assets/f4f8945c-8324-4a66-a4f2-27633ca95612" />



### msf > db_nmap 192.168.181.0/24

<img width="546" height="127" alt="image" src="https://github.com/user-attachments/assets/2c3ff682-d95f-4e4b-a007-2cfae288f5f2" />



### kali > ls-l

<img width="640" height="107" alt="image" src="https://github.com/user-attachments/assets/3eb08660-5fd8-490b-8114-07b590f198e9" />



### info
<img width="979" height="913" alt="image" src="https://github.com/user-attachments/assets/d7469ad0-553a-428a-a60d-c4e365dd61f0" />




## MYSQL ENUMERATION

### db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

<img width="635" height="152" alt="image" src="https://github.com/user-attachments/assets/44f127ab-604c-45c9-9e79-6512149301a2" />


### search

<img width="925" height="297" alt="image" src="https://github.com/user-attachments/assets/4153cb37-257d-4196-8b10-314b0adc973c" />


###  use 11 Or: use auxiliary/scanner/mysql/mysql_version

<img width="798" height="276" alt="image" src="https://github.com/user-attachments/assets/fc838947-821c-48f4-aed9-31cc6d8d6363" />


### Use the set rhosts command to set the parameter and run the module, as follows:

<img width="425" height="81" alt="image" src="https://github.com/user-attachments/assets/c0b0be2e-58d6-4b05-a503-6c6abb44abcc" />


### After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module.

<img width="858" height="392" alt="image" src="https://github.com/user-attachments/assets/a07b241a-eca3-4be8-8cbe-4302e5812ae5" />


### /usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt 

<img width="858" height="392" alt="image" src="https://github.com/user-attachments/assets/5e91dfd0-980f-483a-9e4f-73a7f11a6420" />


<img width="636" height="108" alt="image" src="https://github.com/user-attachments/assets/c14e7666-86a9-42c9-ab97-3450bb2a9c27" />


## RESULT:
The Metasploit framework for reconnaissance is  examined successfully.
