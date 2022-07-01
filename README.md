# The Hacker Playbook 1: Updates

1. [ Installing Social Engineering Toolkit (Page 12) ](#SET)
2. [ Saving Custom Password Lists (Page 10) ](#cpl)
3. [ Start Metasploit (Page 7)](#sm)
4. [ Changes with PeepingTom ](#pt)
5. [ Huge list of optional tools ](#ot)
6. [ bypassuac update ](#bpuac)
7. [ Nishang has moved (page 16) ](#nish)
8. [ SMBExec Update (Page 8) ](#smbu)
9. [ PowerShell Invoke-Shellcode (Meterpreter) ](#psisc)
10. [ Obscure System's post-exploitation (Page 121) ](#ospel)
11. [ Index for The Hacker Playbook ](#THPI)
12. [ Free Radius update (Page 205) ](#FRU)
13. [ Mimikatz Binary Update ](#mbu)
14. [ Get in touch ](#git)
15. [ Document info ](#editor)

<a name="SET"></a>
## 1. Installing Social Engineering Toolkit (Page 12)

It looks like there was a change to SET on page 12. Here is the updated GIT Command:

`git clone https://github.com/trustedsec/social-engineer-toolkit.git set/`

<a name="cpl"></a>
## 2. Saving Custom Password Lists (Page 10)

It looks like the old link is now dead
~~https://mega.co.nz/#!3VZiEJ4L!TitrTiiwygI2I_7V2bRWBH6rOqlcJ14tSjss2qR5dqo~~

Try these other links:
- https://mega.co.nz/#!VIwSmYhL!Q_u0io3nSxIeVnquONJcfb7D7aO0_fpi9SxSchR1mTM 
- http://www.filedropper.com/crackstation-human-onlytxt 
- https://www.dropbox.com/s/ucreldsa3qt1rms/crackstation-human-only.txt.gz?dl=0 

Thanks Andreas! 



#### Editors note: I recommend using 10 million passwords instead of trying to find a link through Mega. I *assume* the content within is probalby similar to the original mega file.

`cd /opt/`

`wget https://github.com/danielmiessler/SecLists/raw/master/Passwords/Common-Credentials/10-million-password-list-top-1000000.txt`

<a name="sm"></a>
## 3. Start Metasploit (Page 7)

~~`service Metasploit start`~~

Should be replaced with

`service metasploit start`

Thanks John!

<a name="pt"></a>
## 4. Changes have been made to PeepingTom and I've had problems with the new version.

I have included the old version here: On your Kali Linux Box, run the following commands from a terminal:

`cd /opt/`

`wget http://thehackerplaybook.com/Download/peepingtom.zip`

`unzip peepingtom.zip`

`cd peepingtom`

`chmod +x *`

<a name="ot"></a>
## 5. Huge List of Optional Tools

On your Kali Linux Box, run the following commands from a terminal

`mkdir /opt/gitlist/`

`cd /opt/gitlist`

`git clone https://github.com/macubergeek/gitlist.git`
 
 `cd gitlist`
 
 `chmod +x gitlist.sh`
 
 `./gitlist.sh` 

<a name="bpuac"></a>
## 6. bypassuac Update

The book points to:

~~`wget http://www.secmaniac.com/files/bypassuac.zip`~~

to download the bypassuac files, but the updated link *should* be:

http://thehackerplaybook.com/Download/bypassuac.zip

Thanks Patrick! 

<a name="nish"></a>
## 7. Nishang has moved (Page 16)

Nishang has moved over to github. Instead of:

~~https://code.google.com/p/nishang/downloads/list~~

Try:

https://github.com/samratashok/nishang

Thanks Don!

<a name="smbu"></a>
## 8. SMBExec Update (Page 8)

SMBExec updated and has a new Git Repo. So instead of:

~~`git clone https://github.com/brav0hax/smbexec.git`~~

Try:

`git clone https://github.com/pentestgeek/smbexec.git`

<a name="psisc"></a>
## 9. PowerShell Invoke-Shellcode (Meterpreter)

If you've been hard coding your `Invoke-Shellcode.ps1` files to download and execute from github (Originally found here: ~~https://raw.githubusercontent.com/mattifestation/PowerSploit/master/CodeExecution/Invoke-Shellcode.ps1~~), **make sure** you grab the **newest** one, as the original is not working (on purpose). As stated by mattifestation, you should **NOT** blindly run a remote powershell script from github. If you need to, fork it! 

https://raw.githubusercontent.com/mattifestation/PowerSploit/master/CodeExecution/Invoke--Shellcode.ps1

<a name="ospel"></a>
## 10. Obscure System's post-exploitation (Page 121)

Link fix

http://bit.ly/18dvL0I 

Thanks Joe!

<a name="THPI"></a>
## 11. Index for The Hacker Playbook

Thanks to Joe, he put together an index for The Hacker Playbook!!! 

http://www.cise.ufl.edu/~jnw/thehackerplaybookindex

<a name="FRU"></a>
## 12. Free Radius update (Page 205)
It looks like Free Radius changed their website.

Change:

~~`wget ftp://ftp.freeradius.org/pub/freeradius/freeradius-server-2.1.12. tar.bz2`~~

To:

`wget ftp://ftp.freeradius.org/pub/freeradius/old/freeradius-server-2.1.12.tar.bz2`

Thanks Jason!

<a name="mbu"></a>
## 13. Mimikatz Binary Update

https://github.com/gentilkiwi/mimikatz/releases/latest

<a name="git"></a>
## 14. Get In Touch

If you would like to get in touch with the author or have general inquiries about the book

book@thehackerplaybook.com

<a name="editor"></a>
## 15. Document info

Note: This document was forked and transcribed on 30 JUN 2022. The orginial information was written on/around 2 MAY 2018.
