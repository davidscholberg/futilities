# Futilities

This project holds some small utility scripts that I've written as well a simple script for installing them into `~/.local/bin` so that they can be called from anywhere.

All scripts managed by this repo are copied to `~/.local/bin` with file permissions set to `555` (read-only and executable). I think that copying the files is better than symlinking for the following reasons:

* Copying the files allows you to make local changes inside this repo without having them go "live" right away.
* Setting the copied files to read-only is a barrier for other programs attempting to make changes to a managed script.

### Usage

To install the scripts here to your home directory, just clone this repo and run the install script:

```bash
git clone git@github.com:davidscholberg/futilities.git && \
cd futilities && \
./futilize
```
