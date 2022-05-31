# Домашнее задание к занятию "3.8. Компьютерные сети, лекция 3" - yakovlev_vs
#### 1. Подключитесь к публичному маршрутизатору в интернет. Найдите маршрут к вашему публичному IP
```bash
telnet route-views.routeviews.org
Username: rviews
show ip route x.x.x.x/32
show bgp x.x.x.x/32
```
Решение 

route
```bash
User Access Verification

Username: rviews
route-views>show ip route 178.176.79.49
Routing entry for 178.176.72.0/21
  Known via "bgp 6447", distance 20, metric 0
  Tag 3303, type external
  Last update from 217.192.89.50 1w4d ago
  Routing Descriptor Blocks:
  * 217.192.89.50, from 217.192.89.50, 1w4d ago
      Route metric is 0, traffic share count is 1
      AS Hops 3
      Route tag 3303
      MPLS label: none
```
bgp
```bash
route-views>show bgp 178.176.79.46
BGP routing table entry for 178.176.72.0/21, version 2297448096
Paths: (24 available, best #20, table default)
  Not advertised to any peer
  Refresh Epoch 1
  8283 8455 31133 25159, (aggregated by 25159 10.205.141.129)
    94.142.247.3 from 94.142.247.3 (94.142.247.3)
      Origin IGP, metric 0, localpref 100, valid, external
      Community: 8283:11 8455:1030 8455:1114 8455:1115 8455:1666 8455:3001
      unknown transitive attribute: flag 0xE0 type 0x20 length 0xC
        value 0000 205B 0000 0006 0000 000B
      path 7FE10A75B8D0 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  53767 174 31133 25159, (aggregated by 25159 10.205.141.129)
    162.251.163.2 from 162.251.163.2 (162.251.162.3)
      Origin IGP, localpref 100, valid, external
      Community: 174:21101 174:22028 53767:5000
      path 7FE05102F6B8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  3549 3356 174 31133 25159, (aggregated by 25159 10.205.141.129)
    208.51.134.254 from 208.51.134.254 (67.16.168.191)
      Origin IGP, metric 0, localpref 100, valid, external
      Community: 3356:3 3356:22 3356:86 3356:575 3356:666 3356:903 3356:2011 3549:2581 3549:30840
      path 7FE0A96486D0 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  19214 174 31133 25159, (aggregated by 25159 10.205.141.129)
    208.74.64.40 from 208.74.64.40 (208.74.64.40)
      Origin IGP, localpref 100, valid, external
      Community: 174:21101 174:22028
      path 7FE17DF8AE88 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  701 174 31133 25159, (aggregated by 25159 10.205.141.129)
    137.39.3.55 from 137.39.3.55 (137.39.3.55)
      Origin IGP, localpref 100, valid, external
      path 7FE0BA8C8FA8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  3356 174 31133 25159, (aggregated by 25159 10.205.141.129)
    4.68.4.46 from 4.68.4.46 (4.69.184.201)
      Origin IGP, metric 0, localpref 100, valid, external
      Community: 3356:3 3356:22 3356:86 3356:575 3356:666 3356:903 3356:2012
      path 7FE185728DA8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  3561 209 3356 174 31133 25159, (aggregated by 25159 10.205.141.129)
    206.24.210.80 from 206.24.210.80 (206.24.210.80)
      Origin IGP, localpref 100, valid, external
      path 7FE0C8CFB9B0 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  57866 6830 174 31133 25159, (aggregated by 25159 10.205.141.129)
    37.139.139.17 from 37.139.139.17 (37.139.139.17)
      Origin IGP, metric 0, localpref 100, valid, external
      Community: 6830:17000 6830:17504 6830:33125 57866:501
      path 7FE154813B58 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  7018 174 31133 25159, (aggregated by 25159 10.205.141.129)
    12.0.1.63 from 12.0.1.63 (12.0.1.63)
      Origin IGP, localpref 100, valid, external
      Community: 7018:5000 7018:37232
      path 7FE105D94318 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  4901 6079 31133 25159, (aggregated by 25159 10.205.141.129)
    162.250.137.254 from 162.250.137.254 (162.250.137.254)
      Origin IGP, localpref 100, valid, external
      Community: 65000:10100 65000:10300 65000:10400
      path 7FE12EA726C8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  6939 31133 25159, (aggregated by 25159 10.205.141.129)
    64.71.137.241 from 64.71.137.241 (216.218.252.164)
      Origin IGP, localpref 100, valid, external
      path 7FE15A28B578 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  20912 3257 174 31133 25159, (aggregated by 25159 10.205.141.129)
    212.66.96.126 from 212.66.96.126 (212.66.96.126)
      Origin IGP, localpref 100, valid, external
      Community: 3257:8070 3257:30155 3257:50001 3257:53900 3257:53902 20912:65004
      path 7FE008FEFC58 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  3267 31133 25159, (aggregated by 25159 10.205.141.129)
    194.85.40.15 from 194.85.40.15 (185.141.126.1)
      Origin IGP, metric 0, localpref 100, valid, external
      path 7FE1491AEAD8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  3333 1103 31133 25159, (aggregated by 25159 10.205.141.129)
    193.0.0.56 from 193.0.0.56 (193.0.0.56)
      Origin IGP, localpref 100, valid, external
      path 7FE1501A5FB0 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  20130 6939 31133 25159, (aggregated by 25159 10.205.141.129)
    140.192.8.16 from 140.192.8.16 (140.192.8.16)
      Origin IGP, localpref 100, valid, external
      path 7FE0A87D0BA8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  3257 174 31133 25159, (aggregated by 25159 10.205.141.129)
    89.149.178.10 from 89.149.178.10 (213.200.83.26)
      Origin IGP, metric 10, localpref 100, valid, external
      Community: 3257:8059 3257:30153 3257:50001 3257:54900 3257:54901
      path 7FE106A34EC8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  101 174 31133 25159, (aggregated by 25159 10.205.141.129)
    209.124.176.223 from 209.124.176.223 (209.124.176.223)
      Origin IGP, localpref 100, valid, external
      Community: 101:20100 101:20110 101:22100 174:21101 174:22028
      Extended Community: RT:101:22100
      path 7FE1220DC8B0 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  852 31133 25159, (aggregated by 25159 10.205.141.129)
    154.11.12.212 from 154.11.12.212 (96.1.209.43)
      Origin IGP, metric 0, localpref 100, valid, external
      path 7FE18ADCA428 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  1351 6939 31133 25159, (aggregated by 25159 10.205.141.129)
    132.198.255.253 from 132.198.255.253 (132.198.255.253)
      Origin IGP, localpref 100, valid, external
      path 7FE04A369B88 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  3303 31133 25159, (aggregated by 25159 10.205.141.129)
    217.192.89.50 from 217.192.89.50 (138.187.128.158)
      Origin IGP, localpref 100, valid, external, best
      Community: 3303:1004 3303:1006 3303:1030 3303:3056
      path 7FE0C51A3200 RPKI State not found
      rx pathid: 0, tx pathid: 0x0
  Refresh Epoch 2
  2497 174 31133 25159, (aggregated by 25159 10.205.141.129)
    202.232.0.2 from 202.232.0.2 (58.138.96.254)
      Origin IGP, localpref 100, valid, external
      path 7FE118D8A0F8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  1221 4637 31133 25159, (aggregated by 25159 10.205.141.129)
    203.62.252.83 from 203.62.252.83 (203.62.252.83)
      Origin IGP, localpref 100, valid, external
      path 7FE01C2B5610 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  49788 12552 31133 25159, (aggregated by 25159 10.205.141.129)
    91.218.184.60 from 91.218.184.60 (91.218.184.60)
      Origin IGP, localpref 100, valid, external
      Community: 12552:12000 12552:12100 12552:12101 12552:22000
      Extended Community: 0x43:100:1
      path 7FE0F14CB2E8 RPKI State not found
      rx pathid: 0, tx pathid: 0
  Refresh Epoch 1
  7660 2516 174 31133 25159, (aggregated by 25159 10.205.141.129)
    203.181.248.168 from 203.181.248.168 (203.181.248.168)
      Origin IGP, localpref 100, valid, external
      Community: 2516:1030 7660:9003
      path 7FE0F14CFB68 RPKI State not found
      rx pathid: 0, tx pathid: 0
```
#### 2. Создайте dummy0 интерфейс в Ubuntu. Добавьте несколько статических маршрутов. Проверьте таблицу маршрутизации.
Решение 

создание интерфейса
```bash
root@vagrant:~# ip link add dummy0 type dummy
root@vagrant:~# ip addr add 192.168.1.66/24 dev dummy0
root@vagrant:~# ip link set dummy0 up
root@vagrant:~# ip addr
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    link/ether 08:00:27:b1:28:5d brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.36/24 brd 192.168.1.255 scope global dynamic eth0
       valid_lft 41611sec preferred_lft 41611sec
    inet6 fe80::a00:27ff:feb1:285d/64 scope link
       valid_lft forever preferred_lft forever
3: dummy0: <BROADCAST,NOARP,UP,LOWER_UP> mtu 1500 qdisc noqueue state UNKNOWN group default qlen 1000
    link/ether ea:b1:56:d9:62:ae brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.66/24 scope global dummy0
       valid_lft forever preferred_lft forever
    inet6 fe80::e8b1:56ff:fed9:62ae/64 scope link
       valid_lft forever preferred_lft forever
root@vagrant:~# ping 192.168.1.66
PING 192.168.1.66 (192.168.1.66) 56(84) bytes of data.
64 bytes from 192.168.1.66: icmp_seq=1 ttl=64 time=0.048 ms
64 bytes from 192.168.1.66: icmp_seq=2 ttl=64 time=0.026 ms
64 bytes from 192.168.1.66: icmp_seq=3 ttl=64 time=0.026 ms
64 bytes from 192.168.1.66: icmp_seq=4 ttl=64 time=0.026 ms
```
добавление маршрутов
```bash
root@vagrant:~# ip route add 10.10.8.0/24 via 192.168.1.3
root@vagrant:~# ip route add 10.10.28.0/24 via 192.168.1.66
root@vagrant:~# ip route
default via 192.168.1.3 dev eth0 proto dhcp src 192.168.1.36 metric 100
10.10.8.0/24 via 192.168.1.3 dev eth0
10.10.28.0/24 via 192.168.1.66 dev dummy0
192.168.1.0/24 dev eth0 proto kernel scope link src 192.168.1.36
192.168.1.0/24 dev dummy0 proto kernel scope link src 192.168.1.66
192.168.1.3 dev eth0 proto dhcp scope link src 192.168.1.36 metric 100
```

#### 3. Проверьте открытые TCP порты в Ubuntu, какие протоколы и приложения используют эти порты? Приведите несколько примеров.

Решение 

```bash
root@vagrant:~# ss -tpan
State        Recv-Q       Send-Q             Local Address:Port             Peer Address:Port       Process
LISTEN       0            4096               127.0.0.53%lo:53                    0.0.0.0:*           users:(("systemd-resolve",pid=671,fd=13))
LISTEN       0            128                      0.0.0.0:22                    0.0.0.0:*           users:(("sshd",pid=779,fd=3))
ESTAB        0            0                   192.168.1.36:22               192.168.1.76:32634       users:(("sshd",pid=2045,fd=4))
ESTAB        0            0                   192.168.1.36:22               192.168.1.76:32633       users:(("sshd",pid=2043,fd=4))
LISTEN       0            128                         [::]:22                       [::]:*           users:(("sshd",pid=779,fd=4))
```
```bash
root@vagrant:~# apt-get install net-tools
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following NEW packages will be installed:
  net-tools
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 196 kB of archives.
After this operation, 864 kB of additional disk space will be used.
Get:1 http://us.archive.ubuntu.com/ubuntu focal/main amd64 net-tools amd64 1.60+git20180626.aebd88e-1ubuntu1 [196 kB]
Fetched 196 kB in 1s (202 kB/s)
Selecting previously unselected package net-tools.
(Reading database ... 40620 files and directories currently installed.)
Preparing to unpack .../net-tools_1.60+git20180626.aebd88e-1ubuntu1_amd64.deb ...
Unpacking net-tools (1.60+git20180626.aebd88e-1ubuntu1) ...
Setting up net-tools (1.60+git20180626.aebd88e-1ubuntu1) ...
Processing triggers for man-db (2.9.1-1) ...
root@vagrant:~# netstat -tulpn
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name
tcp        0      0 127.0.0.53:53           0.0.0.0:*               LISTEN      671/systemd-resolve
tcp        0      0 0.0.0.0:22              0.0.0.0:*               LISTEN      779/sshd: /usr/sbin
tcp6       0      0 :::22                   :::*                    LISTEN      779/sshd: /usr/sbin
udp        0      0 127.0.0.53:53           0.0.0.0:*                           671/systemd-resolve
udp        0      0 192.168.1.36:68         0.0.0.0:*                           669/systemd-network
```
- 22 port - TCP,UDP - под SSH соединение, Sshd (OpenSSH Daemon) — программа демон для ssh. sshd ожидает подключений от клиентов.
- 53 port - TCP,UDP - под DNS, Systemd-resolved — это сервис systemd для локального резолвинга DNS запросов.
- 68 port - UDP - DHCP (англ. Dynamic Host Configuration Protocol — протокол динамической настройки узла). Получение сетевой конфигурации

#### 4. Проверьте используемые UDP сокеты в Ubuntu, какие протоколы и приложения используют эти порты?

Решение

```bash
root@vagrant:~# ss -upan
State       Recv-Q      Send-Q                Local Address:Port             Peer Address:Port      Process
UNCONN      0           0                     127.0.0.53%lo:53                    0.0.0.0:*          users:(("systemd-resolve",pid=671,fd=12))
UNCONN      0           0                 192.168.1.36%eth0:68                    0.0.0.0:*          users:(("systemd-network",pid=669,fd=19))
```

#### 5. Используя diagrams.net, создайте L3 диаграмму вашей домашней сети или любой другой сети, с которой вы работали.

Решение

![](picture/HomeNet.png)

### Нет времени делать дополнительные задания (*) из-за высокой загруженности на работе. Но вот нашел рабочий пример. 

#### 6*. Установите Nginx, настройте в режиме балансировщика TCP или UDP.

Создаем 4 VM (1-ый - клиент, 2-ой - балансировщик, 3-ий и 4-ый - веб-серверы)

vagrantfile
```shell
boxes = {
  'netology1' => '10',
  'netology2' => '60',
  'netology3' => '90',
  'netology4' => '120'
}

Vagrant.configure("2") do |config|
  config.vm.network "private_network", virtualbox__intnet: true, auto_config: false
  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
    v.cpus = 1
  end
  config.vm.box = "bento/ubuntu-20.04"

  boxes.each do |k, v|
    config.vm.define k do |node|
      node.vm.provision "shell" do |s|
        s.inline = "hostname $1;"\
          "ip addr add $2 dev eth1;"\
          "ip link set dev eth1 up;"\
          "apt -y update;"\
          "apt -y install nginx;"\
          "mkdir -p /data/www;"\
          "echo Hello from $1 >> /data/www/index.html;"
        s.args = [k, "172.28.128.#{v}/24"]
      end
    end
  end
end
```
На балансировщике (VM2) добавляем конфиг
```shell
$ sudo nano /etc/nginx/conf.d/proxyTCP.conf
     upstream backend1 {
         server 172.28.128.90:8080;
         server 172.28.128.120:8080;
     }
     server {
         listen 8080;
         location / {
             proxy_pass http://backend1;
         }
     }

$ sudo nginx -s reload
```
На веб-серверах (VM3, VM4) меняем конфиги
```shell
$ sudo nano /etc/nginx/sites-enabled/default
server {
     listen 8080;
     location / {
             root /data/www;
             index  index.html index.htm;
     }
}

$ sudo nginx -s reload
```
Отдаем запрос с VM1
```shell
$ curl 172.28.128.60:8080
Hello from netology3
$ curl 172.28.128.60:8080
Hello from netology4
$ curl 172.28.128.60:8080
Hello from netology3
$ curl 172.28.128.60:8080
Hello from netology4
```

#### 7*. Установите bird2, настройте динамический протокол маршрутизации RIP.

#### 8*. Установите Netbox, создайте несколько IP префиксов, используя curl проверьте работу API.

Установка docker
```shell
# curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
# echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
# sudo apt-get update
# sudo apt-get install docker-ce docker-ce-cli containerd.io
# apt install docker-compose
```
Запуск Netbox
```shell
# git clone -b release https://github.com/netbox-community/netbox-docker.git
# cd netbox-docker
# tee docker-compose.override.yml <<EOF
version: '3.4'
services:
  netbox:
    ports:
      - 8000:8080
EOF
# docker-compose pull
# docker-compose up
```
Запрос на создание префикса через `curl`
```shell
$ sudo curl -ss -X POST -H "Authorization: Token 0123456789abcdef0123456789abcdef01234567" -H "Content-Type: application/json" -H "Accept: application/json; indent=4" http://10.0.2.15:8000/api/ipam/prefixes/ --data '{"prefix": "10.0.8.0/24"}'
{
    "id": 8,
    "url": "http://10.0.2.15:8000/api/ipam/prefixes/8/",
    "display": "10.0.8.0/24",
    "family": {
        "value": 4,
        "label": "IPv4"
    },
    "prefix": "10.0.8.0/24",
    "site": null,
    "vrf": null,
    "tenant": null,
    "vlan": null,
    "status": {
        "value": "active",
        "label": "Active"
    },
    "role": null,
    "is_pool": false,
    "mark_utilized": false,
    "description": "",
    "tags": [],
    "custom_fields": {},
    "created": "2021-12-02",
    "last_updated": "2021-12-02T15:03:45.193570Z",
    "children": 0,
    "_depth": 0
}
```
![](picture/netbox.png)