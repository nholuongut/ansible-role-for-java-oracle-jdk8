# Ansible Role: Installs Java 8 JDK or Server JRE
![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

## Table of Contents

1. [Requirements][Requirements]
2. [Installation][Installation]
3. [Role Variables][Role Variables]
4. [Dependencies][Dependencies]
5. [Example Playbook][Example Playbook]
6. [Licensing][Licensing]
7. [Author Information][Author Information]
8. [Support][Support]
9. [Contributing][Contributing]
10. [Donation][Donation]

## Requirements

None.

## Installation

    ansible-galaxy install kami911.java-oracle-jdk8

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    force_java_install: False

Force to install Java on already installed system.

    java_installer_force_overwrite: False

Force to overwrite Java installer.

    java_installer_keep: False

Do not delete Java installer.

    java_installer_local: False

Install local (form Ansible host) JDK/Server JRE instead of downloading on target machine.

    java_type: jdk

Type of Java installer - JDK is: jdk, and Server JRE is: server-jre

    java_version: 8

Java major version.

    java_update: 201

Java minor version.

    java_build: "09"

Java micro version.

    java_platform: linux-x64

Java platform to install.

    java_bins: [ 'javah', 'javap', 'jmap', 'extcheck', 'pack200', 'jrunscript', 'jinfo', 'jcontrol', 'jmc', 'keytool', 'schemagen', 'jjs', 'jvisualvm', 'policytool', 'rmid', 'wsgen', 'javaws', 'javadoc

Update alternatives on these binaries.

    java_bins_priority: 9

Alternatives priority on these binaries.

    java_usr_folder: /usr/java

Location of installed Java home.

    java_latest_folder: /usr/java/latest

Where to link the latest folder.

    java_download_base_url: http://download.oracle.com/otn-pub/java/jdk

Download link of Java installers.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - java-oracle-jdk8

## Licensing

The lactransformer application and documantations are licensed under the terms of
the MIT / BSD, you will find a copy of this license in the
[LICENSE](LICENSE) file included in the source package.


### Using as a submudule of an AWX playbook

#### Add as a submodule

```
git submodule add --force git@github.com:nholuongut/ansible-role-for-java-oracle-jdk8.git roles/java-oracle-jdk8
```

#### Update as sumodule

Update only this submodule

```
git submodule update --remote roles/java-oracle-jdk8/
```

Update all submodules:

```
git submodule foreach git pull origin master
```

## Contributing

There are many ways to contribute to ansible-role-java-oracle-jdk8 -- whether it be sending patches,
testing, reporting bugs, or reviewing and updating the documentation. Every
contribution is appreciated!

Please continue reading in the [contributing chapter](CONTRIBUTING.md).

### Fork me on Github

SSH:

    git@github.com:nholuongut/ansible-role-for-java-oracle-jdk8.git

HTTPS:

    https://git@github.com:nholuongut/ansible-role-for-java-oracle-jdk8

Add a new remote `upstream` with this repository as value.

```
git remote add upstream https://github.com/nholuongut/ansible-role-for-java-oracle-jdk8.git
```

You can pull updates to your fork's master branch:

```
git fetch --all
git pull upstream HEAD
```

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟