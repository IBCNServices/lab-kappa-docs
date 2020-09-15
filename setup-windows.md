# GDV & DevOps installation manual for Windows

These courses use Docker Desktop on Windows. This is the recommended and most powerful way to run Docker on Windows, but it requires Hyper-V; the Microsoft virtualization hypervisor. As of writing this, VirtualBox still does not fully support Hyper-V, so **VirtualBox will not work anymore** after running these instructions. Other courses of Industrieel Ingenieur Informatica will use VMWare to run virtual machines, because that supports Hyper-V.

Older tutorials might mention *Docker Toolbox* for Windows. However, this does not support all the features required for GDV and DevOps so **you cannot use Docker Toolbox**.

> *Note: If you absolutely need to use VirtualBox, it is possible to create a dualboot of Windows 10 with Hyper-V enabled and Windows 10 without Hyper-V. **We do not recommend this approach** but we can provide some information if you are interested.*

You can download VMWare from [https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) by clicking on "Try Workstation 15.5 Player for Windows". Installing VMWare is not required for these courses.

![VMWare](img/vmware.png)

## Requirements

* Windows 10 - version 2004: Download through [https://www.microsoft.com/nl-nl/software-download/windows10](https://www.microsoft.com/nl-nl/software-download/windows10) and follow to on-screen instructions
  * You can check your version through settings > system > about > "Windows Specifications"

  ![foto](img/about.png)

* Enable some Windows modules
  * Go to control panel (configuratiescherm) > Program and Features
  * On the left side you should see an option to "Turn Windows features on or off"
  
  ![control panel](img/controlpanel.png)

* Select the following features:
  * Containers
  * Hyper-V
  * Virtual Machine Platform
  * Windows Hypervisor Platform
  * Windows Subsystem for Linux
* Click on "OK" and these features will be installed on your PC. Some reboots will be required during the installation process.
* Git must be installed in configured on your system

## Docker installation

* Install Docker for Windows CE edition from:
  * [https://docs.docker.com/docker-for-windows/install-windows-home/](https://docs.docker.com/docker-for-windows/install-windows-home/) for Windows 10 Home users
  * [https://docs.docker.com/docker-for-windows/install/](https://docs.docker.com/docker-for-windows/install/) for Windows 10 Enterprise or Pro users
  * Make sure to select the stable version
* Follow to on-screen instructions
  * Make sure to enable the following option (already enabled by default): "Use the WSL 2 based engine"
  * Start Docker after the installation.

## Visual Studio Code

* Download and install Visual Studio Code from [https://code.visualstudio.com/](https://code.visualstudio.com/)
  * Enable the option to add "code" to PATH

## Next steps

Please follow the specific installation manuals for the courses you attend.

* [Windows installation guide - GDV](./gdv-setup-windows.md)
* [Windows installation guide - DevOps](./devops-setup-windows.md)

> Are you having problems during the installation? Please create an issue in [the docs repository](https://github.ugent.be/GDV/docs/issues). We speak both Dutch and English.
