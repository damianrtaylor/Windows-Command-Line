# Windows-Command-Line

Create Windows Firewall Rule to Block IP Addresses

Netsh.exe advfirewall firewall add rule name=”Tor Exit Node Block” RemoteIP=146.185.220.0/23, 146.185.220.1 - 146.185.221.254  protocol=any dir=in enable=yes action=block profile=private, public, domain interface=any

Parameters
name= <Name of the rule>
RemoteIP= <Public IP Address> (if more than one IP, seperate with comma or enter a range -> 146.185.220.1 - 146.185.221.254)
program = <”File Executable Path”> (if applicable)
protocol= TCP|UDP|any
dir= in|out 
enable = YES|NO
action = Allow|Block|custom
profile = Private|public|domain|any
