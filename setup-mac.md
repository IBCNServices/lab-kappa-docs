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

Download the Zoom Client for Meetings from [https://zoom.us/download](https://zoom.us/download) and install it.

When you start Zoom, login through "SSO", use the `ugent-be` domain and use your UGent email address. The first time you login, an account will be made for you automatically. For more instructions (only in Dutch) see [Zoom handleiding studenten](https://web.microsoftstream.com/video/2096e73b-f69b-4c84-b2da-a27e06da6d34?referrer=https:%2F%2Fonderwijstips.ugent.be%2Fnl%2Ftips%2Fzoom%2F) (login using your UGent email).

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

1. Download and install Visual Studio Code from [https://code.visualstudio.com/](https://code.visualstudio.com/)
   * Enable the option to add "code" to PATH
1. Install the vscode "Remote - Containers" extension from Microsoft.

   ```bash
   # Note: you might need to reboot before the `vscode` command becomes available.
   code --install-extension ms-vscode-remote.remote-containers
   ```

1. Now you are ready to start the labs! Note that each lab might have additional installation instructions. Make sure to complete those before that specific lab starts.

> Are you having problems during the installation? Please create an issue in [the docs repository](https://github.ugent.be/GDV/docs/issues). We speak both Dutch and English.
