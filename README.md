# ansible-role-java
Ansible role to install java

# Supported Platforms
- RedHat 8
- RedHat 9

# Requirements
- The role supports installation of any java version available on the platform. Headless JRE 11 will be installed by default.

# Example Variables

## Install JDK 21

```
java_version: "21"
java_type: jdk
```

## Install full JRE 8

```
java_version: "8"
java_type: jre
```

# Example Playbook
```
---
- hosts: java
  roles:
    - role: dborisov.java
```

# Role Variables
Please see `defaults/main.yml`

# Dependencies
None

# License
MIT