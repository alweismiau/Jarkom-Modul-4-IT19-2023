# Jarkom-Modul-3-IT19-2023
## Kelompok IT19
- Fina Keiza Arismana       5027211028
- Rifqi Akhmad Maulana      502721035

# Topologi
![](https://media.discordapp.net/attachments/1025213238763327683/1181175844710924378/Screenshot_2023-12-04_170901.png?ex=65801aba&is=656da5ba&hm=1b67e15c4987f74b6e9e464994af16a7be2687c168ad82900c102d6555ee1bb8&=&format=webp&quality=lossless&width=1060&height=775)

# Rute
![image](https://github.com/alweismiau/Jarkom-Modul-4-IT19-2023/assets/112788819/21fda5ca-ad37-4167-8d19-9483439c5602)

# VLSM (Variable Length Subnet Masking)
## Pengelompokan dari VSLM
![](https://cdn.discordapp.com/attachments/1025213238763327683/1181186797129170994/Group_10.png?ex=658024ed&is=656dafed&hm=4dc5265fe8c3b040a188813be742fed50f6c49ecf0ae839cc047a58bfd7d80a7&)

## Tree
![](https://cdn.discordapp.com/attachments/1025213238763327683/1181584753376374824/WhatsApp_Image_2023-12-02_at_21.44.36_5013cef4.jpg?ex=6581978d&is=656f228d&hm=dd48ac0a257c59cc313e276caebbfc0c230bc15e12f00aa22f0e65a5ed88c802&)

## Pembagian IP
![](https://cdn.discordapp.com/attachments/1025213238763327683/1181585306013679667/image.png?ex=65819811&is=656f2311&hm=dbebb9ddd27e2d6634d72def865e3b5a4e762f019b316133659da305f555a9ba&)

## Konfigurasi Network
- Aura
```
# DHCP config for eth0
auto eth0
iface eth0 inet dhcp

# eth1 A9 Denken
auto eth1
iface eth1 inet static
    address 10.73.24.129
    netmask 255.255.255.252

# eth2 A11 Eisen
auto eth2
iface eth2 inet static
    address 10.73.24.133
    netmask 255.255.255.252

#eth3 A8 Frieren
auto eth3
iface eth3 inet static
    address 10.73.24.125
    netmask 255.255.255.252
```
- AppetitRegion & LaubHills
```
# Appetit
# Fern
auto eth0
iface eth0 inet static
	     address 10.73.0.2
	     netmask 255.255.248.0
	     gateway 10.73.0.1

# Laub
# Fern
auto eth0
iface eth0 inet static
	     address 10.73.0.3
	     netmask 255.255.248.0
	     gateway 10.73.0.1
```
- BredthRegion
```
# Lawine
auto eth0
iface eth0 inet static
	     address 10.73.24.3
	     netmask 255.255.255.192
	     gateway 10.73.24.1
```
- Denken
```
# Ke aura
auto eth0
iface eth0 inet static
    address 10.73.24.130
    netmask 255.255.255.252
    gateway 10.73.24.129

# Ke royal & wille
auto eth1
iface eth1 inet static
    address 10.73.23.1
    netmask 255.255.255.0

```
- Eisen
```
# Ke aura
auto eth0
iface eth0 inet static
    address 10.73.24.134
    netmask 255.255.255.252
    gateway 10.73.24.133

# Richter revolte
auto eth1
iface eth1 inet static
    address 10.73.24.105
    netmask 255.255.255.248
    up echo nameserver 192.168.122.1 > /etc/resolv.conf


# Linie
auto eth2
iface eth2 inet static
    address 10.73.24.145
    netmask 255.255.255.248
    up echo nameserver 192.168.122.1 > /etc/resolv.conf

# Stark
auto eth3
iface eth3 inet static
    address 10.73.24.137
    netmask 255.255.255.252
    up echo nameserver 192.168.122.1 > /etc/resolv.conf

# Lugner
auto eth4
iface eth4 inet static
    address 10.73.24.141
    netmask 255.255.255.252
    up echo nameserver 192.168.122.1 > /etc/resolv.conf

```
- Fern
```
# Flamme
auto eth0
iface eth0 inet static
    address 10.73.24.118
    netmask 255.255.255.252
    gateway 10.73.24.117

# Appet Laub
auto eth1
iface eth1 inet static
    address 10.73.0.1
    netmask 255.255.248.0
```
- Flamme
```
# Frieren
auto eth0
iface eth0 inet static
    address 10.73.24.122
    netmask 255.255.255.252
    gateway 10.73.24.121

# Himmel
auto eth1
iface eth1 inet static
    address 10.73.24.113
    netmask 255.255.255.252

# Rohr
auto eth2
iface eth2 inet static
    address 10.73.8.1
    netmask 255.255.252.0

# Fern
auto eth3
iface eth3 inet static
    address 10.73.24.117
    netmask 255.255.255.252
```
- Frieren
```
# Aura
auto eth0
iface eth0 inet static
    address 10.73.24.126
    netmask 255.255.255.252
    gateway 10.73.24.125

# Flamme
auto eth1
iface eth1 inet static
    address 10.73.24.121
    netmask 255.255.255.252

# Lake
auto eth2
iface eth2 inet static
    address 10.73.24.65
    netmask 255.255.255.224
```
- Granzchannel
```
# Linie
auto eth0
iface eth0 inet static
	     address 10.73.20.2
	     netmask 255.255.254.0
	     gateway 10.73.20.1

```
- Heiter
```
# Lawine
auto eth0
iface eth0 inet static
	     address 10.73.24.2
	     netmask 255.255.255.192
	     gateway 10.73.24.1

# Sein - Riegel
auto eth1
iface eth1 inet static
	     address 10.73.16.1
	     netmask 255.255.252.0
```
- Himmel
```
# Flamme
auto eth0
iface eth0 inet static
    address 10.73.24.114
    netmask 255.255.255.252
    gateway 10.73.24.113

# Schwer
auto eth1
iface eth1 inet static
    address 10.73.24.97
    netmask 255.255.255.248
```
- LakeKorridor
```
# Frieren
auto eth0
iface eth0 inet static
    address 10.73.24.66
    netmask 255.255.255.224
    gateway 10.73.24.65
```
- Lawine
```
# Linie
auto eth0
iface eth0 inet static
	     address 10.73.24.150
	     netmask 255.255.255.252
	     gateway 10.73.24.149

# Bredth
auto eth1
iface eth1 inet static
	     address 10.73.24.1
	     netmask 255.255.255.192
```
- Linie
```
# Ke Eisen
auto eth0
iface eth0 inet static
    address 10.73.24.146
    netmask 255.255.255.252
    gateway 10.73.24.145

# Lawine
auto eth1
iface eth1 inet static
    address 10.73.24.149
    netmask 255.255.255.252
    up echo nameserver 192.168.122.1 > /etc/resolv.conf

# Granz
auto eth2
iface eth2 inet static
    address 10.73.20.1
    netmask 255.255.254.0
    up echo nameserver 192.168.122.1 > /etc/resolv.conf

```
- Lugner
```
# Ke Eisen
auto eth0
iface eth0 inet static
    address 10.73.24.142
    netmask 255.255.255.252
    gateway 10.73.24.141

# Grobe
auto eth1
iface eth1 inet static
    address 10.73.22.1
    netmask 255.255.255.0
    up echo nameserver 192.168.122.1 > /etc/resolv.conf

# Turk
auto eth2
iface eth2 inet static
    address 10.73.12.1
    netmask 255.255.252.0
    up echo nameserver 192.168.122.1 > /etc/resolv.conf

```
- Richter & Revolte
```
# Richter
# Eisen
auto eth0
iface eth0 inet static
	     address 10.73.24.106
	     netmask 255.255.255.248
	     gateway 10.73.24.105

# Revolte
# Eisen
auto eth0
iface eth0 inet static
	     address 10.73.24.107
	     netmask 255.255.255.248
	     gateway 10.73.24.105
```
- Rohr
```
# Flamme
auto eth0
iface eth0 inet static
    address 10.73.8.2
    netmask 255.255.252.0
    gateway 10.73.8.1
```
- RoyalCapital & WilleRegion
```
# Royal
# Denken
auto eth0
iface eth0 inet static
	     address 10.73.23.2
	     netmask 255.255.255.0
	     gateway 10.73.23.1

# Wille 
# Denken
auto eth0
iface eth0 inet static
	     address 10.73.23.3
	     netmask 255.255.255.0
	     gateway 10.73.23.1

```
- SchwerMountains
```
# Himmel
auto eth0
iface eth0 inet static
	     address 10.73.24.98
	     netmask 255.255.252.248
         gateway 10.73.24.97
```
- Sein & Riegel
```
# Sein
# heiter
auto eth0
iface eth0 inet static
	     address 10.73.16.2
	     netmask 255.255.252.0
         gateway 10.73.16.1

# Riegel
# heiter
auto eth0
iface eth0 inet static
	     address 10.73.16.3
	     netmask 255.255.252.0
         gateway 10.73.16.1
```
- Stark
```
# Eisen
auto eth0
iface eth0 inet static
	     address 10.73.24.138
	     netmask 255.255.255.252
	     gateway 10.73.24.137
```
- Turk & Grobe
```
# Grobe
# Lugner
auto eth0
iface eth0 inet static
	     address 10.73.22.2
	     netmask 255.255.255.0
	     gateway 10.73.22.1

# Turk 
# Lugner
auto eth0
iface eth0 inet static
	     address 10.73.12.2
	     netmask 255.255.255.0
	     gateway 10.73.12.1
```

##  Routing
- Aura
```
iptables

# Denken
route add -net 10.73.24.128 netmask 255.255.255.252 gw 10.73.24.130
# Eisen
route add -net 10.73.24.132 netmask 255.255.255.252 gw 10.73.24.134
# Frieren
route add -net 10.73.24.124 netmask 255.255.255.252 gw 10.73.24.125

# Denken - client 
route add -net 10.73.23.0 netmask 255.255.255.0 gw 10.73.24.130

# Eisen - Richter -Revolte
route add -net 10.73.24.104 netmask 255.255.255.248 gw 10.73.24.134

# Eisen - Stark
route add -net 10.73.24.136 netmask 255.255.255.252 gw 10.73.24.134

# Eisen - Lugner - Turk
route add -net 10.73.12.0 netmask 255.255.255.252 gw 10.73.24.134

# Eisen - Lugner - Grobe
route add -net 10.73.22.0 netmask 255.255.255.252 gw 10.73.24.134

# Eisen - Linie - Granz
route add -net 10.73.20.0 netmask 255.255.254.0 gw 10.73.24.134

# Eisen - Linie - Lawin - Bredth
route add -net 10.73.24.0 netmask 255.255.255.192 gw 10.73.24.134

# Eisen - Linie - Lawin - Heiter - Sein - Riegel
route add -net 10.73.16.0 netmask 255.255.252.0 gw 10.73.24.134

# Frieren - Lake 
route add -net 10.73.24.64 netmask 255.255.255.224 gw 10.73.24.126

# Frieren - Flamme - Himmel - Schwer
route add -net 10.73.24.96 netmask 255.255.255.248 gw 10.73.24.126

# Frieren - Flamme - Rohr
route add -net 10.73.8.0 netmask 255.255.252.0 gw 10.73.24.126

# Frieren - Flamme - Fern - Ap - Laub
route add -net 10.73.0.0 netmask 255.255.248.0 gw 10.73.24.126

```
- Denken
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.129
```
- Eisen
```

# Aura
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.133

# Lugner - Turk
route add -net 10.73.12.0 netmask 255.255.252.0 gw 10.73.24.142

# Lugner - Grobe
route add -net 10.73.22.0 netmask 255.255.255.0 gw 10.73.24.142

# Linie - Granz
route add -net 10.73.20.0 netmask 255.255.254.0 gw 10.73.24.146

# Linie - Lawin - Bredth
route add -net 10.73.24.0 netmask 255.255.255.192 gw 10.73.24.146

# Linie - Lawin - Heiter - Sein - Riegel
route add -net 10.73.16.0 netmask 255.255.252.0 gw 10.73.24.146
```
- Fern
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.117
```
- Flamme
```
# Himmel - Schwer
route add -net 10.73.24.96 netmask 255.255.255.248 gw 10.73.24.114

# Rohr
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.121

# Fern - Ap - Laub
route add -net 10.73.0.0 netmask 255.255.248.0 gw 10.73.24.118
```
- Frieren
```
# Lake
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.125

# Flamme - Himmel - Schwer
route add -net 10.73.24.96 netmask 255.255.255.248 gw 10.73.24.122

# Rohr
route add -net 10.73.8.0 netmask 255.255.252.0 gw 10.73.24.122

# Flamme - Fern - Ap - Laub
route add -net 10.73.0.0 netmask 255.255.248.0 gw 10.73.24.122
```
- Heiter
```
# Aura - Lawine
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.1
```
- Himmel
```
# Flamme
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.113
```
- Lawine
```
# Aura - Linie
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.149

# Sein - Riegel
route add -net 10.73.16.0 netmask 255.255.252.0 gw 10.73.24.150
```
- Linie
```
# Aura - Eisen - Granz
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.145

# Bredth
route add -net 10.73.24.0 netmask 255.255.255.192 gw 10.73.24.150

# Lawine - Heiter - Sein - Riegel
route add -net 10.73.16.0 netmask 255.255.252.0 gw 10.73.24.2
```
- Lugner
```
# Eisen
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.73.24.141
```

## Result
- Ping Aura -> Denken
![](https://cdn.discordapp.com/attachments/1025213238763327683/1181588652778860595/WhatsApp_Image_2023-12-04_at_18.25.56_524679d6.jpg?ex=65819b2f&is=656f262f&hm=a7c1682752eef034dcaa74e1420201775ab3642f99e9a67992e64d7887fa76d0&)
- Ping Eisen -> Revolte
![](https://cdn.discordapp.com/attachments/1025213238763327683/1181588951811756145/WhatsApp_Image_2023-12-04_at_18.26.21_8905bef6.jpg?ex=65819b76&is=656f2676&hm=3cb8fcf683b09ce1ca539e4114fd7aee2d24987ab13a1d5d890de0592483b2ab&)
- Ping Himmel -> SchwerMountains
![](https://cdn.discordapp.com/attachments/1025213238763327683/1181588983621369916/WhatsApp_Image_2023-12-04_at_18.26.44_e75a1f9b.jpg?ex=65819b7e&is=656f267e&hm=347a3e440fa5cf3af250a5951a681732bc4ba7dfd6d6240f80d6466517506d2d&)

# CIDR (Classless Inter Domain Routing)

## Pengelompokan dari CIDR
![image](https://github.com/alweismiau/Jarkom-Modul-4-IT19-2023/assets/112788819/0544e13b-3881-4f7f-97fa-d0729b9bcac9)

## Tree
![image](https://github.com/alweismiau/Jarkom-Modul-4-IT19-2023/assets/112788819/d3b929d6-b356-4aee-a2ca-3e10fa856528)


## Penggabungan Subnet

Berikut adalah proses penggabungan subnet bertahap yang dilakukan. Adapun untuk tingkatan yang digunakan adalah dari abjad A-J

![image](https://github.com/alweismiau/Jarkom-Modul-4-IT19-2023/assets/112788819/9e9569ad-c723-4afa-b5d9-a7aab9a4f01d)

![image](https://github.com/alweismiau/Jarkom-Modul-4-IT19-2023/assets/112788819/eb638c58-ed58-4630-962f-89f5ff8e5608)


# Kendala

Tidak ada kendala yang dialami selama pengerjaan
