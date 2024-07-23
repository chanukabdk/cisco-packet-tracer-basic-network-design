# Switch1 Configuration

## VLAN Configuration

```
vlan 10
name VLAN10
```

## Interface Configuration

```
interface range FastEthernet0/1 - 3
switchport mode access
switchport access vlan 10
```

## Save Configuration

```
write memory
```
