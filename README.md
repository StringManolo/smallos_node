# smallos_node (informal fork of [small](https://github.com/stringmanolo/small))

Small is a tiny userland distro. This is the aarch64 version patched to run with proot-distro under termux. This fork is made just for develop node apps in termux

##### Full Install on Termux

```bash
git clone https://github.com/stringmanolo/smallos_node
cd smallos_node
pkg install proot-distro
./installInProotDistro.sh
```

##### Usage

- Login into small:
```bash
sos_node
```

- Run a command inside small
```bash
sos_node ls -a
```

