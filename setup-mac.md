# GDV installation manual for macOS

In contrast to the Windows installation, Mac users can still use Virtualbox for their virtual machines. A transition to VMWare is possible, but this is only with a paid license. Other non-free VM-software for macOS is Parallels Desktop.

## Requirements
* **Mac hardware must be a 2010 or a newer model**, with Intel’s hardware support for memory management unit (MMU) virtualization, including Extended Page Tables (EPT) and Unrestricted Mode. You can check to see if your machine has this support by running the following command in a terminal: `sysctl kern.hv_support`. If your Mac supports the Hypervisor framework, the command prints `kern.hv_support: 1`
* **macOS must be version 10.13 or newer.** That is, Catalina, Mojave, or High Sierra. We recommend upgrading to the latest version of macOS. **NOTE**, once macOS 11 (Big Sur) is released, Catalina will not be supported anymore!
* At least 4 GB of RAM
* Git installed and configured

## Docker installation
* Install Docker Desktop on Mac CE edition from:
  * [https://docs.docker.com/docker-for-mac/install/](https://docs.docker.com/docker-for-mac/install/)
  * Make sure to select the stable version
* Once downloaded, mount the .dmg file, and drag the Docker application to your Applications folder.
* Open the Docker application and follow the on-screen instructions (elevated access will be asked)
* If you click on the Docker icon (located in the top status bar) and choose preferences, you can change the resources the Docker VM is using in the resource tab (maybe required to change in some lab sessions)

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


https://stackoverflow.com/questions/32834082/how-to-increase-docker-machine-memory-mac
