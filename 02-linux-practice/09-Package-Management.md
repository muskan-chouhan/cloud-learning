# Package Management

## apt  >like a playstore

APT (Advanced Package Tool) is the package manager for Ubuntu/Debian.

It is used to:

- Install software
- Remove software
- Update package information
- Upgrade installed software
- Search packages

Examples:
apt
apt --help


Real World: Used by Linux administrators and DevOps engineers to manage software on servers.

## apt update = package list update karta hai.

Updates the local package list from online repositories.

Syntax: sudo apt update


Important:

- ❌ Does NOT update installed software.
- ✅ Downloads the latest package information.

Real World: Run before installing or upgrading packages to get the latest package list.

# apt upgrade
installed software ko update karta hai. 

## apt install

Installs a software package.

Syntax: sudo apt install package_name


Examples:
sudo apt install nginx
sudo apt install git
sudo apt install zip


Process:
1. Checks package list.
2. Checks dependencies.
3. Downloads package.
4. Installs package.

## apt remove

Removes an installed package.

Syntax: sudo apt remove package_name


Example: sudo apt remove nginx

---

## apt purge

Removes the package along with its configuration files.

Syntax: sudo apt purge package_name

Difference:

- remove → Software only
- purge → Software + configuration files

Real World:
- remove → Temporary uninstall
- purge → Complete cleanup

# apt autoremove = Kabhi package remove karte ho to kuch dependency packages bach jaate hain.
# apt list --installed = Installed packages dekhna  /apt list --installed | grep nginx
# apt show = Package ki details / apt show nginx


## apt search

Searches for available software packages.

Syntax: apt search package_name
`

Example:

apt search nginx
apt search docker


Real World: Used when you don't know the exact package name.

# apt show

Example:

apt show nginx