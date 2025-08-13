# Linux File and Folder Permissions:
  - Ensure you have developer group and dev1 user
  - Create a folder with ubuntu user and also create some files in it
  - Change owner from ubuntu to dev1 for all files and folders in it
  - change group from ubuntu to developer for all files and folders in it
  - Now create a file called as say hello.sh with following content
      - #!/bin/bash
echo hello
  - This file will have permissions of 664
  - give execute permissions to owner, group and others
      - `**chmod +x sayhello.sh**`
  - file permisions
     - changing permissions
     - changing ownerships
     - changing groups
 - download maven tar file from [Refer Here](u can use the linunk form Website)
     - cd /tmp
     - wget https://dlcdn.apache.org/maven/maven-3/3.9.8/binaries/apache-maven-3.9.8-bin.tar.gz
     - untar the file and copy into /opt folder
     - tar xvzf apache-maven-3.9.8-bin.tar.gz
     - ls -l
     - sudo mv apache-maven-3.9.8 /opt/
     - ls -l /opt
 - Lets do the same for openjdk 21 [Refer Here](https://jdk.java.net/archive/)

## Next Topics

 - Environmental variable PATH
 - Installing applications
    - download code, compile code and run on a system (any distribution)
    - download binary, extract and configure
    - packages
      - .deb (debian)
      - .rpm (redhat)
   - Package Managers
      - apt (debian)
      - yum | dnf (redhat)
      - snap (any distribution)