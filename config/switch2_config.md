# Switch2 Configuration

## VLAN Configuration

```
vlan 20
name VLAN20
```

## Interface Configuration

```
interface range FastEthernet0/1 - 3
switchport mode access
switchport access vlan 20
```

## Save Configuration

```
write memory
```
