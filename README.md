# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
![image](https://github.com/user-attachments/assets/e3799741-8857-46c2-bc0a-64aabf46b181)



Invoke msfconsole:
## OUTPUT:
![image](https://github.com/user-attachments/assets/38b39bfc-8277-4088-997c-548a48fa1d33)

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.
![image](https://github.com/user-attachments/assets/77825746-89b4-45e6-9b22-5c9a657da087)

Port Scanning:

Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).

msf > nmap -sT 192.168.1810/24 -p1-1000
![image](https://github.com/user-attachments/assets/ff9e7997-1479-442e-b24c-55e584ff9ea8)

step4: use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.

msf > db_nmap 192.168.181.0/24

![image](https://github.com/user-attachments/assets/f7550393-dc7c-49c8-9248-be533651eb3c)

Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to

Metasploit's auxiliary modules and list all the scanner modules.

cd /usr/share /metasploit-framework/modules/auxiliary

kali > ls -l

![image](https://github.com/user-attachments/assets/2acfba34-35be-47e8-9425-fcb419b739b5)

Search is a powerful command in Metasploit that you can use to find what you want to locate.

msf >search name:Microsoft type:exploit

![image](https://github.com/user-attachments/assets/65985d14-de59-4fd8-8e3b-854659d3b992)
search type:auxiliary mysql
![image](https://github.com/user-attachments/assets/75a6e995-2e22-43fc-857c-bb6e26ee70aa)

search type:auxiliary mysql
![image](https://github.com/user-attachments/assets/7b6c961a-8267-49de-8fbc-a294d1c43d4b)

use 11
![image](https://github.com/user-attachments/assets/db0da20c-bc44-4b36-81d1-dca9c1fbd1cd)

set RHOSTS
![image](https://github.com/user-attachments/assets/3d8bc098-38b4-4449-a802-d0395fa0d79b)

use auxiliary/scanner/mysql/mysql_login



set PASS_FILE /usr/share/wordlists/rockyou.txt

set RHOSTS

set BLANK_PASSWORDS true

set verbose no

run

![image](https://github.com/user-attachments/assets/ee14073d-9e4a-4301-a452-1347a3ac715f)















## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
