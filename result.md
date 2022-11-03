## Scenario 1

- [x] N02 - OT
- [x] N02 - CRDT-CS
- [x] N02 - CRDT-P2P
- [x] N04 - OT
- [x] N04 - CRDT-CS
- [x] N04 - CRDT-P2P
- [x] N08 - OT
- [x] N08 - CRDT-CS
- [x] N08 - CRDT-P2P

## Scenario 2

- [x] N02 - OT
- [x] N02 - CRDT-CS
- [x] N02 - CRDT-P2P
- [x] N04 - OT
- [x] N04 - CRDT-CS
- [x] N04 - CRDT-P2P
- [x] N08 - OT
- [x] N08 - CRDT-CS
- [x] N08 - CRDT-P2P

## Scenario 3

- [ ] N02 - OT
- [x] N02 - CRDT-CS
- [x] N02 - CRDT-P2P
- [ ] N04 - OT
- [x] N04 - CRDT-CS
- [x] N04 - CRDT-P2P
- [ ] N08 - OT
- [x] N08 - CRDT-CS
- [x] N08 - CRDT-P2P

## Scenario 4

- [ ] N02 - OT
- [ ] N02 - CRDT-CS
- [ ] N02 - CRDT-P2P
- [ ] N04 - OT
- [ ] N04 - CRDT-CS
- [ ] N04 - CRDT-P2P
- [ ] N08 - OT
- [ ] N08 - CRDT-CS
- [ ] N08 - CRDT-P2P

```
1667402386

peer-1: 34.101.227.234
peer-2: 34.101.56.179

crdt-p2p: 35.247.146.237
ot-ws: 34.142.229.79
crdt-ws: 34.143.155.91

netd 34.128.119.200 1667492280 peer-1
netd 34.101.227.234 1667492280 peer-2
netd 34.142.229.79 1667492280 ot-ws

scpd 34.128.119.200 peer-1
scpd 34.101.227.234 peer-2
scpd 34.101.131.0 peer-3
scpd 34.101.56.179 peer-4
scpd 34.101.252.194 peer-5
scpd 34.101.214.2 peer-6
scpd 34.128.87.115 peer-7
scpd 34.101.220.136 peer-8

1667489670
netd 34.128.119.200 1667490000 peer-1
netd 34.101.227.234 1667490000 peer-2
netd 35.247.146.237 1667490000 crdt-p2p

scpd 34.128.119.200 peer-1
scpd 34.101.227.234 peer-2
scpd 34.101.131.0 peer-3
scpd 34.101.56.179 peer-4
scpd 34.101.252.194 peer-5
scpd 34.101.214.2 peer-6
scpd 34.128.87.115 peer-7
scpd 34.101.220.136 peer-8



netd 34.128.119.200 1667491620 peer-1
netd 34.101.227.234 1667491620 peer-2
netd 34.143.155.91 1667491620 crdt-ws

scpd 34.128.119.200 peer-1
scpd 34.101.227.234 peer-2
scpd 34.101.131.0 peer-3
scpd 34.101.56.179 peer-4
scpd 34.101.252.194 peer-5
scpd 34.101.214.2 peer-6
scpd 34.128.87.115 peer-7
scpd 34.101.220.136 peer-8


```

## CRDT P2P


```
1667407290

netd 34.101.227.234 1667413350 peer-1
netd 34.101.56.179 1667413350 peer-2
netd 35.247.146.237 1667413350 crdt-p2p

scpd 34.101.227.234 peer-1
scpd 34.101.56.179 peer-2






1667408370


netd 34.101.227.234 1667408370 peer-1
netd 34.101.56.179 1667408370 peer-2
netd 35.247.146.237 1667408370 crdt-p2p

scpd 34.101.227.234 peer-1
scpd 34.101.56.179 peer-2
scpd 34.101.131.0 peer-3
scpd 34.128.119.200 peer-4


1667413710

netd 34.101.227.234 1667413710 peer-1
netd 34.101.56.179 1667413710 peer-2
netd 35.247.146.237 1667413710 crdt-p2p

scpd 34.101.227.234 peer-1
scpd 34.101.56.179 peer-2
scpd 34.101.131.0 peer-3
scpd 34.128.119.200 peer-4
scpd 34.101.220.136 peer-5
scpd 34.128.87.115 peer-6
scpd 34.101.214.2 peer-7
scpd 34.128.125.184 peer-8
```

## CRDT CS


```
1667412210

netd 34.101.227.234 1667412210 peer-1
netd 34.101.56.179 1667412210 peer-2
netd 34.143.155.91 1667412210 crdt-cs

scpd 34.101.227.234 peer-1
scpd 34.101.56.179 peer-2






1667411730


netd 34.101.227.234 1667411730 peer-1
netd 34.101.56.179 1667411730 peer-2
netd 34.143.155.91 1667411730 crdt-cs

scpd 34.101.227.234 peer-1
scpd 34.101.56.179 peer-2
scpd 34.101.131.0 peer-3
scpd 34.128.119.200 peer-4





1667411250

netd 34.101.227.234 1667411250 peer-1
netd 34.101.56.179 1667411250 peer-2
netd 34.143.155.91 1667411250 crdt-cs

scpd 34.101.227.234 peer-1
scpd 34.101.56.179 peer-2
scpd 34.101.131.0 peer-3
scpd 34.128.119.200 peer-4
scpd 34.101.220.136 peer-5
scpd 34.128.87.115 peer-6
scpd 34.101.214.2 peer-7
scpd 34.128.125.184 peer-8
```



Real Memory

```
http://34.142.229.79:19999/api/v1/data?chart=apps.mem&dimension=node&after=1667313120&points=0&group=average&gtime=0&timeout=0&format=csv&options=seconds
```

Network

```
http://34.142.229.79:19999/api/v1/data?chart=system.ip&after=1667313120&points=0&group=average&gtime=0&timeout=0&format=csv&options=seconds
```

CPU

```
http://34.142.229.79:19999/api/v1/data?chart=apps.cpu&dimension=node&after=1667313120&points=0&group=average&gtime=0&timeout=0&format=csv&options=seconds
```

