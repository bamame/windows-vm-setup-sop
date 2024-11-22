# Standard Operating Procedure

**Company Name**: MITT  
**Address**: 130 Henlow Bay, Winnipeg, MB R3Y 1G4  
**Phone Number**: +1(204)9896500  
## Revision History
| Version | Date       | Author  | Approved by  | Description      |
|---------|------------|---------|--------------|------------------|
|  1.0    | 2024-11-22 | YiWei   | Felix        |Initial SOP draft


---

## Purpose
To standardize the process of installing Windows OS on a virtual machine using VMware, ensuring efficiency and consistency.

---

## Application
This document applies to new developers during their onboarding process to set up a Windows virtual machine for development tasks.

---

## Definitions
1. VM: Virtual Machine, a software-based emulation of a physical computer.  
2. VMware: A virtualization platform used to create and manage virtual machines.  
3. ISO File: A disk image file format used for installing operating systems.  
4. Host Machine: The physical computer where VMware is installed and virtual machines are hosted.  
5. NAT (Network Address Translation): A networking method that allows the virtual machine to access external networks using the host machine's IP address.

---

## Prerequisites
- Windows Server ISO file
- Minimum system requirements: 8 GB RAM, 100 GB disk space
- Valid license key

---

## Installation Steps

### **Step 1: Create a New Virtual Machine**
1. Open **VMware Workstation/Player**.
2. Click on **Create a New Virtual Machine**.
3. Select **Typical (recommended)** as the configuration type and click **Next**.
4. In the installation source, choose **I will install the operating system later**, and click **Next**.


### **Step 2: Configure Virtual Machine Settings**
1. Choose the operating system:
   - Select **Microsoft Windows** as the operating system type.
   - Choose **Windows Server 2022** as the version.
2. Set the virtual machine name:
   - Name the virtual machine (e.g., `WinSer2022`).
   - Specify the location to save the virtual machine.
3. Specify disk capacity:
   - Allocate **100 GB** for the disk.
   - Choose **Store virtual disk as a single file**.
4. Customize hardware:
   - Assign at least **8 GB of RAM** (8 GB recommended).
   - Allocate appropriate CPU cores based on your hardware.
   - Under **CD/DVD Settings**, select **Use ISO image file** and load the Windows Server 2022 ISO file.

### **Step 3: Start the Virtual Machine**
1. Click **Finish** to create the virtual machine.
2. Select the newly created VM and click **Power On**.
3. The installation process for Windows Server 2022 will begin.

### **Step 4: Install Windows Server 2022**
1. Follow the on-screen prompts to:
   - Select your language, time, and keyboard layout.
   - Click **Install Now**.
2. Enter a valid product key.
3. Select the **Windows Server Edition** you want to install (e.g., Standard or Datacenter).
4. Choose **Custom Installation** to install a fresh copy of Windows.
5. Partition the virtual disk:
   - Select the allocated disk and click **Next**.

### **Step 5: Complete Setup**
1. Wait for the installation process to finish.
2. Configure the **Administrator Password** when prompted.
3. Log in to the system using the Administrator account.

---

## Testing & Verification
- Verify server connectivity via Remote Desktop.
- Test DNS and DHCP roles, if applicable.

---

## Maintenance
- Perform regular updates using Windows Update.
- Monitor system performance using Task Manager.

---

## Resources
- [VMware Workstation Documentation](https://www.vmware.com/products/workstation-pro.html)
- [Windows Server 2022 Overview](https://www.microsoft.com/en-us/windows-server)
- [Troubleshooting VMware Issues](https://kb.vmware.com/)
