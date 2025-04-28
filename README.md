# linux-administration-lab-2---storage-management-solved
**TO GET THIS SOLUTION VISIT:** [Linux Administration Lab 2 – Storage Management Solved](https://www.ankitcodinghub.com/product/linux-administration-lab-2-storage-management-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119270&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Linux Administration Lab 2 - Storage Management Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Shortly after becoming the Linux system administrator for Dunder Mifflin, you receive a few ‘friendly’ emails from ‘management’ complaining that the internal file server’s disk is full. Instead of being able to jump to work on it, ‘management’ pulls you into a 2 hour meeting to discuss which project management approach should be used to handle the disaster, who will manage the project, etc., etc.

After putting up with the meeting for a total of 15 minutes, you silently step out, grab a spare 5 GB SATA hard drive, and plug it into the server. You then find some online resources

(https://www.google.com/search?q=lvm+tutorial&amp;ie=utf-8&amp;oe=utf-8) (this one being somewhat detailed

(http://web.archive.org/web/20190503083414/https://www.debian-

administration.org/article/410/A_simple_introduction_to_working_with_LVM) ), leading you through the process of setting up logical volumes on the new disk.

Device Mount Point Size Type Mount Options

/dev/centos/root / 4 GB xfs defaults

/dev/sda1 /boot 500 MB xfs defaults

/dev/new/home /home 4 GB xfs nodev

/dev/new/tmp /tmp 1 GB xfs nodev,nosuid,noexec

/dev/centos/swap None 512 MB swap

Why Logical Volumes?

Logical volumes mitigate many of the issues commonly faced with partitioning; e.g., the very limited number of partitions. The logical volume manager supports up to 2^32 logical volumes. Logical volumes not only alleviate some of the physical limitations of partitioning, but also give advanced features such as:

the ability to easily resize logical volumes (a typically painful and error-prone process with partitions)

the ability to take a snapshot of a logical volume and revert to it at any time (impossible with partitions alone)

the ability to move an entire logical volume from one physical disk to another (also impossible with partitions alone)

These are just some of the reasons to prefer logical volumes to partitions. Major downsides are the added complexity of setup and lack of redundancy. This is currently being addressed by the development of a kernel-based filesystem called btrfs. btrfs wraps the functionality of RAID and Logical Volumes directly into the filesystem itself.

Dunder Mifflin Network Topology &amp; Configuration

D-M has the following CentOS Linux servers:

1. A gateway (machine A) handles dhcp, ip_forwarding, and network/port address translation (nat/pat).

2. A file server (machine E) stores company files centrally.

3. An http server (machine B) hosts the corporate website.

4. An ftp server (machine C) updates prices and accepts batch orders.

5. A dns server (machine D) maps between domain names and IP addresses.

You will be given a unique number this semester. You need to substitute that number for each N in an IP address.

All your production machines have the same default root password of saclass. You are strongly encouraged to change this password to something more secure immediately.

The ssh (secure shell) service is running on all production machines so you can ssh in after connecting to the vpn.

Most of your production machines can be accessed from the vpn. The sole exception is machine E. To reach machine E, first ssh from the vpn into machine A. From machine A you can then ssh (pivot) into machine E.

Prerequisites

Submission Requirements

1. Please submit your notes on this lab. At a minimum they should list the commands you ran to add the storage, copy the existing contents, etc.

2. Your internal file server (machine E) should have two logical volumes named home (4GB) and tmp

(1GB). They should be contained in one volume group named new. That volume group should live

on one physical volume /dev/sdb on the new hard drive that has been added to the production virtual machine for you.

3. Any existing contents of /home, and /tmp should be moved to the logical volumes on the new disk and should match the structure of the old disk.

Hints

Import the physical volume (pvcreate)

Create a new volume group (vgcreate)

Create the logical volumes (lvcreate)

Make two xfs filesystems (mkfs)

Mount the new filesystems to temporary mount points (mount)

Copy the existing contents from the old disk to the new filesystems (cp or tar) Update /etc/fstab so the new filesystems are persistent across a reboot

At this point, have you actually freed up the disk blocks in the original filesystem? If not, how can you free this no-longer-used storage in the root filesystem? Make sure you don’t skip this last piece, as a full root filesystem was the reason you needed to add a new disk.

5113 Extra Challenge

Implement a mirrored or RAID5/6 volume to hold /home. You can use LVM or the MD Driver (https://linux.die.net/man/4/md) for this.
