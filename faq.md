# Frequently asked questions

## Can't open notebook: "Unable to start session for kernel Python ..."
Check the version of the `traitlets` library inside the remote container.
```
$ pip freeze | grep traitlets
```
If the version is between 4.3.3 and 5.0.4 try to reinstall the library. Close all notebooks before reinstalling the library.
```
python -m pip install 'traitlets==5.0.4' --force-reinstall
```

## Docker problems on Windows 10 Home

* Make sure that you have Windows 10 - 2004 installed, and that all the windows features as requested
* Quit Docker desktop
* Install all windows updates (if available)
* Quit visual studio code
* Start Docker desktop as administrator (righ-click > Run as administrator)
  * If docker is hanging on startup, follow these steps:
    * Stop Docker Desktop
    * Open Powershell and execute these commands:
      * stop WSL (`wsl --shutdown`)
      * unregister the docker-desktop distro (which contains binaries, but no data) with `wsl --unregister docker-desktop`
    * Restart Docker Desktop as administrator

Also make sure that no Docker Toolbox installation is still on your system.
