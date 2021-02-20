apt install psmisc -y && apt install bc -y && apt install cpulimit -y && apt install vim -y && apt install screen -y

wget https://raw.githubusercontent.com/BrunuhVille/xxss/main/config.json && wget https://github.com/BrunuhVille/xxss/raw/main/xmrig

chmod 777 xmrig && chmod 777 config.json

vim config.json

dd if=/dev/zero of=wu bs=1M count=300

screen -S qw

cpulimit -b -l 80 -P /root/xmrig

cpulimit -b -l 90 -P /root/xmrig

/root/xmrig

killall -9 cpulimit
