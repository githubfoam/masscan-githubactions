# masscan-githubactions-
[![masscan with ubuntu 20.04 CI workflow](https://github.com/githubfoam/masscan-githubactions/actions/workflows/ubuntu-2004-masscan-wf.yml/badge.svg)](https://github.com/githubfoam/masscan-githubactions/actions/workflows/ubuntu-2004-masscan-wf.yml)  
[![masscan with ubuntu 16.04 CI workflow](https://github.com/githubfoam/masscan-githubactions/actions/workflows/ubuntu-1604-masscan.yml/badge.svg)](https://github.com/githubfoam/masscan-githubactions/actions/workflows/ubuntu-1604-masscan.yml)  
[![masscan with kalilinux CI workflow](https://github.com/githubfoam/masscan-githubactions/actions/workflows/kali-masscan-wf.yml/badge.svg)](https://github.com/githubfoam/masscan-githubactions/actions/workflows/kali-masscan-wf.yml)  
[![masscan with debian buster CI workflow](https://github.com/githubfoam/masscan-githubactions/actions/workflows/debian-buster-masscan-wf.yml/badge.svg)](https://github.com/githubfoam/masscan-githubactions/actions/workflows/debian-buster-masscan-wf.yml)  
[![masscan with debian bullseye CI workflow](https://github.com/githubfoam/masscan-githubactions/actions/workflows/debian-bullseye-masscan-wf.yml/badge.svg)](https://github.com/githubfoam/masscan-githubactions/actions/workflows/debian-bullseye-masscan-wf.yml)  

~~~~

$ git clone https://github.com/githubfoam/masscan-githubactions.git
$ docker build -t masscan/kalilinux . --file masscan-githubactions/dockerfiles/Dockerfile.kali.masscan
$ docker image ls
REPOSITORY               TAG       IMAGE ID       CREATED         SIZE
masscan/kalilinux        latest    f7927dbe090b   2 minutes ago   165MB
$ docker run masscan/kalilinux:latest -h                                                                        125 ⨯
usage:
masscan -p80,8000-8100 10.0.0.0/8 --rate=10000
 scan some web ports on 10.x.x.x at 10kpps
masscan --nmap
 list those options that are compatible with nmap
masscan -p80 10.0.0.0/8 --banners -oB <filename>
 save results of scan in binary format to <filename>
masscan --open --banners --readscan <filename> -oX <savefile>
 read binary scan results in <filename> and save them as xml in <savefile>
$ docker run masscan/kalilinux:latest 10.10.10.1/24 -p80

~~~~
~~~~
https://github.com/robertdavidgraham/masscan
~~~~
