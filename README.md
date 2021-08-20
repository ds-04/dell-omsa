# dell-omsa

Ansible role to install Dell OpenManage Server Administrator on Centos/RHEL (7/8) and Debian (10/11).

- please see distro specific notes below.
- the role will not do anything to your firewall, you need to enable web access if you want it to see OMSA web.
- systemd service is setup by the role and started/enabled.

# RHEL/Centos (7/8)

The role will download the bootstrap script and setup OMSA.

(https://linux.dell.com/repo/hardware/dsu/bootstrap.cgi)


# Debian (10/11)

Firstly please see https://linux.dell.com/repo/community/openmanage/

Note Debian 10/11 is **NOT officially supported**, but this role has been created to install OMSA - **use at own risk!**

- It will install Ubuntu libraries needed. See defaults/main.yml file.
- It is hardcoded to **930 'bionic'** at the moment (see URL above).
- It will install the gpg key, again though, much of this is currently hardcoded.


# Ubuntu / openSUSE etc.

Out of scope here, please submit a pull request if you want it.



