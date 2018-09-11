## installation script
[![build](https://github.com/SuzukazeAoran/SVG/blob/master/build%20passing.svg)](https://github.com/nanqinlang-shadowsocksr/shadowsocksr-python)
[![language](https://github.com/SuzukazeAoran/SVG/blob/master/language-python-blue.svg)](https://github.com/nanqinlang-shadowsocksr/shadowsocksr-python)
[![author](https://github.com/SuzukazeAoran/SVG/blob/master/author-nanqinlang-lightgrey.svg)](https://github.com/nanqinlang-shadowsocksr/shadowsocksr-python)

powered by nanqinlang and editd by tm at 20180911 

`#wget -N --no-check-certificate https://github.com/nanqinlang/shadowsocksr/releases/download/2.1/ssr_setup_2.1.sh && chmod +x ssr_setup_2.1.sh && bash ssr_setup_2.1.sh install`

then,your can find your user-passwd config in user-config.json,which you can edit it by yourself

if you want to add user for your server,you can edit user-config.json like this:
```
{
    "server": "0.0.0.0",
    "server_ipv6": "::",
    "local_address": "127.0.0.1",
    "local_port": 1080,
    "port_password": {
                    "10000": "password10000",
                    "10001": "password10001"
                    },
    "method": "rc4-md5",
    "protocol": "origin",
    "protocol_param": "",
    "obfs": "plain",
    "obfs_param": "",
    "speed_limit_per_con": 0,
    "speed_limit_per_user": 0,

    "additional_ports" : {}, // only works under multi-user mode
    "additional_ports_only" : false, // only works under multi-user mode
    "timeout": 120,
    "udp_timeout": 60,
    "dns_ipv6": false,
    "connect_verbose_info": 0,
    "redirect": "",
    "fast_open": true
}
```
wiki：https://github.com/tm2018/shell/blob/master/shadowsockr-shell/ssr-setup.sh

releases：https://github.com/nanqinlang/shadowsocksr/releases

#help:

all your files for ssr is in dir /home/shadowsocks,you can select to remain here or move to other dirs

you can do like this:
```
start project 
#cd /home/shadowsocks && chmod +x *.sh && ./run.sh

stop project
#cd /home/shadowsocks && ./stop.sh
```
