# Dual boot Windows with- and without Hyper-V

**Make sure to enable Hyper-V first!**

You can dual boot your PC: one Windows installation with Hyper-V enabled, and one not. This can be done with your current installation. **Use at your own risk**: you will adapt your boot sequence in order to activate this option. To do so, follow these steps:

* Run a powershell prompt with elevated rights (right click on the Windows Logo, and choose Windows Powershell (Admin))
* Run following command: *bcdedit /copy {current} /d "No Hyper-V"*
* Copy the ID you get as output and run the following command:  *bcdedit /set {YOUR_ID_HERE} hypervisorlaunchtype off*

  ![bcedit](img/bcedit.png)

* Restart your computer by holding shift en pressing the restart button. In the boot menu, choose "Use another operating system" and than you can choose between your normal installation (with Hyper-V active), or the No Hyper-V version.

From now on, every time you boot your PC, you will need to choose which version you want to use. After 60s, the default version will be booted.
