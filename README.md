# supermicro-setup
> supermicro server setup-guide

By following this order, you will correctly erase the existing Rocky Linux installation, install the new Ubuntu operating system, and then install and configure the OpenSSH server.

### 1. BIOS Settings Configuration

***1. Boot Settings***
- Enter the BIOS setup.
- Navigate to the `Boot` menu.
- Set the boot device to UEFI USB Hard Disk

***2. Advanced Settings:***
- Navigate to the Advanced tab.
- Go to CPU Configuration.
- Check the setting Intel® Virtualization Technology and ensure it is set to Disabled

### 2. Installing a new Ubuntu operating system
- Connect to the internet: `Use wired connection`
- What do you want to do with Ubuntu?: `install Ubuntu`
- How would you like to install Ubunto?: `Interactive installation`
- What apps would you like to install to start with?: `Default selection`
- How do you want to install Ubunto?: `Erase disk and install Ubuntu` (Check "Advanced features: None.")
- Create your account
- Install

### 3. Installing and configuring the OpenSSH Server on a new Ubuntu installation
```python
# Before running the following code, configure the network settings.
# Click the network icon in the top-right corner > click the gear icon > Ethernet > IPv4 > Manual (enter Addresses and DNS) > Apply.
# If the network is connected properly, open the terminal and enter the following code.
sudo apt update
sudo apt install openssh-server
```
