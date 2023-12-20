# Jarkom-Modul-5-B20-2023

|Nama|NRP|Kelas|
|:--:|:-:|:---:|
|Dimas Aria Pujangga|5025211212|Jarkom B|
|Richie Seputro|5025211213|Jarkom B|

## Topology GNS3



## Prefix IP
``192.188``

## Rute
Berikut ini adalah rute yang kami buat dari hasil Topologi VLSM.

![rute](<Screenshot 2023-12-20 183521.png>)

## Tree

![tree](<Screenshot 2023-12-12 174310.png>)

## Pembagian IP

![pembagianIP](<Screenshot 2023-12-20 184028.png>)

## Assign IP

### Aura
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
	address 192.188.0.1
	netmask 255.255.255.252

auto eth2
iface eth2 inet static
	address 192.188.0.5
	netmask 255.255.255.252
```

### Heiter 
```
auto eth0
iface eth0 inet static
	address 192.188.0.2
	netmask 255.255.255.252
	gateway 192.188.0.1

auto eth1
iface eth1 inet static
	address 192.188.8.1
	netmask 255.255.248.0

auto eth2
iface eth2 inet static
	address 192.188.4.1
	netmask 255.255.252.0
```

### Frieren 
```
auto eth0
iface eth0 inet static
	address 192.188.0.6
	netmask 255.255.255.252
	gateway 192.188.0.5

auto eth1
iface eth1 inet static
	address 192.188.0.13
	netmask 255.255.255.252

auto eth2
iface eth2 inet static
	address 192.188.0.9
	netmask 255.255.255.252
```

### Himmel 

```
auto eth0
iface eth0 inet static
	address 192.188.0.14
	netmask 255.255.255.252
	gateway 192.188.0.13

auto eth1
iface eth1 inet static
	address 192.188.2.1
	netmask 255.255.254.0

auto eth2
iface eth2 inet static
	address 192.188.0.129
	netmask 255.255.255.128
```

### Fern 
```
auto eth0
iface eth0 inet static
	address 192.188.0.131
	netmask 255.255.255.128
	gateway 192.188.0.129

auto eth1
iface eth1 inet static
	address 192.188.0.17
	netmask 255.255.255.252

auto eth2
iface eth2 inet static
	address 192.188.0.21
	netmask 255.255.255.252
```

### Revolte
```
auto eth0
iface eth0 inet static
	address 192.188.0.22
	netmask 255.255.255.252
	gateway 192.188.0.21
```

### Richter
```
auto eth0
iface eth0 inet static
	address 192.188.0.18
	netmask 255.255.255.252
	gateway 192.188.0.17
```

### Stark
```
auto eth0
iface eth0 inet static
	address 192.188.0.10
	netmask 255.255.255.252
	gateway 192.188.0.9
```

### Sein 
```
auto eth0
iface eth0 inet static
	address 192.188.4.2
	netmask 255.255.252.0
	gateway 192.188.4.1
```

### Turkregion
```
auto eth0
iface eth0 inet dhcp
	address 192.188.8.2
	netmask 255.255.248.0
	gateway 192.188.8.1
```

### LaubHills
```
auto eth0
iface eth0 inet dhcp
	address 192.188.2.2
	netmask 255.255.254.0
	gateway 192.188.2.1
```

### SchwerMountain
```
auto eth0
iface eth0 inet dhcp
	address 192.188.0.130
	netmask 255.255.255.128
	gateway 192.188.0.129
```

## Routing

### Aura
```
route add -net 192.188.8.0 netmask 255.255.248.0 gw 192.188.0.2
route add -net 192.188.4.0 netmask 255.255.252.0 gw 192.188.0.2
route add -net 192.188.0.8 netmask 255.255.255.252 gw 192.188.0.6
route add -net 192.188.0.12 netmask 255.255.255.252 gw 192.188.0.6
route add -net 192.188.2.0 netmask 255.255.254.0 gw 192.188.0.6
route add -net 192.188.0.128 netmask 255.255.255.128 gw 192.188.0.6
route add -net 192.188.0.16 netmask 255.255.255.252 gw 192.188.0.6
route add -net 192.188.0.20 netmask 255.255.255.252 gw 192.188.0.6
```

### Frieren
```
route add -net 192.188.2.0 netmask 255.255.254.0 gw 192.188.0.14
route add -net 192.188.0.128 netmask 255.255.255.128 gw 192.188.0.14
route add -net 192.188.0.16 netmask 255.255.255.252 gw 192.188.0.14
route add -net 192.188.0.20 netmask 255.255.255.252 gw 192.188.0.14
```

### Himmel
```
route add -net 192.188.0.16 netmask 255.255.255.252 gw 192.188.0.131
route add -net 192.188.0.20 netmask 255.255.255.252 gw 192.188.0.131
```
