# free cloud-comparison

<table border="1">
<tbody><tr>
<td>name</td>
<td>free space</td>
<td>additional free space</td>
<td>referral code</td>
<td>credit card needed</td>
<td>files expiration</td>
<td>webdav, s3, ftp etc.</td>
<td>note</td>
</tr>

<tr>
<td><a href="https://infini-cloud.net/en/">ininfini-cloud.net</a></td>
<td>20 GB</td>
<td>+5 GB, enter referal code in My Page. <b>Storage bonus valid for one year</b>. </td>
<td>ZPF5G</td>
<td>No</td>
<td>2 years, if not used. You will be warned via e-mail</td>
<td>webdav</td>
<td></td>
</tr>

<tr>
<td><a href="https://tebi.io/">tebi.io</a><a></a></td>
<td>20 GB</td>
<td>?</td>
<td>?</td>
<td>Yes, after 14 days free trial</td>
<td>?</td>
<td>s3, ftp, ftps</td>
<td>250 GB/Month free traffic. You will be charged if you go over that.</td>
</tr>
	
<tr>
<td><a href="https://www.microsoft.com/en-us/microsoft-365/onedrive/free-online-cloud-storage">one drive</a></td>
<td>5 GB</td>
<td>?</td>
<td>?</td>
<td>?</td>
<td>?</td>
<td>webdav NOT supported</td>
<td></td>
</tr>

<tr>
<td><a href="https://drive.google.com/">google drive</a></td>
<td>15 GB</td>
<td>?</td>
<td>?</td>
<td>?</td>
<td>?</td>
<td>webdav NOT supported</td>
<td></td>
</tr>

<tr>
<td><a href="https://mega.io/">mega</a></td>
<td>20 GB</td>
<td>+5 GB for desktop app, mobile app, and invite <b>Storage bonus valid for one year</b>. </td>
<td><a href="https://mega.nz/#newsignupaGF2YWppQHlhaG9vLmNvbYGjvdF7zokU">code</a></td>
<td>?</td>
<td>?</td>
<td>webdav and ftp supported only through local command line server "MEGA CMD"</td>
<td>Download limited. "The limit is based on the amount of data downloaded from your IP address over the past six hours." </td>
</tr>

</tbody></table>



### Mega cmd how to use to get webdav and ftp local server:

<code><pre>
download [megacmd](https://mega.io/cmd)
install
(or, if you unzip to to some folder. you have to start MEGAcmdServer.exe first, 
and then MEGAcmdShell.exe
since app path is hardcoded to your localappfolder  C:\Users\yourname\AppData\Local\MEGAcmd)

-to login to your account inside server emulator, type in MEGAcmdShell window:: 
login your@email.com
enter your password

-to start local 'webdav' server of your mega cloud folder, type in MEGAcmdShell window:
webdav /

(to serve "newfolder" that is created in mega cloud storage, type in:
webdav newfolder)

you can connect to webdav server using winscp, and your mega email and pass,
or "connect to network drive" in windows explorer, without requiring email and pass.
webdav server example:
http://127.0.0.1:4443/someletters/Cloud%20Drive

-to start local 'ftp' server, type in:
ftp /
or 
ftp newfolder
ftp server example:
ftp://127.0.0.1:4990/someletters/Cloud%20Drive

you can see webdav and ftp location by typing 
webdav
or
ftp
after setting them up in MEGAcmdShell.exe

someletters represent your mega web location in browser:
https://mega.nz/fm/someletters

note:
-I got a lot lot of timeout detected using winscp/ftp with 35 mb file, webdav works fine in explorer.
-megacmd will create a lot of temp files in '.megaCmd' subfolder
</pre></code>

<sub>
Q: How do I use html in github MarkDown?  
	
A: As usual, just don't indent, and have one line empty on start and end html.
</sub>
