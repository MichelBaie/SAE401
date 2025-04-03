# SAE401

### Identifiants sur les machines du projet :

ciscocisco

### Définir le hostname d’un équipement cisco

```
configure terminal
hostname MonEquipement
```

#### Configurer les interfaces réseau d’un équipement cisco

```
configure terminal
interface GigabitEthernet0/1
ip address 192.168.1.1 255.255.255.0
no shutdown
```

#### Afficher l’état des interfaces réseau d’un équipement cisco

```
show ip interface brief
show interfaces
```

#### Enregister définitivement la configuration d’un équipement Cisco

```
write memory
```

#### CIDR

```
255.255.255.252 : /30
255.255.255.0 : /24
255.255.255.248 : /29
```

#### VLANs

```
configure terminal

! Sous-interface pour le VLAN 10
interface GigabitEthernet0/1.10
 encapsulation dot1Q 10
 ip address 192.168.10.1 255.255.255.0

! Sous-interface pour le VLAN 20
interface GigabitEthernet0/1.20
 encapsulation dot1Q 20
 ip address 192.168.20.1 255.255.255.0

end

```

