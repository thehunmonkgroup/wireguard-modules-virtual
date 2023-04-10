# wireguard-modules-virtual

Provide `wireguard-modules` virtual package for kernels that don't properly declare it.

## Purpose

Some kernels provide the wireguard kernel module natively, but do not correctly declare this in their kernel packaging.

This can lead to problems when installing other wireguard packages.

This virtual package just stands in for the kernel packaging error, by providing the `wireguard-modules` virtual package.

## Building

From the directory above the repository root:

```sh
dpkg-deb --build wireguard-modules-virtual

```

## Installing

```sh
sudo dpkg -i wireguard-modules-virtual.deb
```
