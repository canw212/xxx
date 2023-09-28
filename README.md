# xxx
x-ui面板
bash <(curl -Ls https://raw.githubusercontent.com/vaxilu/x-ui/master/install.sh)

是否支持GPT
bash <(curl -Ls https://cdn.jsdelivr.net/gh/missuo/OpenAI-Checker/openai.sh)

CPU型号
cat /proc/cpuinfo

docker钱
curl -fsSL https://get.docker.com | bash
AMD钱
docker run -d --restart=always --name tm traffmonetizer/cli_v2 start accept --token wfMV1JZDNmE7QQNNfzRh/2PYSbSRZnx3Geqektdz9L4=
ARM钱
docker run -d --restart always --name tm traffmonetizer/cli_v2:arm64v8 start accept --token wfMV1JZDNmE7QQNNfzRh/2PYSbSRZnx3Geqektdz9L4= 

Ubuntu更新纯净版
apt update -y && apt full-upgrade -y && apt autoremove -y && apt autoclean -y

BBR
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh

清理垃圾
sudo apt autoremove --purge -y

sudo apt clean -y

sudo apt autoclean -y

sudo apt remove --purge $(dpkg -l | awk '/^rc/ {print $2}') -y

sudo journalctl --rotate

sudo journalctl --vacuum-time=1s

sudo journalctl --vacuum-size=50M

sudo apt remove --purge $(dpkg -l | awk '/^ii linux-(image|headers)-[^ ]+/{print $2}' | grep -v $(uname -r | sed 's/-.*//') | xargs) -y

