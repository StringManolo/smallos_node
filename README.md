# smallos_node (informal fork of [small](https://github.com/stringmanolo/small))

Small is a tiny userland distro. This is the aarch64 version patched to run with proot-distro under termux. This fork is made just for develop node apps in termux

## Install and Usage
##### Full Install on Termux

```bash
git clone https://github.com/stringmanolo/smallos_node
cd smallos_node
pkg install proot-distro
./installInProotDistro.sh
```

##### Usage

- Login into sos_node
```bash
sos_node
```

- Run a command inside sos_node
```bash
sos_node ls -a
```

## Info
##### sos_nodeFileSystem
sos_nodeFileSystem is a minimal distro configured version with basic software
- npm 8.1.3
- node v17.8.0
- apk-tools 2.12.7

##### sos_node.7z 
sos_node.7z is a minimal distro configured version.  
This version doesn't have npm and node installed.  
To install:  
```bash
rm sos_nodeFileSystem;
7z x sos_node.7z -o./sos_nodeFileSystem;
./installInProotDistro.sh
sos_node
apk update
apk add npm
```

## Extra
You can fork this project and export your full distro with all your installed packages, historial of commands, etc. Just use the exportInstalledSos_node.sh script to generate your sos_node-installed.7z file.  
  

You can import your sos_node-installed.7z by extracting the folder inside, renaming it to sos_nodeFileSystem.   
  

Then you can push the changes to your fork using the git add, commit and push commands.    
  

Once you updated your fork, install your custom system following default termux install instructions.
