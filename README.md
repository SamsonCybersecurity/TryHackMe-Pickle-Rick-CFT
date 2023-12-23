<h1>TryHackMe | Pickle Rick CTF</h1>


<h2>Description</h2>
This Rick and Morty-themed challenge requires you to exploit a web server and find three ingredients to help Rick make his potion and transform himself back into a human from a pickle.
<br />


<h2>Utilities Used</h2>

- <b>Nmap</b> 
- <b>Nikto</b>
- <b>Gobuster</b>

<h2>Environments Used </h2>

- <b>Linux </b> (Ubuntu)

<h2>CTF Walk-through:</h2>

<p align="center">
Run an nmap scan: <br/>
<img src="https://i.imgur.com/JlmJ65U.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Go to http://10.10.68.85/:  <br/>
<img src="https://i.imgur.com/G1MdOj1.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
View source page: <br/>
<img src="https://i.imgur.com/M97eBbM.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Nikto Scan:  <br/>
<img src="https://i.imgur.com/MYnyIlR.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<img src="https://i.imgur.com/sApY91H.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Gobuster Scan:  <br/>
<img src="https://i.imgur.com/tXkrLDa.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Portal Login Page:  <br/>
<img src="https://i.imgur.com/gks6qb3.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
ls command panel:  <br/>
<img src="https://i.imgur.com/5HCBQix.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
cat Sup3rS3cretPickl3Ingred.txt :  <br/>
<img src="https://i.imgur.com/NXqRG8I.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Sudo ls ../../../home:  <br/>
<img src="https://i.imgur.com/q3qNAbv.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Sudo ls ../../../home/rick:  <br/>
<img src="https://i.imgur.com/5Eh7Mu5.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Sudo ls ../../../home/rick/"second ingredients":  <br/>
<img src="https://i.imgur.com/0SK8EtO.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Sudo ls../../root:  <br/>
<img src="https://i.imgur.com/fFPz1IX.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
<br />
<br />
Sudo less../../root/3rd/text:  <br/>
<img src="https://i.imgur.com/pAIJopL.png" height="80%" width="80%" alt="TryHackMe | Pickle Rick CTF Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
