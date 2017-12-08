Usefull commands:

Show linux version:
>> lsb_release -a 

Install only security updates:

>> sudo apt-get -s dist-upgrade | grep "^Inst" |  grep -i securi | awk -F " " {'print $2'} |      xargs apt-get install


List all GIT global settings:

>> git config --global -l


Unset Git proxy:
>> git config --global --unset http.proxy
