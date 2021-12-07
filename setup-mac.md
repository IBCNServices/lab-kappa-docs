# General installation manual for macOS

## Requirements

* **Mac hardware must be a 2010 or a newer model**, with Intel’s hardware support for memory management unit (MMU) virtualization, including Extended Page Tables (EPT) and Unrestricted Mode. You can check to see if your machine has this support by running the following command in a terminal: `sysctl kern.hv_support`. If your Mac supports the Hypervisor framework, the command prints `kern.hv_support: 1`
* **macOS must be version 10.14 or newer.** That is Mojave, High Sierra or Big Sur. We recommend upgrading to the latest version of macOS. **NOTE**, please do not install the newest macOs version (Monterey) before our approval (we will evaluate it asap once it is released)
* **M1 Macs are not supported**.
* At least 8 GB of RAM

## Git installation

1. Install git using the one of the options provided on [https://git-scm.com/download/mac](https://git-scm.com/download/mac). **Use the default settings of the git installer.**
2. Open your terminal and configure your username and email using the following commands.

```bash
# Run this inside the terminal with the correct email and name
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

## Docker installation

1. Install Docker Desktop for macOS from:
   * [https://docs.docker.com/desktop/mac/install/](https://docs.docker.com/desktop/mac/install/)
   * Make sure to select the stable version
1. Once downloaded, mount the .dmg file, and drag the Docker application to your Applications folder.
1. Open the Docker application and follow the on-screen instructions (elevated access will be asked)
1. If you click on the Docker icon (located in the top status bar) and choose preferences, you can change the resources the Docker VM is using in the resource tab (maybe required to change in some lab sessions)

## Visual Studio Code

1. Download and install Visual Studio Code from [https://code.visualstudio.com/](https://code.visualstudio.com/)
   * Enable the option to add "code" to PATH
1. Install the vscode "Remote - Containers" extension from Microsoft.

   ```bash
   # Note: you might need to reboot before the `vscode` command becomes available.
   code --install-extension ms-vscode-remote.remote-containers
   ```

1. Now you are ready to start the lab!

## [Optional] VMWare installation

If you experience trouble installing Docker, you can try our Virtual Machine. You can install VMWare for free using the following instructions.

Install [VMware Fusion Player](https://www.vmware.com/be/products/fusion.html). As a student, you can use it for free by clicking on "Get a Free 'Personal Use' License". During registration, you might get stuck on the "Activate Your My VMware Account" step. If this is the case, log out from the website by surfing to [https://my.vmware.com/web/vmware/logout](https://my.vmware.com/web/vmware/logout), refresh all VMware pages and try to register again for the personal use license.

> Are you having problems during the installation? Please create an issue in [the docs repository](https://github.com/IBCNServices/lab-kappa-docs/issues). We speak both Dutch and English.
