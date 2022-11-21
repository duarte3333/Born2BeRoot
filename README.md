# Born2BeRoot

<h2 id="What is a Virtual Machine">What is a Virtual Machine?</h2>
<p>A virtual machine (VM) is a computer that runs entirely on 
software instead of physical hardware. 
Virtual machines use software on a physical (host) computer to replicate or emulate the functionality 
of a different computer or operating system. In essence, a VM is a simulated computer within a real computer.</p>

<p>From a user perspective, virtual machines function just like normal computers. 
They have an operating system (OS), store files, run programs, and even have virtual 
hardware components. But because VMs are entirely software-based, 
they need to borrow hardware resources from a host computer. For example, in a virtual 
machine, the physical host computer’s real Central Processing Unit (CPU) is used to model a virtual CPU.</p>

<p>The software that creates a VM is called a hypervisor, so the hypervisor manages the hardware 
and separates physical resources from the virtual environment.
If the VM user wants to perform a task that requires resources from the 
physical environment, the hypervisor manages the request and gives permission 
to the guest OS to access the physical resources of the real computer.</p>

Advantages of a VM:
<ul>
  <li>Allows to create an environment to test unstable programs</li>
  <li>Makes possible to run several operating systems on the same computer easily</li>
  <li>Easy to implement, because is possible to copy VMs to another physical device.</li>
</ul>

<h2 id="What is a Virtual Machine">What is a Virtual Hard Disk?</h2>
<p>A virtual hard disk (VHD) or a “virtual drive”, is essentially a file on your computer that is “mounted” as a hard drive. Your operating system sees it as a independent hard drive. Virtual hard drives are most commonly used in connection with a “virtual machine” which is a emulated OS that exists on the virtual drive and is launched via virtualization software such as VMWare, or VirtualBox, or Microsoft Hypervisor.</p>
<p>The Virtual Machine stores the settings of the system, this includes 
the quantity of CPUs, memory, hard disks, SCSI controllers, etc. On the other hand, the Virtual Hard 
Disks contain the actual data (boot volumes, data volumes, etc.)</p>
<p>Is possible to save a VHD on a USB flash memory device, since they are independent 
of the Hardware thanks to the hypervisor. So a VHD is type of disk drive that has similar 
functionalities as a typical hard drive but is accessed, managed and installed 
on a virtual machine infrastructure, such as Hyper-V, VMWare Workstation, etc...</p>
<h2>What is LVM</h2>
LVM stands for Logical Volume Management. It is a system of managing logical volumes, or filesystems, that is much more advanced and flexible than the traditional method of partitioning a disk into one or more segments and formatting that partition with a filesystem. LVM as "dynamic partitions", meaning that you can create/resize/delete LVM "partitions" (they're called "Logical Volumes" in LVM-speak) from the command line while your Linux system is running: no need to reboot the system to make the kernel aware of the newly-created or resized partitions.
<h2> What is Operating System?</h2>
An operating system (OS) is the program that, after being initially loaded into the computer by a boot program, manages all of the other application programs in a computer. The application programs make use of the operating system by making requests for services through a defined application program interface (API).

<h2> What is UNIX? </h2>
<p>UNIX is an operating system which was first developed in the 1960s, and has been under constant development ever since.The UNIX operating system is made up of three parts; the kernel, the shell and the programs. </p>
<h3> The kernel</h3>
<p>The kernel of UNIX is the hub of the operating system: it allocates time and memory to programs and handles the filestore and communications in response to system calls.</p>
<p>As an illustration of the way that the shell and the kernel work together, suppose a user types rm myfile (which has the effect of removing the file myfile). The shell searches the filestore for the file containing the program rm, and then requests the kernel, through system calls, to execute the program rm on myfile. When the process rm myfile has finished running, the shell then returns the UNIX prompt % to the user, indicating that it is waiting for further commands.</p>
<h3> The shell</h3>
<p>The shell acts as an interface between the user and the kernel. When a user logs in, the login program checks the username and password, and then starts another program called the shell. The shell is a command line interpreter (CLI). It interprets the commands the user types in and arranges for them to be carried out. The commands are themselves programs: when they terminate, the shell gives the user another prompt (% on our systems).</p>

<h2> Linux</h2>
Linux is an open source operating system (OS). Linux was designed to be similar to UNIX, but has evolved to run on a wide variety of hardware from phones to supercomputers. Every Linux-based OS involves the Linux kernel—which manages hardware resources—and a set of software packages that make up the rest of the operating system.
<p>The OS includes some common core components, like the GNU tools, among others. These tools give the user a way to manage the resources provided by the kernel, install additional software, configure performance and security settings, and more. All of these tools bundled together make up the functional operating system. Because Linux is an open source OS, combinations of software can vary between Linux distributions.</p>

<h2>Debian vs CentOS</h2>
<table>
  <tr>
    <th>CentOS</th>
    <th>Debian</th>
  </tr>
  <tr>
    <td>Red Hat community</td>
    <td>Debian individuals</td>
  </tr>
  <tr>
    <td>Doesn't support much architectures/td>
    <td>Has more packages</td>
  </tr>
  <tr>
    <td>More Stable</td>
    <td>Less Stable</td>
  </tr>
  <tr>
    <td>Long testing cycle</td>
    <td>Short testing cycle</td>
  </tr>
  <tr>
    <td>Best for servers</td>
    <td>Best for software</td>
  </tr>
  <tr>
    <td>Bad GUI</td>
    <td>Good GUI</td>
  </tr>
  <tr>
    <td>More difficult to update to a new version</td>
    <td>Easier to update to a new version</td>
  </tr>
<p>CentOS vs Debian are two flavors of Linux operating systems. For this project, my choice was Debian because has a better user graphical interface, has much more packages and overall it is more suitable for beginners.
</table>

<h2> What is APT?</h2>
<p>APT stands for Advanced Packaging Tool. It is an open-source tool, which means you can use it without the need to pay anything. APT is designed to handle software installation and removal.</p>
<p>APT was part of Debian’s .deb package; however, it was updated to work with the RPM Package Manager. If you have used APT before, you would have noticed that it is a command-line tool. This means you need to use commands to work with it with no visual reference from a graphical interface(the initial plan was to include a graphical interface, but the idea was later dropped).</p>
<p>If you use the apt command, it will not only download and install the required dependencies for the said package. As a user, you do not have to worry about the package dependencies.</p>

<h2>What is Aptitude?</h2>
Aptitude is also an advanced packaging tool. However, it is a front-end tool that gives users access to the user-interface to access functionality. This means that you can use Aptitude to install and remove packages using it. 

<h2>Differences between APT and Aptitude?</h2>
Apt-get being a lower level package manager is restricted only to command line, while Aptitude being a higher-level tool has a default text-only interactive interface along with option of command-line operation by entering required commands.

<h2> What is AppArmor </h2>
AppArmor ("Application Armor") is a Linux kernel security module that supplements the standard Linux user and group based permissions to confine programs to a limited set of resources. AppArmor can be configured for any application to reduce its potential attack surface and provide greater in-depth defense. It is configured through profiles tuned to allow the access needed by a specific program or container, such as Linux capabilities, network access, file permissions, etc. Each profile can be run in either enforcing mode, which blocks access to disallowed resources, or complain mode, which only reports violations.



<h2>Set the basic up</h2>
<p> Login as root: <code>su -</code></p>
<p> Update & Upgrade: <code> apt update</code> and <code> apt upgrade</code></p>
<p> Install sudo: <code> apt install sudo</code></p>
<h3> What is sudo? </h3>
Sudo (sometimes considered as short for Super-user do) is a program designed to let system administrators allow some users to execute some commands as root (or another user). The basic philosophy is to give as few privileges as possible but still allow people to get their work done. Sudo is also an effective way to log who ran which command and when.
<h3>What is a Group?</h3>
A user can create, delete, or modify the file. Group: A group can contain multiple users. All the users belonging to a group have same access permission for a file. Other: Any one who has access to the file other than user and group comes in the category of other.
<h3> What is a Sudo group? </h3>
A sudo group is a group of superusers that have privileged access to root commands.
<h3>Setup</h3>
<p> Create a group: <code>groupadd < namegroup ></code>
<p> Add user to sudo group: <code>adduser dsa-mora sudo</code></p>
<p> Add user to user42 group(should be done in root): <code>adduser dsa-mora user42</code></p>
<p> Delete a user: <code>deluser newuser</code>
<p> If signed in as another non-root user with sudo privileges: <code>sudo deluser newuser</code>
<p> To check if your user is in the sudo group <code>getent group sudo</code></p>
<p> How to find the name and the version of the OS in linux: <code>cat /etc/os-release</code> 
<p>How to change user: <code>sudo -u < user > -s</code><p>
<p>How to remove a user(su -): <code>userdel < username ></code> and delete the user’s home directory <code>userdel -r < username ></code></p>
<p>Command to change a password of a user: <code>sudo passwd vivek < username ></code></p>
<p>See all users: <code>getent passwd</code>


<h2> Password protection </h2>
The main goal here is to force users to use strong passwords in linux
<h3> Linux PAM </h3>
<p>Linux Pluggable Authentication Modules (PAM) is a suite of libraries that allows a Linux system administrator to configure methods to authenticate users. It provides a flexible and centralized way to switch authentication methods for secured applications by using configuration files instead of changing application code. It by default installed on Linux.</p>
<p>Instalation of an adicional module: <code>sudo apt install libpam-crack </code></p>
<p>To back up the file where all the password policies are:</p>
<p><code>sudo cp /etc/pam.d/common-password /etc/pam.d/common-password.bak </code></p>
<p>Opens the file where the user password policies will be changed:</p>
<p><code>sudo nano /etc/pam.d/common-password</code></p>
<p>Add the following line to the file: <code>password required pam_cracklib.so retry=3 minlen=10 lcredit=-1 ucredit=-1 dcredit=-1 difok=7 reject_username </code></p>
Explanation:
<p><code> retry=3 </code>, number of tries</p>
<p><code>lcredit=-1</code>, must have at least one lowercase</p>
<p><code>ucredit=-1</code>, must have at least one uppercase</p>
<p><code>dcredit=-1</code>, must have at least one digit</p>
<p><code>difok=7</code>, number of characters that must be different from the last password </p>
<p><code>reject_username </code>, the password cannot include username</p>
<p><code>enforce_for_root </code>, to implement the same policy on root</p>
<p> File where I change the number of days before the password expire, minimum number of days allowed before the modification of a password and the number of days the user has to receive a warning message before their password expires: <code>sudo nano /etc/login.defs</code></p>
<h4>Get the password expiry information</h4>
<code>sudo change -l < username ></code>

<h2>Setup SSH Service</h2>
<h3>What is SSH?</h3>
SSH or Secure Shell is a network communication protocol that enables two computers to communicate and share data. An inherent feature of ssh is that the communication between the two computers is encrypted meaning that it is suitable for use on insecure networks. SSH is often used to "login" and perform operations on remote computers but it may also be used for transferring data.
<h3>What is OpenSSH?</h3>
OpenSSH is an open-source implementation of the SSH protocol. It is based on the free version by Tatu Ylonen and further developed by the OpenBSD team and the user community.
<h3>What is a SSH key?</h3>
SSH keys are a pair of public and private keys that are used to authenticate and establish an encrypted communication channel between a client and a remote machine over the internet.
<h3>Setup</h3>
<p> Install OpenSSH: <code>sudo apt install openssh-server</code></p>
<p> Verify ssh service: <code>sudo systemctl status ssh</code></p>
<p> Start ssh service: <code>sudo systemctl start ssh</code></p>
<p> Stop ssh service: <code>sudo systemctl stop ssh</code></p>
<p> To start the ssh server everytime I boot the VM: <code>sudo systemctl enable ssh</code></p>
<p> Add port 4242: go to <code>/etc/ssh</code>, run <code>sudo nano sshd_config</code> and edit the <code>#Port22</code> to <code>Port 4242</code></p>
<p>To remotly acess the VM with ssh: <code>ssh < username >@< ip-addr > -p 4242</code>
<p> To terminate SSH session anytime: <code>logout</code>
<p>Check installation: <code>dpkg -l | grep ssh</code></p>


<h2>Hostname and Partitions</h2>
<h3>What is a hostname?</h3>
In computer networking, a hostname is a label that is assigned to a device connected to a computer network and that is used to identify the device in various forms of electronic communication, such as the World Wide Web. In brief, the hostname is what a device is called on a network.
<h3>What is a Firewall?</h3>
A Firewall is a network security device that monitors and filters incoming and outgoing network traffic based on an organization's previously established security policies. At its most basic, a firewall is essentially the barrier that sits between a private internal network and the public Internet.
<h3>What is UFW Firewall?</h3>
Uncomplicated Firewall (UFW) is a program for managing a netfilter firewall designed to be easy to use. It uses a command-line interface consisting of a small number of simple commands, and uses iptables for configuration. UFW is available by default in all Ubuntu installations since 8.04 LTS.
<h3>What is a hostname?</h3>
<p>A hostname is a label assigned to a machine that identifies the machine on the network. Each device in the network should have a unique hostname.</p>
<h3>Setup</h3>
<p> Get your ip: <code>ip a</code>or<code>hostname -I</code></p>
<p> Know what user I am using: <code>whoami</code></p>
<p> To check the current hostname: <code>hostnamectl</code></p>
<p> To change the host name: <code>sudo hostnamectl set-hostname < newhostname ></code>, on success 0 is returned.

<p> Install UFW Firewall: <code> sudo apt install ufw</code>(should reboot after)</p>
<p> Activate UFW: <code>sudo ufw enable</code></p>
<p> To check if its enable: <code>sudo systemctl status ufw</code>, if it isn't do <code>sudo ufw enable</code></p>
<p>See all partitions: <code>lsblk</code></p>
<h2>Sudo Policy</h2>
<h3>What is TTY?</h3>
Linux operating system represents everything in a file system, the hardware devices that we attach are also represented as a file. The terminal is also represented as a file. There a command exists called tty which displays information related to terminal. The tty command of terminal basically prints the file name of the terminal connected to standard input. tty is short of teletype, but popularly known as a terminal it allows you to interact with the system by passing on the data (you input) to the system, and displaying the output produced by the system.
<h3>What is visudo command?</h3>
The visudo command opens a text editor like normal, but it validates the syntax of the file upon saving. This prevents configuration errors from blocking sudo operations, which may be your only way of obtaining root privileges. Traditionally, visudo opens the /etc/sudoers file with the vi text editor.
<h3>Setup</h3>
<p> Go to <code>/etc/sudoers.d</code>  and run <code>sudo visudo</code></p>
<p> Find the <code>Defaults</code> section and add:</p>
<p> To enable TTY <code> Defaults        requiretty</code></p>
<p> To select the right folder for your log files <code> Defaults        logfile="/var/log/sudo/sudo.log"</code></p>
<p>To archive all sudo inputs & outputs to /var/log/sudo/: </p><code>Defaults        iolog_dir="/var/log/sudo"</code></p>
<code>Defaults        log_input, log_output</code></p>
<p> To set your password retries (It usually comes 3 times as default, but still...) <code> Defaults        passwd_tries=3</code></p>
<p> To enable TTY <code> Defaults        badpass_message="Your message"</code></p>
<p> The security pass probably is already there, but in case it isn't <code>Defaults        secure_path="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin"</code></p>
Check if sudo is installed: <code>dpkg -l | grep sudo</code>

<h2>Setting up cron</h2>
<h3>What is cron</h3>
The cron command-line utility is a job scheduler on Unix-like operating systems. Users who set up and maintain software environments use cron to schedule jobs[1] (commands or shell scripts), also known as cron jobs,[2][3] to run periodically at fixed times, dates, or intervals.
<h3>Setup</h3>
<p>To configure cron as root: <code>sudo crontab -u root -e</code></p>
Replace <code># m h  dom mon dow   command</code> to <code>*/10 * * * * sh /path/to/script</code>

<h2 id="Script">Script</h2>
<h3> Create script </h3>
<p> Run: <code>sudo vim /usr/local/bin/monitoring.sh</code></p>
<p> Every bash script start with <code>#!/bin/bash</code></p>
<p> <code>wall</code> is a command-line utility that displays a message on the terminals of all logged-in users. The messages can be either typed on the terminal or the contents of a file.</p>
<h3> Architecture </h3>
<p> The command <code>uname -a</code> is use to get the architecture, <code>uname</code> is used to to print certain system information including kernel name, and the <code>-a</code> or <code>all</code> print all information </p>
<h3> Physical CPU </h3>
<p> To list the number of physical CPU's you can use <code>grep "physical id" /proc/cpuinfo | sort | uniq | wc -l</code></p>
<p> The last you can find the full command if you just google the subject line</p>
<h3> Virtual CPU </h3>
<p> To list how many virtual processors you have you can use <code>grep "^processor" /proc/cpuinfo | wc -l</code></p>
<h3> Free RAM and usage % </h3>
<p> Now, lets set the free RAM and it's percentage, to see the free RAM we have lets run <code>free -m</code> the <code>-m</code> flag makes the output in MB as we want.</p>
<p> We only want the Mem row,to do that we can <code>grep Mem</code>, the available memory is in the 4th column, to represent that we use <code>$4</code>, and to show just that value we will use <code>awk '{print $4}'</code>, if you don't know what <code><a href="https://www.geeksforgeeks.org/awk-command-unixlinux-examples/" target="_blank">awk</a></code> is, got study please!</p>
<p> So overall the command is <code>free -m | grep Mem | awk '{print $4}'</code></p>
<p> To get the total RAM memory we will do the same but instead of the column <code>$4</code> the total memory is in the column <code>$2</code></p>
<p> So it will be <code>free -m | grep Mem | awk '{print $2}'</code></p>
<p> To get the percentage of usage, we have to get the usage that is in the column<code>$3</code> and we will have to divide <code>$3/$2</code> and multiply by 100, <code>free -m | grep Mem | awk '{printf("%.2f"), $3/$2*100}'</code></p>
<h3> Free server space and usage %</h3>
<p> To see the server space you can run <code>df</code> that it will show you your disk space, to show it in MB we will use the flag <code>-m</code> and in GB we have to use 2 flags, <code>-B</code> to show the block size of the size we will ask, and <code>-g</code> that makes the size in GB. Our server it's the lines that start with <code>/dev/</code> so to get oly those lines we can <code>grep '^/dev/'</code>, the <code>^</code> means the beggining of the line so, every line that starts with ... . Those partitions(lines) are our home, our boot system and our dev, but actually you don't have acess to th boot partition because you can add or delete anything of that, so to take of only the line with boot we can use <code> grep -v '/boot$'</code>, the <code>-v</code>, is a flag to deselect the line, and the <code>$</code> is to select the end of the line, so it we are saying to take out the line that ends with ... . this time the print is a sum of the 3 lines so I created a variable (fdisk) and add the lines of the same column <code>awk '{fdisk += $4}</code>, to print the end result we have to add to the <code>awk</code> the following <code>END {print fdisk}</code>. So in the end we get <code>df -Bm | grep '^/dev/' | grep -v '/boot$' | awk '{fdisk += $4} END {print fdisk}'</code></p>
<p> To get the total disk space lets do the same but change the variable name to tdisk, the <code>-m</code> for <code>-Bg</code> and the column <code>$4</code> to <code>$2</code> so <code>df -Bg | grep '^/dev/' | grep -v '/boot$' | awk '{tdisk += $2} END {print tdisk}'</code></p>
<p> For the usage percent of the server is putting together what we did in the RAM but with the disk commands we did earlier, so <code>df -Bm | grep '^/dev/' | grep -v '/boot$' | awk '{fdisk += $3} {tdisk += $2} END {printf("%.2f"), fdisk/tdisk*100}'</code></p>
<h3> CPU usage %</h3>
<p> Now lets get the Cpu usage in percent, fortunately the command <code>top</code> already give us the cpu %, I'll use the flag <code>-b</code> to start in batch mode, that is usefull for sending output from top to toher programs or to a file, and I'll use the flag <code>-n numberx</code> that specify the max number of iterations or frames, top should produce before ending.</p>
<p> Because there is so many lines, lets grabe the one that matter <code>grep '^%Cpu'</code></p>
<p> To values we want are in the column <code>$2</code> so lets grab him in percentage with 1 decimal number <code>awk '{printf("%.1"), $2}'</code></p>
<p> In the end <code>top -bn1 | grep '^%Cpu' | awk '{printf("%.1f%%"), $2}'</code></p>
<h3> Last reboot</h3>
<p> For the the date and time of the last reboot, the command <code>who</code> it's the one, it prints out information about users who are currently loggend in, and with the flag <code>-b</code> shows the time of last system boot.</p>
<p> To get only the information we want we just selecting the columns that we need <code>$3 $4</code>, but to print both columns we need to add a <code>" "</code> between, so <code>awk '{print $3 " " $4}'</code>, so the final command will be <code>who -b | awk '{print $3 " " $4}'</code></p>
<h3> LVM active</h3>
<p> So, theres no command to run that says if the LVM is active or not so the way I did is, I run the command <code>lsblk</code> that will show the partitions, and I'm grabing just the lvm part <code>grep lvm</code> to check I'll do an if, so if I the column <code>$1</code> is different from NULL print an yes and exit, otherwise print a no <code>awk '{if ($1) {print "yes";exit;} else {print "no"}}'</code> </p>
<p> if you are excentric and want to add a little bit of life to your progrm you can use colors by adding <code>\033[0;32m"Your string"\033[0m</code> defining the string with <code>\033[0;32m</code> will make your string green you can check out other colours <code><a href="https://en.wikipedia.org/wiki/ANSI_escape_code" target="_blank">here</a></code>, when ending the string you must return to the original colour, the command to do so is <code>\033[0m</code>, by doing this, only your string will be coloured, leaving the rest with the original colour </p>
<p> The final command will be <code>lsblk | grep 'lvm' | awk '{if ($1) {printf "\033[0;32mYes\033[0m";exit} else {print "\033[0;031mNo\033[0m";exit;}}'</code></p>
<h3> Number of connections</h3>
<p> To get the number of connections you can use <code>ss</code>, ss is a tool that displays network socket related information, and we're going to use <code>-t</code> that lists only the tcp connections. To get the active ones, we going to use <code>grep ESTAB</code> and to print the number os lines we will use <code>wc</code> that prints a newline, word and byte counts for files, and if we use the flag <code>-l</code> just print the newline counts. </p>
<p> The final command is <code>ss -t | grep ESTAB | wc -l</code></p>
<h3> Number of users</h3>
<p> To see the number os users, we are going to run <code>who</code> again, and lets cut until the first space <code>cut -d " "</code>, the <code>-d</code> flag use delimiter instead of TAB for field delimite, and after lets use the flag <code>-f</code> to select only these fields and add 1, so its like <code? cut -d " " -f 1</code>.</p>
<p> Now lets use the command <code>sort</code> with the flag <code>-u</code> to output only the first of an equal run so it doesn't repeat, and that count the number of lines <code>wc -l</code>, so the command is <code>who | cut -d " " -f 1 | sort -u | wc -l</code></p>
<h3> IPv4 Adress & MAC (Media Access Control) </h3>
<p> Setting the IP of our server we will search the IP of the host, if you run <code>hostname</code> it displays the system's DNS name, and if you had the flag <code>-I</code> it display  all  network  addresses  of the host, so just use <code>hostname -I</code></p>
<p> To find the MAC (Media Access Control) we can use the <code>ip</code> that shows / manipulate routing, network devices, interfaces and tunnels, and with the object <code>link show</code> shows the network device. The lines we want are the ones that have ether, so just <code>grep ether</code> and to get the MAC we just need to print the column <code>$2</code>, in the end is just <code>ip link show | grep ether | awk '{print $2}'</code></p>
<h3> Numbers of sudo commands</h3>
<p> I tried so hard to do this with install netstat, but couldn't get to the right number, so just <code>sudo apt install net-tools</code></p>
<p> Now we have access to the command <code>journalctl</code> may be used to query the contents of the systemd(1) journal as
  written by systemd-journald.service(8), lets add <code>_COMM</code> to match for the script name <code>(sudo)</code>is added to the query. Lets grab just the commands thats what we want <code>grep COMMAND</code>, and lets cound the number of lines <code>wc -l</code> </p>
<p> The final command <code>journalctl _COMM=sudo | grep COMMAND | wc -l</code></p>
<p> Now lets use wall to print all the variables with the right text to it looks pretty.</p>

<h3>Installation</h3>
I have my folder with my vdi in: cd sgoinfre/born2beroot