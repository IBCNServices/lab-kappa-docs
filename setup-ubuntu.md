# General installation manual for Ubuntu

> *Note: we only support Ubuntu 20.04.* You can use another version or distribution, but we cannot guarantee it will work.

1. Install the GCC toolchain and build dependencies.

    ```bash
    sudo apt install git
    ```

1. Configure git with your username.

    ```bash
    # Run this with the correct email and name
    git config --global user.email "you@example.com"
    git config --global user.name "Your Name"
    ```

1. Install VSCode

    ```bash
    sudo snap install code --classic
    ```

1. Install Zoom

    ```bash
    sudo snap install zoom-client
    ```

   * Follow the on-screen instructions
     * Login through "SSO"
       * Instructions can be found on [https://ufora.ugent.be/d2l/le/content/9061/viewContent/463766/View](https://ufora.ugent.be/d2l/le/content/9061/viewContent/463766/View)
       * *Only availabe in Dutch*
1. Install Microsoft Teams using the DEB [from their website](https://www.microsoft.com/en-us/microsoft-365/microsoft-teams/download-app).

   > *Note: Installing the file straight from the browser might fail. In this case, first download it to a directory and then open it using Files.*

## Next steps

Please follow the specific installation manuals for the courses you attend.

* [Ubuntu installation guide - GDV](./gdv-setup-ubuntu.md)
* [Ubuntu installation guide - DevOps](./devops-setup-ubuntu.md)

> Are you having problems during the installation? Please create an issue in [the docs repository](https://github.ugent.be/GDV/docs/issues). We speak both Dutch and English.
