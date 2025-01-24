# Deploy a Pre-Built Kali Linux Virtual Machine (VM)

## Objectives
In this lab, you will complete the following objectives:

1. Deploying a Customized Kali Linux VM on AMD or Intel Chip-based Computer
2. Deploying a Customized Kali Linux VM on ARM M1/M2 based macOS Computer
3. Exploring Linux

## Background / Scenario
Computing power and resources have increased tremendously in a short period of time. A benefit of multi-core processors and large amounts of RAM is the ability to run multiple operating systems on a computer using virtualization.

With virtualization, one or more virtual computers can operate on a single physical computer. Virtual computers that run on physical computers are called virtual machines (VMs). Virtual machines are often called guests, and physical computers are often called hosts. Anyone with a modern computer and operating system can run virtual machines.

In this lab, you will first install a desktop virtualization application, such as Oracle VirtualBox, and deploy a virtual machine running a Kali Linux OS.

## Required Resources
- Computer with a minimum of 4 GB of RAM and 50 GB of free disk space
- Internet access to download virtualization software, Oracle VirtualBox or UTM, and VM image

## Instructions
### Preliminary Step: Check Virtualization Capability
Ensure your computer supports virtualization. If unsure, perform an internet search to confirm and enable virtualization as necessary.

### Part 1: Deploying a Pre-Built Customized Kali VM on AMD or Intel Chip-based Computer

#### Step 1: Download and Install VirtualBox
1. Navigate to [https://www.virtualbox.org/](https://www.virtualbox.org/).
2. Click the download link and choose the appropriate installation file based on your operating system.
3. Run the installer and accept the default installation settings.

#### Step 2: Download the Pre-built Customized Kali VM
1. Navigate to the Resource Hub on [skillsforall.com](https://skillsforall.com/).
2. Download the `OVA` file for this course and note its location on your computer.

#### Step 3: Deploy the VM in VirtualBox
1. Open VirtualBox.
2. Click **File > Import Appliance** and select the downloaded `Kali.ova` file. Click **Next** to continue.
3. Review the appliance settings and adjust RAM if needed. Click **Finish** to complete the import.
4. Click **Start** to power up the newly created VM.

### Part 2: Deploying a Pre-Built Customized Kali VM on ARM M1/M2 Chip-based Computer

#### Step 1: Download and Install UTM
1. Navigate to [https://mac.getutm.app/](https://mac.getutm.app/).
2. Click **Download** to get the free version of UTM.
3. Install UTM after downloading the file.

#### Step 2: Download and Load the Pre-built Customized Kali
1. Navigate to the Resource Hub on [skillsforall.com](https://skillsforall.com/).
2. Download the `Kali.utm.zip` file and note its location on your computer.
3. Unzip the archive and double-click the unzipped file to open the VM in UTM.

### Part 3: Exploring Linux

#### Step 1: Root Privileges
1. Log into the Kali system using the username `kali` and password `kali`.
2. Open a terminal emulator by right-clicking the desktop, selecting **Applications**, and clicking **Terminal Emulator**.
3. Attempt to view and edit the file `/etc/sudoers` using the `visudo` command.
   ```
   visudo
   visudo: /etc/sudoers: Permission denied
   ```
4. Temporarily elevate permissions using `sudo visudo`:
   ```
   sudo visudo
   ```
5. Scroll to the end of the file and observe the configurations that allow users in the `sudo` group to execute commands. Exit without saving changes.

6. Verify that the `kali` user is part of the `sudo` group:
   ```
   grep sudo /etc/group
   ```
   Output:
   ```
   sudo:x:27:kali
   ```

#### Step 2: Keyboard Shortcuts
1. Use the **up** arrow key to locate the previously entered `visudo` command. Note how many presses were needed.
2. Use the **down** arrow key to locate the `sudo visudo` command. Note how many presses were needed.
3. View the command history using the `history` command:
   ```
   history
   ```
   Example output:
   ```
       1  visudo
       2  sudo visudo
       3  grep sudo /etc/group
       4  history
   ```
4. Repeat commands using the history number:
   - Enter `!3` to re-run the command `grep sudo /etc/group`.
   - Enter `!his` to re-run the `history` command.

5. Use the **Tab** key for autocompletion:
   - Enter `hi` and press **Tab**. The system will autocomplete `history`.
   - Enter `ls /me` and press **Tab** to autocomplete `/media`. Press **Enter** to view the folder contents.

### Reflection Question
**What are the benefits of using either the installer image or the pre-built image to create the Kali VM?**

Answer:
- **Installer Image**: Offers more customization options during the setup process, allowing you to tailor the VM to your specific needs.
- **Pre-built Image**: Saves time by providing a ready-to-use environment with pre-configured settings, making it ideal for quick deployments or training purposes.
