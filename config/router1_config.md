# Router1 Configuration

## Interface Configuration

```
interface GigabitEthernet0/0
ip address 192.168.1.1 255.255.255.0
no shutdown

interface GigabitEthernet0/1
ip address 192.168.2.1 255.255.255.0
no shutdown
```

## Routing Configuration

```
ip route 192.168.1.0 255.255.255.0 GigabitEthernet0/0
ip route 192.168.2.0 255.255.255.0 GigabitEthernet0/1
```

## Save Configuration

```
write memory
```
