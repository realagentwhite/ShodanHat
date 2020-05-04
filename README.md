
# ShodanHat - Shodan scanner
===

### About
This is a shodan scanner made in **python2**. I am trying to find a way to 
upgrade it to **python3**. (Check **TODO** at the bottom)


## NOTE!!!
I am not the owner of this tool but since it has been long time without maintaining it,
I have forked it and decided to try maintaining it by adding improvements.

# Requirements
If you do not install the deps. below, the script will automatically install for you
then restart the tool. 

You need to install shodan with pip install shodan or easy_install shodan.<br />
You need to install python-nmap with pip install python-nmap.<br />
You need to set your API Key in the 'constantes.py' file.

# Options
-h, --help                 show this help message and exit<br />
-i IP, --ip=IP             info about one host<br />
-l LIST, --list=LIST       info about a list of hosts<br />
-s SQ, --sq=SQ             searchquery string<br />
--nmap                     perform a nmap scan in the hosts<br />
--setkey=SETKEY		       set your api key automatically<br />
-r RANGE, --range=RANGE    scan a range of ips. ex: 192.168.1.1-192.168.1.255<br />
-o OUTPUT, --output=OUTPUT specify a output file<br /><br />

Nmap Options:<br />
--sS                  TCP Syn Scan<br />
--sT                  TCP Connect Scan<br />
--sU                  UDP Scan

# Usage
<em>For One Host<em><br />
python shodanhat.py -i IP<br />
<em>For a list of Hosts</em><br />
python shodanhat.py -l list.txt<br />
You can also set a searchquery to make a specific query with '-s' option!

# TODO
- Upgrade from python2 to python3 as python2 is no longer being used most of the time
