# General installation manual for Ubuntu

> *Note: we only support Ubuntu 20.04.* You can use another version or distribution, but we cannot guarantee it will work.

## Git installation

First, install git using the package manager.

```bash
sudo apt install git
```

After installation, configure git with your username.

```bash
# Run this with the correct email and name
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

## Docker installation

Install Docker from the Ubuntu repository

```shell
sudo apt install docker.io docker-compose
sudo groupadd docker
sudo usermod -aG docker $USER
```

After this, **restart your computer**.

## Visual Studio Code

1. Install VSCode using the snap.

   ```bash
   sudo snap install code --classic
   ```

1. Install the vscode "Remote - Containers" extension from Microsoft.

   ```bash
   # Note: you might need to reboot before the `vscode` command becomes available.
   code --install-extension ms-vscode-remote.remote-containers
   ```

1. Now you are ready to start the labs! Note that each lab might have additional installation instructions. Make sure to complete those before that specific lab starts.

> Are you having problems during the installation? Please create an issue in [the docs repository](https://github.com/IBCNServices/lab-kappa-docs/issues). We speak both Dutch and English.
