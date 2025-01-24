# Lab - Investigate Kali Linux

## Objectives

In this lab, you will complete the following objectives:

- Familiarize yourself with the Kali Linux GUI.
- Familiarize yourself with the Kali Linux shell.

## Background / Scenario

Linux is open source, fast, reliable, and small. It requires very little hardware resources to run and is highly customizable. Unlike other operating systems such as Windows and Mac OS X, Linux was created, and is currently maintained by, a community of programmers. Linux is part of several platforms and can be found on devices anywhere from “wristwatches to supercomputers.” Because Linux is open source, any person or company can get the kernel’s source code, inspect it, modify it, and re-compile it at will. They are also allowed to redistribute the program with or without charges.

Linux distributions are packages created by different organizations. Linux distributions (or distros) include the Linux kernel with customized tools and software packages. While some of these organizations may charge for their Linux distribution support (geared towards Linux-based businesses), most of them also offer their distribution for free without support. Debian, Red Hat, Ubuntu, CentOS, and SUSE are just a few examples of Linux distributions.

Kali Linux is a special version of Linux designed specifically for security auditing and penetration testing. Many changes have been implemented to ensure security, system integrity, and security-specific capabilities. It is not recommended to use Kali for standard uses, such as gaming, development, and other day-to-day uses. As a security and pentesting expert, it is very important for you to know how to get around in Kali, both in the GUI and at the terminal. You need to be able to find the tools that you need to perform your job and manipulate files in the file system.

## Required Resources

- Kali VM customized for Ethical Hacker course
- Internet access

---

## Instructions

### Part 1: Familiarize Yourself with the Kali Linux GUI

#### Step 1: Start the VM and learn about the Kali GUI

1. Log into the Kali system with the username `kali` and the password `kali`. You are presented with the Kali desktop.
   
   - Like the Windows desktop, Kali has icons representing things like the trash, file explorer, and other links.
   - There are also several icons across the top, like the Windows taskbar. In addition, icons for running applications will appear there. This is called the panel.

2. From the panel, you can:
   - Launch the Firefox web browser and terminals.
   - Set up additional desktops using the numbered buttons. Each desktop can be configured differently with specific links and files on it.

3. Right-click the panel, click **Panel**, and then **+ Add New Items...**
   - Here you can add many items to the panel to help you get to the tools and configurations that you use the most.

4. Right-click the panel, click **Panel**, and then **Panel Preferences...**
   - Here you can modify many settings to customize how the panel works and what it looks like. Additional panels can be added as well, to accommodate more items.

5. Investigate the settings and change the settings if you desire. Close both configuration windows when you are finished.

6. The top-right corner shows settings and information, such as network connection, audio, time and date, and the power button. You can add additional items to this area using the panel configuration.

#### Step 2: Navigate the Applications menu

1. Click the first icon on the left side of the panel. This opens the **Applications menu**.
   - Like the Start button in Windows, this menu contains shortcuts to the applications and settings in the operating system.
   - From here, you can navigate to any of the tools that have been installed, find the operating system settings, and search for anything you are looking for.

2. Navigate through the folders and look at all the different tools. Open a few if you would like to see them.
   - Note that some of the tools have GUIs, but most open in a terminal window.

3. Close any open windows and click the square black and white icon in the panel. This will open a terminal for the next part of the lab.

---

### Part 2: Familiarize Yourself with the Kali Linux Shell

The shell refers to the command interpreter in Linux. Also known as the terminal, command line, or command prompt, the shell is a very powerful way to interact with a Linux computer.

Linux commands are programs created to perform specific tasks. Use the `man` command (short for manual) to obtain detailed documentation about commands. For example, `man ls` provides documentation about the `ls` command from the user manual.

#### Step 1: Command documentation

1. To learn more about the man page, open a terminal, and type:

   ```bash
   man man
   ```

2. Scroll through the output and name a few sections that are included in a man page.
   
   **Answer Area**

3. Type `q` to exit the man page.

4. To invoke a command via the shell, simply type its name. The shell will try to find it in the system path and execute it.

   The table below lists some basic Linux commands and their functions:

   | Command    | Description                                                          |
   |------------|----------------------------------------------------------------------|
   | `mv`       | Moves or renames files and directories.                              |
   | `chmod`    | Modifies file permissions.                                          |
   | `chown`    | Changes the ownership of a file.                                    |
   | `dd`       | Copies data from an input to an output.                             |
   | `pwd`      | Displays the name of the current directory.                         |
   | `ps`       | Lists the processes that are currently running in the system.       |
   | `su`       | Simulates a login as another user or to become a superuser.         |
   | `sudo`     | Runs a command as a super user, by default, or another named user.  |
   | `grep`     | Searches for specific strings of characters within a file.          |
   | `ifconfig` | Displays or configures network card related information.            |
   | `apt-get`  | Installs, configures, and removes packages on Debian-based systems. |
   | `iwconfig` | Displays or configures wireless network card related information.   |
   | `shutdown` | Shuts down the computer.                                            |
   | `passwd`   | Changes the password for a user.                                    |
   | `cat`      | Lists the contents of a file.                                       |
   | `man`      | Displays the documentation for a specific command.                  |

5. Many command line tools are included in Linux by default. Users can pass parameters and switches along with the command to adjust its operation. For example:

   | Command  | Description                                      |
   |----------|--------------------------------------------------|
   | `ls`     | Displays the files inside a directory.           |
   | `cd`     | Changes the current directory.                  |
   | `mkdir`  | Creates directories.                            |
   | `cp`     | Copies files and directories.                   |
   | `rm`     | Removes files or directories.                   |
   | `grep`   | Searches for specific strings within a file.    |
   | `cat`    | Lists the contents of a file.                   |

6. For complete help on everything Kali Linux, open the Firefox web browser and go to [Kali Linux Documentation](https://www.kali.org/docs/).

---

### More Steps (Omitted for Brevity)

- **Step 2: Create and change directories**
- **Step 3: Redirect output**
- **Step 4: Redirect and append to a text file**
- **Step 5: Delete files and directories**
- **Step 6: Move files and directories**
