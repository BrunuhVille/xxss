#### normal dd
wget 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && chmod 777 InstallNET.sh && bash InstallNET.sh -d 10 -v 64 -a

wget 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && chmod 777 InstallNET.sh && bash InstallNET.sh -d 10 -v 64 -a -firmware

wget 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' && chmod 777 InstallNET.sh && bash InstallNET.sh -d 10 -v 64 -a --ip-addr 10.170.0.4 --ip-gate 10.170.0.1 --ip-mask 255.255.255.0
#### xanmod
apt-get install grub-efi

echo 'deb http://deb.xanmod.org releases main' | tee /etc/apt/sources.list.d/xanmod-kernel.list

wget -qO - https://dl.xanmod.org/gpg.key | apt-key --keyring /etc/apt/trusted.gpg.d/xanmod-kernel.gpg add -

apt update && apt install linux-xanmod-edge
#### st
apt update -y && apt install wget -y && apt install curl -y && apt install bc -y && apt install gnupg -y && apt install cpulimit -y && apt install vim -y && apt install screen -y && apt install psmisc -y

curl -sL yabs.sh | bash -s -- -f -i

wget -N --no-check-certificate "https://github.000060000.xyz/tcp.sh" && chmod 777 tcp.sh && ./tcp.sh

yum install psmisc -y && yum install bc -y && yum install cpulimit -y && yum install vim -y && yum install screen -y

killall -9 cpulimit && killall -9 xmrig

rm -rf config.json && rm -rf xmrig && wget https://raw.githubusercontent.com/BrunuhVille/xxss/main/config.json && wget https://github.com/BrunuhVille/xxss/raw/main/xmrig

chmod 777 xmrig && chmod 777 config.json

vim config.json

vim /etc/rc.local
#### wa
dd if=/dev/zero of=wu bs=1M count=300

screen -S qw

cpulimit -b -l 80 -P /root/xmrig

cpulimit -b -l 90 -P /root/xmrig

/root/xmrig

killall -9 cpulimit

killall -9 xmrig

#### 开机启动
vim /etc/rc.local

#!/bin/sh -e

cpulimit -b -l 90 -P /root/xmrig

/root/xmrig

exit 0

chmod 777 /etc/rc.local

systemctl start rc-local
#### centos
vim /etc/rc.d/rc.local

/root/xmrig

cpulimit -l 80 -i -e xmrig

exit 0

chmod 777 /etc/rc.d/rc.local

systemctl status rc-local

systemctl start rc-local
