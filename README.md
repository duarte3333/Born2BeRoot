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
<h2> What is Operating System </h2>
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
<h2 id="What is a Virtual Machine">Debian vs CentOS</h2>
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
<h2 id="Set the basic up">What is APT?</h2>
<p>APT stands for Advanced Packaging Tool. It is an open-source tool, which means you can use it without the need to pay anything. APT is designed to handle software installation and removal.</p>
<p>APT was part of Debian’s .deb package; however, it was updated to work with the RPM Package Manager. If you have used APT before, you would have noticed that it is a command-line tool. This means you need to use commands to work with it with no visual reference from a graphical interface(the initial plan was to include a graphical interface, but the idea was later dropped).</p>
<p>If you use the apt command, it will not only download and install the required dependencies for the said package. As a user, you do not have to worry about the package dependencies.</p>
<h2 id="Set the basic up">What is Aptitude?</h2>
Aptitude is also an advanced packaging tool. However, it is a front-end tool that gives users access to the user-interface to access functionality. This means that you can use Aptitude to install and remove packages using it. 
<h2 id="Set the basic up">Differences between APT and Aptitude?</h2>
Apt-get being a lower level package manager is restricted only to command line, while Aptitude being a higher-level tool has a default text-only interactive interface along with option of command-line operation by entering required commands.
<h2> What is AppArmor </h2>
AppArmor ("Application Armor") is a Linux kernel security module that supplements the standard Linux user and group based permissions to confine programs to a limited set of resources. AppArmor can be configured for any application to reduce its potential attack surface and provide greater in-depth defense. It is configured through profiles tuned to allow the access needed by a specific program or container, such as Linux capabilities, network access, file permissions, etc. Each profile can be run in either enforcing mode, which blocks access to disallowed resources, or complain mode, which only reports violations.

<h2 id="Set the basic up">Set the basic up</h2>
<p> Login as root: <code>su -</code></p>
<p> Update & Upgrade: <code> apt update</code> and <code> apt upgrade</code></p>
<p> Install sudo: <code> apt install sudo</code></p>
<h3> What is sudo? </h3>
Sudo (sometimes considered as short for Super-user do) is a program designed to let system administrators allow some users to execute some commands as root (or another user). The basic philosophy is to give as few privileges as possible but still allow people to get their work done. Sudo is also an effective way to log who ran which command and when.
<h3> What is a Sudo group? </h3>
A sudo group is a group of superusers that have privileged access to root commands.
<p> Add user to sudo group: <code>adduser dsa-mora sudo</code></p>
<p> Add user to user42 group(should be done in root): <code>adduser dsa-mora user42</code></p>
<p> Delete a user: <code>deluser newuser</code>
<p> If signed in as another non-root user with sudo privileges: <code>sudo deluser newuser</code>
<p> To check if your user is in the sudo group <code>getent group sudo</code></p>
<p> File where I change the number of days before the password expire, minimum number of days allowed before the modification of a password and the number of days the user has to receive a warning message before their password expires: <code>sudo nano /etc/login.defs</code></p>
<p> How to find the name and the version of the OS in linux: <code>cat /etc/os-release</code> 


<h2>SSH</h2>
