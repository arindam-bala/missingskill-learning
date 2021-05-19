# **Linux Operating System**
---
## **Sections**
- [History](#Introduction)
- [Linux Terminal Commands](#about-Richard-Stallman)
- [Linux File System](#file-system)

## **History**
---
### **Basics**
* To understand the history of **Linux** we have to take a look back in **1970s**.

* Before Bell Labs was introduced **UNIX** operating system, Computer was only used in **NASA or DARPA** space and military agencies of US

* Years of discovering and developing and upgrading the Linux Kernal based OS :
 
    ( 1970 | 1980 | 1985 | 1986 | 1990 | 1991 |1995 | 2020 )

* **Linux was first developed in Bell labs** and that time the operating system was called UNIX operating system.

* **Engineers and Scientists** of **Bell Labs** started to create their own system called UNIX.They started to sell this operating system to different **Companies** and **Universities**.At that time price is about $2000 to $40000 to get a UNIX system.

* Examples of some UNIX in 1980s:
    
    * **Apple UNIX**
    * **HP UNIX**
    * **IBM UNIX**

### **Richard Stallman**    

* **Richard Matthew Stallman**, also known by his initials, RMS, is an American free software movement activist and programmer. He campaigns for software to be distributed in a manner such that its users receive the freedoms to use, study, distribute, and modify that software.

* In **1980s** Richard Stallman starts to create a free software with the help of his friends.

* In **1985** he started a non profit organization known as **Free Software Foundation(FSF)**

* **Richard Stallman** is the **God father** of the journey of free software in the World.
In **1985** he started creating his own Operating System called **GNU**.

* The kernel of GNU is known as **HURD**.

* In **1986 Richard Stallman** build an operating system called **BSD/UNIX**


###  **Linus Torvalds**
---
* In between **1987** to **1990** a person named **Linus Torvalds** was doing some research on Physics and Mathematics and he was wanted to use the **BSD/LINUX** system.

* Linus Torvalds don’t like **BSD/LINUX** system and both **Linus Torvalds** and **Richard Stallman** build a Kernal called Linux.. Which was totally free.

* **Linux is a Kernal**.But **GNU Linux** is an operating system.Where **GNU** is actually a group or collection of free software.

* This GNU Linux is completely free from **1991**.


* **(1992-1994)** **Netscape** (First Browser)
* **(1995-1996)** **Google** came and all new technologies came from **GNU Linux**.

* In today’s world in **2021** almost **99%** of worlds computer software technology is based on Linux.

## **Linux Terminal Commands**
---
1. **ls** : shows all the files and folders in the current directories, ls actually represents list.

1. **ls – l** : shows all the files and folders in the current directories in a descriptive manner.

1. **uname**  : shows user name of your computer

1. **uname -r** : shows user name in details [ -r represents recursive]

1. **uname -a** : for all details

1. **history** : shows all commands fired by user

1.  **cd ..**  : catch directory and goto level back one directory( change directory)

1. **mv** :move or cut

1. **cp**  : copy cp filename/directory name

1. **rm** : remove or delete

1. **/#**  stands for user directory

1. **~#**     stands for root directory

1. **touch**  :for creating a file in the selected directory
1. **mkdir** :for creating a directory

1. **rmdir** : to remove a directory

1. **ls -l test** :[permission checking command of a file]

1. **chmod 764 test**  :     [change permission manually according to values sum of symbol]

1. **pwd**  : print working directory( simply shows the current directory)

1. **who**  :

1. **who I am** :

1. **cat**   : displays all the content in the file inside the terminal

1. **less** : will give you more data

1. **more** :will give you less data

1. **echo** : to print something ( print anything like a number or string given as a parameter)

1. **echo $PATH**  : prints the whole path of the system

1. **top** : this command is used for monitor system use(system load information)
		
        * for exit press <q> in the keyboard
1. **ps**  : networking commands used to view all the applications which is running
	
    * ps -ef   is also used for detailed output ( gather information of running processes)


1. **ifconfig** : checking network status

1. **wget**  https://ipinfo.io  : getting ip address information  file is saved in your pc in
 index.html format , this file can be run using json application 
    
    * wget is nothing but a command line browser


1. **wget** https://ipinfo.io/json              

    * running this file with json
1. **cat json**  :  open the file information

1. **exit**  : exit from the terminal

1. **whoami**   : prints the login user

1. **who**   : list of login users

1. **ping**   : check the internet connection and possibly speed
1. **ssh**   : access the remote server

1. **which**  : this command prints the address path of the program which is given as an argument
		
        * example : which firefox , which ls( this gives path of this command)


## **Linux File System**
---
Most users of  Linux have seen the root directory but not everybody understands what 
the directories are used for. A Windows user when opens **my computer** looks C: Drive, where the 
program files and Windows directories are present. But in case of Linux based Operating Systems
there is no such place named as C: Drive. In Linux if we open **file system** we can see many folders.
Among those folders there is a Home directory and a root directory.All the folders present inside the
**file system** of Linux Opereating System contructs a Linux File System Structure. The file system 
structure of Linux is totally different from Windows Operating System.
 
### **Directories of Linux System**
---
**From top to bottom, the directories you are seeing are as follows.**

* **/bin** : bin stands for binaries,all the binary programs are present inside this bin directory. These binary programs runs in CLI inside terminal. Some examples of binaries are **cat, sudo, chmod**.                

* **/boot** : boot directory contains **boot loader**. It is a program which starts or booting the computer. 

* **/dev** : dec directory contains device files.Some of these files are generated at the time of booting. Another files are generated when a device is connected to the computer. Such as a **USB FLASH DRIVE** or a **WEB CAM**.

* **/etc** : this dicrectory names from **et cetera**. It consists of configuration files. Some example is : files that contains name of computer, files that contains user passwords.

* **/home** :  Home directory contains each user's personal files. Each user can only access their own files from home directory by entering their passwords.

* **/lib** : lib directory stands for libraries.
this directory includes **lib32** and **lib64** folders.All the libraries are stroed inside this folder.
Libraries are files that applications are used to perform various functions.

* **/media** : media directory automatically creates files for mounting devices such as **Pendrive, usbstick , card reader**.

* **/mnt** : mnt represents mount. This is also used for media device files but used manually.

* **/opt** : opt stands for optional folder. This directory is used for manually installed softwares from vendors. This is also used for softwares created by the user.

* **/proc** : proc is a **virtual directory**, used for pseudo files. These are not actual files, they are generating by kernels in the runtime of OS.

* **/root** : root is the home directory for the **superuser** also known as **administrator**.Only administrator can access this root folder by using admin password.

* **/run** : This directory is used by **RAM** of the system. All files generated inside this folder is actually present inside the RAM. When computer is shutdown all files inside it are gone.

* **/sbin** : This directory includes system binaries. A **system administrator** could use this binaries and standard user would'nt have access to this directory without permission.

* **/usr** :This directory is used for user applications. Inside this folder bin sbin, lib and other folders are found. This folder is also known as **UNIX SYSTEM RESOURCE**. User applications are installed in several folders inside this usr directory. Normal programs are generally stored inside the local folder and larger programs are installed inside the shared folders.

* **/srv** : This is the service directory where service data is stored. This directory is actually used when an user runs a server such a **web-server** or a **ftp server** it stores files that will be used by external users.

* **/sys** : sys stands for system files.This directory directory interact with the kernel.This folder is similar as run folder. When the system boots up this directory is created and used and after shutting down all files and directories are torally erased.

* **/tmp** : This is the temporary directory. This contains temporary files generated by applications. After saving data or termination of a application the temporary files are completely removed from this directory.

* **/var** : var is the variable directory. It contains files and directories that can grow inside. Means the size of those files and directories may change with time of processing.This directory is totally maintained by the system itself.

* **/snap** : This directory is used for storing snapshot of the operating system current states for future use when a problem may occurs in the system. This folder actually saves a backup of the system current configuration as log files.







	
		






