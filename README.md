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
<td>+5 GB, enter other persons referal code in 'My Page'. <b>Storage bonus valid for one year</b>. </td>
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
<td><a href="https://mega.io/">mega</a></td>
<td>20 GB</td>
<td>+5 GB for desktop app, mobile app, and invite. <b>Storage bonus valid for one year</b>. </td>
<td><a href="https://mega.nz/#newsignupaGF2YWppQHlhaG9vLmNvbYGjvdF7zokU">code</a></td>
<td>?</td>
<td>?</td>
<td>webdav and ftp supported only through local command line server "MEGA CMD". See below for more info.</td>
<td>Download limited. "The limit is based on the amount of data downloaded from your IP address over the past six hours." </td>
</tr>


<tr>
<td><a href="https://e.mail.ru/">mail.ru</a></td>
<td>8 GB</td>
<td>?</td>
<td>?>code</a></td>
<td>?</td>
<td>?</td>
<td>webdav, you have to enable pass for external apps.</td>
<td>english version of site is at: https://e.mail.ru </td>
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
<td><a href="https://www.microsoft.com/en-us/microsoft-365/onedrive/free-online-cloud-storage">one drive</a></td>
<td>5 GB</td>
<td>?</td>
<td>No</td>
<td>?</td>
<td>?</td>
<td>webdav NOT supported</td>
<td></td>
</tr>

</tbody></table>

<code><pre>

## How to

### How to use 'Mega CMD' to get webdav and ftp local server:


-download [megacmd](https://mega.io/cmd)
-install and start MEGAcmdShell
(or, if you unzip to to some folder, you have to start MEGAcmdServer.exe first, 
and then MEGAcmdShell.exe, since app path is hardcoded to your localappfolder, 
C:\Users\yourname\AppData\Local\MEGAcmd)

-to login to your account inside server emulator, type in MEGAcmdShell window:: 
login your@mega_account_email.com
enter your password

-to start local 'webdav' server of your mega cloud folder, type in MEGAcmdShell window:
webdav /

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
webdav, or ftp, after setting them up in MEGAcmdShell.exe

someletters represent your mega web location in browser:
https://mega.nz/fm/someletters

note:
-I got a lot lot of timeout detected using winscp/ftp with 35 mb file, webdav works fine in explorer.
-megacmd will create a lot of temp files in '.megaCmd' subfolder
-to serve "newfolder" that is created in mega cloud storage, type in: webdav newfolder

### Tebi.io

After a 14-day trial, you will be automatically switched to the Free Tier, 
which offers 25GB of storage in 2 copies and 250GB of outbound transfer each month.
FTP is always available. You will also have to enter your credit card info, 
but they say you won't be charged unless use more than 250 outbound transfer per month

howto to use:
-add bucket, name it ftp1, or whatever
-create master key
-click on edit key, enable ftp in keys
-use key as ftp username 
-click on 'show secret' and use it as ftp password


### Infinicloud

-First copy and save 'apps password' somewhere, it will be only showed once.
-You can reissue it later, but it will take few minutes to refresh.
-To enable ftp, go to my page and enable 'Turn on Apps Connection'
-Use your username as ftp username, and 'apps password' as ftp password.

### mail.ru - https://e.mail.ru/ 
-login, click on settings / security in bottom left, or go to https://id.mail.ru/security
-click on 'create passwords for external apps' at the bottom
-click on 'create', name it 'webdav'
-enable webdav
-enter your password
-copy new auto created pass for webdav
-webdav server is webdav.cloud.mail.ru




</pre></code>

<sub>
Q: How do I use html in github MarkDown?  
	
A: As usual, just don't indent, and have one line empty on start and end html.
</sub>


