# scAuto
#update & upgrade
apt update && apt upgrade -y

#install
sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && bzip2 gzip coreutils curl && wget https://raw.githubusercontent.com/rioxy/scAuto/main/setup.sh && chmod +x setup.sh && sed -i -e 's/\r$//' setup.sh && ./setup.sh
