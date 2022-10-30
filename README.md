# ansible-role-java
Ansible role to install Java

## Role Variables

### java_version (optional)

Acceptable Java versions for RHEL7-based OS:
- 1.6.0
- 1.7.0
- 1.8.0
- 11

Acceptable Java versions for RHEL8-based and RHEL9-based OS:
- 1.8.0
- 11
- 17

```
java_version: 11 # default
```
### java_install_jdk (optional)

Install JDK or JRE only

```
java_install_jdk: no # default
```

### java_package (optional)

You can pin the exact Java package version by setting this variable

```
java_package: java-17-openjdk-17.0.0.0.26
```

## Example playbook

Install JDK 1.8.0 (java-1.8.0-openjdk-devel package)

```
---
- name: Install Java
  hosts: all
  roles:
    - role: ansible-role-java
      java_version: "1.8.0"
      java_install_jdk: yes
```