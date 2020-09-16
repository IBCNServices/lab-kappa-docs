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

## Zoom installation

Zoom will be used for presentations during labs and to help students remotely. Because the Zoom web client does not support remote control, you need to install the Zoom desktop app.

```bash
sudo snap install zoom-client
```

When you start Zoom, login through "SSO", use the `ugent-be` domain and use your UGent email address. For more instructions (only in Dutch) see [Activatie van Zoom door studenten](https://ufora.ugent.be/d2l/le/content/9061/viewContent/463766/View).

## Microsoft Teams installation

Install Microsoft Teams using the DEB [from their website](https://www.microsoft.com/en-us/microsoft-365/microsoft-teams/download-app).

> *Note: Installing the file straight from the browser might fail. In this case, first download it to a directory and then open it using Files.*

## Docker installation

Install Docker from the Ubuntu repository

```shell
sudo apt install docker.io
sudo groupadd docker
sudo usermod -aG docker $USER
```

After this, **restart your computer**.

## Visual Studio Code

Install VSCode using the snap.

```bash
sudo snap install code --classic
```

## Next steps

Please follow the specific installation manuals for the courses you attend.

* [Ubuntu installation guide - GDV](./gdv-setup-ubuntu.md)
* [Ubuntu installation guide - DevOps](./devops-setup-ubuntu.md)

> Are you having problems during the installation? Please create an issue in [the docs repository](https://github.ugent.be/GDV/docs/issues). We speak both Dutch and English.
