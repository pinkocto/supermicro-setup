# supermicro-setup
> supermicro server setup-guide


- Boot: `UEFI USB Hard Disk`
- Advanced > CPU Configuration
*Check the setting `Intel® Virtualization Technology` and ensure it is set to `Disabled`*

### Installing a new Ubuntu operating system
- Connect to the internet: `Use wired connection`
- What do you want to do with Ubuntu?: `install Ubuntu`
- How would you like to install Ubunto?: `Interactive installation`
- What apps would you like to install to start with?: `Default selection`
- How do you want to install Ubunto?: `Erase disk and install Ubuntu` (Check "Advanced features: None.")
- Create your account
- Install

### Installing and configuring the OpenSSH Server on a new Ubuntu installation
```python
# Before running the following code, configure the network settings.
# Click the network icon in the top-right corner > click the gear icon > Ethernet > IPv4 > Manual (enter Addresses and DNS) > Apply.
# If the network is connected properly, open the terminal and enter the following code.
sudo apt update
sudo apt install openssh-server
```
