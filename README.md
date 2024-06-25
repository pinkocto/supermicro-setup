# supermicro-setup
> supermicro server setup-guide

By following this order, you will correctly erase the existing Rocky Linux installation, install the new Ubuntu operating system, and then install and configure the OpenSSH server.

### 0. Preparing the Ubuntu Installation USB
***0.1. Download Ubuntu ISO:***
- Go to the [Ubuntu website](https://ubuntu.com/download/desktop).
- Download the latest Ubuntu Desktop ISO file.
<img src="https://github.com/pinkocto/supermicro-setup/assets/57980370/015babd9-4fd6-4dc5-bdbc-a7781bd509fa" alt="description" width="500" height="250">

***0.2.Create a Bootable USB Drive:***
- Use a tool like [Rufus](https://rufus.ie/ko/) (for Windows), balenaEtcher (for Windows, macOS, and Linux), or the Startup Disk Creator (for Ubuntu) to create a bootable USB drive.
- Insert the USB drive into your computer.
- Open the tool you chose to use.
- Select the downloaded Ubuntu ISO file.
- Select the USB drive as the destination.
- Click the button to start creating the bootable USB drive.

Once the bootable USB drive is ready, you can proceed with the BIOS settings configuration and the installation process.


### 1. BIOS Settings Configuration

***1.1. Boot Settings***
- Enter the BIOS setup.
- Navigate to the `Boot` menu.
- Set the boot device to `UEFI USB Hard Disk`

***1.2. Advanced Settings:***
- Navigate to the `Advanced` tab.
- Go to `CPU Configuration`.
- Check the setting `Intel® Virtualization Technology` and ensure it is set to `Disabled`

***1.3. Reboot:***
- Save changes and exit the BIOS setup.
- Insert the USB drive with the Ubuntu installation media.
- Reboot the system to apply the new BIOS settings and start the installation from the USB drive.

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
