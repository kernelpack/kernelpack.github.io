# yuros kernel pack

## gain administrator

```
sudo su
```
## edit pacman.conf
```
nvim /etc/pacman.conf 
```

## add this line at the end of pacman.conf file
```
[yuros_kernel]
SigLevel = Optional TrustAll
Server = https://kernelpack.yuros.org/$arch
```

## update database
```
pacman -Syy
```

## install kernel
```
pacman -S linux-karim
```
