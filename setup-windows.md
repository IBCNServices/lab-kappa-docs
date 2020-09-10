# GDV installation manual for Windows

Windows users will have to enable Hyper-V in order to use to full power of Docker. **Therefore VirtualBox will not work anymore**. VMWare will be used for virtual machines in the future. In case you still want to use VirtualBox, you have two options:

* You have enough RAM: you can use Docker toolbox, but this is at own risk. We will provide minimal support for this (but you can always ask us a question in case of problems). Make sure to search for "how to enlarge ram memory for Docker toolbox".
  * See [https://github.com/crops/docker-win-mac-docs/wiki/Windows-Instructions-(Docker-Toolbox)](https://github.com/crops/docker-win-mac-docs/wiki/Windows-Instructions-(Docker-Toolbox))
* You can enable a dual boot to choose between a Windows 10 with Hyper-V active and one without Hyper-V. This approach is not recommended, but if you want to, you can ask the assistants for more information.

VMWare can be downloaded from [https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) by clicking on "Try Workstation 15.5 Player for Windows".

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
* Start Visual Studio Code
* Navigate to Extensions

  ![extensions](img/extensions.png)

* Search the Python extension and install

  ![python](img/python_extension.png)

* Search for the Remote containers extension and install
  
  ![remote_containers](img/remote_containers.png)

You are now ready to start coding using Visual Studio Code and Docker!
