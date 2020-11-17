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

Check this [file](docker_on_windows.md).

## How can I change the location of docker images when using WSL2 with Windows 10?

Check this [Stack Overflow post](https://stackoverflow.com/questions/62441307/how-can-i-change-the-location-of-docker-images-when-using-wsl2-with-windows-10-h).
