# General installation manual for macOS

In contrast to the Windows installation, Mac users can still use VirtualBox for their virtual machines. A transition to VMWare is possible, but this is only with a paid license. Other non-free VM-software for macOS is Parallels Desktop.

## Requirements

* **Mac hardware must be a 2010 or a newer model**, with Intel’s hardware support for memory management unit (MMU) virtualization, including Extended Page Tables (EPT) and Unrestricted Mode. You can check to see if your machine has this support by running the following command in a terminal: `sysctl kern.hv_support`. If your Mac supports the Hypervisor framework, the command prints `kern.hv_support: 1`
* **macOS must be version 10.13 or newer.** That is, Catalina, Mojave, or High Sierra. We recommend upgrading to the latest version of macOS. **NOTE**, once macOS 11 (Big Sur) is released, Catalina will not be supported anymore!
* At least 8 GB of RAM

## Git installation

1. Install git using the one of the options provided on [https://git-scm.com/download/mac](https://git-scm.com/download/mac). **Use the default settings of the git installer.**
2. Open your terminal and configure your username and email using the following commands.

```bash
# Run this inside the terminal with the correct email and name
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

## Zoom installation

Zoom will be used for presentations during labs and to help students remotely. Because the Zoom web client does not support remote control, you need to install the Zoom desktop app.

* Download the Zoom Client for Meetings from [https://zoom.us/download](https://zoom.us/download)
  * Follow the on-screen instructions
  * Login through "SSO"
    * Instructions can be found on [https://ufora.ugent.be/d2l/le/content/9061/viewContent/463766/View](https://ufora.ugent.be/d2l/le/content/9061/viewContent/463766/View)
    * *Only available in Dutch*

## Microsoft Teams installation

* Download the Microsoft Teams application from [https://www.microsoft.com/nl-be/microsoft-365/microsoft-teams/download-app](https://www.microsoft.com/nl-be/microsoft-365/microsoft-teams/download-app)
  * Follow the on-screen instructions
  * Use your UGent-account to login

## Docker installation

1. Install Docker Desktop on Mac CE edition from:
   * [https://docs.docker.com/docker-for-mac/install/](https://docs.docker.com/docker-for-mac/install/)
   * Make sure to select the stable version
1. Once downloaded, mount the .dmg file, and drag the Docker application to your Applications folder.
1. Open the Docker application and follow the on-screen instructions (elevated access will be asked)
1. If you click on the Docker icon (located in the top status bar) and choose preferences, you can change the resources the Docker VM is using in the resource tab (maybe required to change in some lab sessions)

## Visual Studio Code

* Download and install Visual Studio Code from [https://code.visualstudio.com/](https://code.visualstudio.com/)
  * Enable the option to add "code" to PATH

## Next steps

Please follow the specific installation manuals for the courses you attend.

* [macOS installation guide - GDV](./gdv-setup-mac.md)
* [macOS installation guide - DevOps](./devops-setup-mac.md)

> Are you having problems during the installation? Please create an issue in [the docs repository](https://github.ugent.be/GDV/docs/issues). We speak both Dutch and English.
