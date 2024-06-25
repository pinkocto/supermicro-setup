## Creating a Bootable Ubuntu Installation USB with Rufus

### 1. Download and Install Rufus:
- Go to the Rufus official website [rufus.ie](https://rufus.ie/ko/) and download Rufus.
- Run the downloaded executable to start Rufus (no installation is required as it is a portable application).

<img src="https://github.com/pinkocto/supermicro-setup/assets/57980370/3a303632-3adc-4eb5-acdf-f359dfeb6d3a" alt="https://rufus.ie/ko/" width="500" height="250">

### 2. Download the Ubuntu ISO File:
- Visit the Ubuntu official website and download the latest Ubuntu Desktop ISO file.

### 3. Run Rufus:
- Open Rufus. You might need to run it as an administrator.

### 4. Select the USB Drive:
- In the "Device" dropdown menu, select the USB drive you want to use for the bootable USB.

*Warning: All data on this USB drive will be erased, so make sure to back up any important data.*

### 5. Boot Selection:
- Under "Boot selection", choose "Disk or ISO image (Please select)".
- Click the "Select" button and navigate to where you downloaded the Ubuntu ISO file, then select it.

### 6. Partition Scheme and Target System:
- Partition scheme: Select "GPT" (this is suitable for most modern systems with UEFI).
- Target system: Select "UEFI (non CSM)".

### 7. File System and Cluster Size:
- File system: Select "FAT32".
- Cluster size: Leave it at the default setting.

### 8. Start the Process:
- Once all settings are configured, click the "Start" button.
- A warning message will appear indicating that all data on the USB drive will be destroyed. Confirm by clicking "OK".

### 9. Wait for the Process to Complete:
- Rufus will create the bootable USB drive. This process may take several minutes.
- Once the process is complete, click "Close" to exit Rufus.

Now your bootable Ubuntu installation USB is ready. You can proceed with configuring your BIOS settings and installing Ubuntu as described in the previous instructions.
