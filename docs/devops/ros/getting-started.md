# Getting Started with ROS2

Robot Operating System 2 (ROS2) is the robotics framework upon which we base our software. 

Currently, we use **ROS2 Foxy Fitzroy** (released for Ubuntu 20.04 LTS).

## Installing ROS2
ROS2 is most well-supported on the Ubuntu Linux operating system, and most packages are developed with this OS in mind. While ROS2 is supported on Windows and to a limited extent on MacOS, our robots will be running Ubuntu, so it is best if we keep our development and deployment environments as similar as possible.

It is possible to work with Ubuntu on your Windows or Mac machines with x86 processors. ARM processors such as the M-series on Macs may cause complications. In most cases, you will end up with either a virtual or native version of Ubuntu on your system, and will follow the instructions for Ubuntu as the final step.

If this proves to be difficult for your system, computers are available in the lab for working with ROS2.

### ROS2 on Windows
#### Using Windows Subsystem for Linux 2 (WSL2)
Through Windows Subsystem for Linux 2 (WSL2), Ubuntu can be installed on a Windows machine without the need for dual booting. See the video below for more.

<div class="video-wrapper">
	<iframe width="560" height="315" src="https://www.youtube.com/embed/Zo9Ms2_U_4c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

#### Using Virtual Machine (VMs)
Virtual machines (VMs) allow for the simulation of other operating systems on your native operating system. The video below covers the installation of **ROS1 Melodic** through the use of a VM. Note that **this is not the current version** of Ubuntu or ROS that we are using.

<div class="video-wrapper">
	<iframe width="560" height="315" src="https://www.youtube.com/embed/e2nIShXX1iM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

#### Dual Booting
With most Windows machines, given enough storage space, it is possible to partition the disk and boot both Windows and Ubuntu natively on the same machine. However, this is also the most involved method of using Ubuntu with a Windows machine, and a backup of your files is highly recommended before attempting this.

### ROS2 on MacOS
Welcome to [the road not taken](https://www.poetryfoundation.org/poems/44272/the-road-not-taken). We have not yet investigated ROS2 on MacOS (Intel or M-series). If you're interested in paving this road, please let someone know!

### ROS2 on Linux Distributions other than Ubuntu
On Linux distributions other than Ubuntu, methods involving Docker or Podman containers will likely provide the highest level of integration with the system. Distrobox may be a useful tool for this scenario.

#### Distrobox
Install [Distrobox](https://github.com/89luca89/distrobox) and create an image with the current version of Ubuntu.

```
distrobox-create --image ubuntu:20.04 --name ub20
distrobox-enter ub20
```

### ROS2 on Ubuntu Linux
For Ubuntu, the instructions available on the [ROS2 documentation](https://docs.ros.org/en/foxy/Installation.html) should suffice for installation.




