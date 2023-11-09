---
date: 2023-11-09
tags:
  - Hardware
---
Les commandes de configuration IP peuvent varier légèrement entre les systèmes d'exploitation. Voici les commandes couramment utilisées pour configurer l'adresse IP sur Windows et Linux.

## Windows

### Afficher la Configuration IP :
```bash
ipconfig
```

### Renouveler l'Adresse IP (DHCP) :
```bash
ipconfig /renew
```

### Libérer l'Adresse IP (DHCP) :
```bash
ipconfig /release
```

### Changer l'Adresse IP Manuellement :
```bash
netsh interface ipv4 set address "NomInterface" static AdresseIP Masque Passerelle
```

### Changer les Serveurs DNS Manuellement :
```bash
netsh interface ipv4 set dns "NomInterface" static ServeurDNS
```

## Linux

### Afficher la Configuration IP :
```bash
ifconfig
```
ou
```bash
ip addr show
```

### Renouveler l'Adresse IP (DHCP) :
```bash
dhclient
```

### Libérer l'Adresse IP (DHCP) :
```bash
dhclient -r
```

### Changer l'Adresse IP Manuellement :
```bash
sudo ifconfig interface new_ip_address netmask new_subnet_mask
```
ou
```bash
sudo ip addr add new_ip_address/mask_bits dev interface
```

### Changer les Serveurs DNS Manuellement :
Modifier le fichier `/etc/resolv.conf` :
```bash
sudo nano /etc/resolv.conf
```
Ajoutez ou modifiez les lignes :
```bash
nameserver DNS_server_IP
```
