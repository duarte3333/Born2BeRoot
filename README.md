# Born2BeRoot

<h1>Born2beRoot</h1>
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

<h2 id="What is a Virtual Machine">Virtual Machine vs Virtual Hard Disk?</h2>
<p>The Virtual Machine configuration stores the settings of the system.  This includes 
the quantity of CPUs, memory, hard disks, SCSI controllers, etc. On the other hand, the Virtual Hard 
Disks contain the actual data (boot volumes, data volumes, etc.)</p>
<p>Is possible to save a VM and VHD on a USB flash memory device, since they are independent 
of the Hardware thanks to the hypervisor. So a VHD is type of disk drive that has similar 
functionalities as a typical hard drive but is accessed, managed and installed 
on a virtual machine infrastructure, such as Hyper-V, VMWare Workstation, etc...</p>


<h2 id="Set the basic up">Set the basic up</h2>
<p> Login as root: <code>su -</code></p>
<p> Update & Upgrade: <code> apt update</code> and <code> apt upgrade</code></p>
<p> Install sudo: <code> apt install sudo</code></p>
<p> Add user to sudo group: <code>sudo usermod -aG sudo bmiguel-</code></p>
<p> <code>-a</code> is a shortcut for --append: It means append the group to the list of groups the user belongs to!</p>
<p> <code>-G</code> is a shortcut for --groups: It tells usermod that the next argument is a group. Note that you need to use a capital -G here because we don’t want to modify the user’s primary group but the list of supplemental groups the user belongs to.</p>
<p> To check if your user is in the sudo group <code>getent group sudo</code></p>
<p> Leave root to your user now <code>su - bmiguel-</code></p>
