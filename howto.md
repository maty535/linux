# Usefull commands:

### LINUX

Show linux version:

`>> lsb_release -a` 

Install only security updates:

`>> sudo apt-get -s dist-upgrade | grep "^Inst" |  grep -i securi | awk -F " " {'print $2'} |      xargs apt-get -y install`

Check installed locales support:

`>>  locale -a |grep bg`

Check installed fonts which supports bulgarian:

`>> fc-list :lang=bg`


### GIT
List all GIT global settings:

`>> git config --global -l`


Unset Git proxy:
`>> git config --global --unset http.proxy`
