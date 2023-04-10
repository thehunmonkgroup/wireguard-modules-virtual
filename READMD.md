# wireguard-modules-virtual

Provide wireguard-modules package dependency for kernels that don't declare it.

## Building

From the directory above the repository root:

```sh
dpkg-deb --build wireguard-modules-virtual

```

## Installing

```sh
sudo dpkg -i wireguard-modules-virtual.deb
```
