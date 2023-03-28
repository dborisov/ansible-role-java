# ansible-role-java
Ansible role to install java

# Supported Platforms
- RedHat 8
- RedHat 9

# Requirements
- The role supports the installation of java versions `8`, `11` and `17`. Default is `11`.

# Example Variables
```
java_version: "17"
java_type: jdk
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