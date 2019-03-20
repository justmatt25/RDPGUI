Simple Remote Desktop Connection Client in PyQt4<br>
<br>
Packages needed: python-qt4, python-configparser,python-urllib3
<br><br>
sudo apt-get install python-qt4 python-configparser python-urllib3
<br>
edit rdpgui.ini to fit your server environment<br>
<br>
config for FreeRDP (older versions are not necessarily supported) > 1.0.1 (new command line release: https://github.com/FreeRDP/FreeRDP/wiki/CommandLineInterface):<br>
[DEFAULT]<br>
RDPBinary = xfreerdp<br>
RDPOptions = <your-file-path-to-rdp-file.rdp><br>
RDPDomain = RPiTC<br>
RDPServer = server1.domain.lan server2.domain.lan server3.domain.lan<br>
RDPDomainFlags = /d:<br>
RDPServerFlags = /v:<br>
RDPUserFlags = /u:<br>
RDPPasswordFlags = /p:<br>
RDPDefaulfFlags = /cert-ignore /f<br>
RDPExtraFlags = /sound:sys:pulse /rfx /fonts<br>
<br>

