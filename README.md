Update 38

For those who have versions before 10 have to send this command in putty.
After sending the command, make full remake to the main

 
1
if you have problems with updates go in the Main /etc/sudoers and modify
 
xtreamcodes ALL=(root) NOPASSWD: /sbin/iptables
 
to look like this:
 
xtreamcodes ALL=(root) NOPASSWD: /sbin/iptables, /usr/bin/chattr
 
2
go to /home/xtreamcodes/iptv_xtream_codes/adtools/balancer if you have any .json in that folder delect
 
3
when doing Full Remake on Main or Balance wait whenever the operation is finished to do it again (all done calm ... Rome is not built in a day)
 
4
password cannot contain odd characters like ? or # etc etc



After Update insert password and port on manager servers in Main and LB for the functions to work

clear Browser cache

Update

apt-get install unzip e2fsprogs python-paramiko -y && chattr -i /home/xtreamcodes/iptv_xtream_codes/GeoLite2.mmdb && rm -rf /home/xtreamcodes/iptv_xtream_codes/admin && rm -rf /home/xtreamcodes/iptv_xtream_codes/pytools && wget "http://xcodes.mine.nu/XCodes/update.zip" -O /tmp/update.zip -o /dev/null && unzip /tmp/update.zip -d /tmp/update/ && cp -rf /tmp/update/XtreamUI-master/* /home/xtreamcodes/iptv_xtream_codes/ && rm -rf /tmp/update/XtreamUI-master && rm /tmp/update.zip && rm -rf /tmp/update  && chown -R xtreamcodes:xtreamcodes /home/xtreamcodes/ && chmod +x /home/xtreamcodes/iptv_xtream_codes/permissions.sh && /home/xtreamcodes/iptv_xtream_codes/permissions.sh && find /home/xtreamcodes/ -type d -not \( -name .update -prune \) -exec chmod -R 777 {} + && /home/xtreamcodes/iptv_xtream_codes/start_services.sh && chattr +i /home/xtreamcodes/iptv_xtream_codes/GeoLite2.mmdb
clean installation 22 CK MODS (install.py) with Mysql:

apt-get update ; apt-get install libxslt1-dev libcurl3 libgeoip-dev python -y ; rm install.py ; rm install_XCUI.py?dl=0 ; wget https://www.dropbox.com/s/25b20wik96o0xgx/install_XCUI.py?dl=0 ; cp install_XCUI.py?dl=0 install.py ; sudo python install.py



