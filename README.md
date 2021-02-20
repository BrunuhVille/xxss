apt update -y && apt install curl -y && apt install psmisc -y && apt install bc -y && apt install cpulimit -y && apt install vim -y && apt install screen -y

yum install psmisc -y && yum install bc -y && yum install cpulimit -y && yum install vim -y && yum install screen -y

wget https://raw.githubusercontent.com/BrunuhVille/xxss/main/config.json && wget https://github.com/BrunuhVille/xxss/raw/main/xmrig

chmod 777 xmrig && chmod 777 config.json

vim config.json

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
