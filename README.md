<div align="center">
  <h1 align="center">blend</h1>
  <p align="center">A package manager for blendOS</p>
  <p align="center"><b>rs2009 here. I've used a README from a Vanilla OS repository (almost) as a template, and accidentally included a paragraph from it. I've written this package manager from scratch (none of the files aside from the README in this repository have any code from any other repository on GitHub, other than anything developed by me).</b></p>
</div>
### Help
```
Usage:
  blend [command] [options] [arguments]

Version: 1.0.4

blend is a package manager for blendOS, which includes support for Arch, Ubuntu and Fedora packages.

default distro: arch (default container's name is the same as that of the default distro)

Here's a list of the supported distros:
1. arch
2. fedora-rawhide
3. ubuntu-22.04
4. ubuntu-22.10
(debian support is coming soon)

You can use any of these distros by passing the option --distro=[NAME OF THE DISTRO].

You can even install a supported desktop environment in a blend container (run `blend install-de [DESKTOP ENVIRONMENT NAME]` to install your favorite desktop environment).

However, this feature is still somewhat experimental, and some apps might be buggy.

Here's a list of the supported desktop environments:
1. gnome
2. mate
(support for many more DEs is coming soon)

arch also supports AUR packages, for an extremely large app catalog.

available commands:
  help                  Show this help message and exit.
  version               Show version information and exit.
  enter                 Enter the container shell.
  export                Export the desktop entry for an installed blend.
  unexport              Unexport the desktop entry for a blend.
  install               Install packages inside a container.
  install-de            Install a desktop environment inside a container. (EXPERIMENTAL)
  remove                Remove packages inside a managed container.
  create-container      Create a container managed by blend.
  remove-container      Remove a container managed by blend.
  list-containers       List all the containers managed by blend.
  start-containers      Start all the container managed by blend.
  sync                  Sync list of available packages from repository.
  search                Search for packages in a managed container.
  show                  Show details about a package.
  update                Update all the packages in a managed container.

options for commands:
  -cn CONTAINER NAME, --container-name CONTAINER NAME
                        set the container name (the default is the name of the distro)
  -d DISTRO, --distro DISTRO
                        set the distro name (supported: arch fedora-rawhide ubuntu-22.04 ubuntu-22.10; default is arch)
  -y, --noconfirm       assume yes for all questions
  -v, --version         show version information and exit

options:
  -h, --help  show this help message and exit

Made with ❤ by Rudra Saraswat.
```
