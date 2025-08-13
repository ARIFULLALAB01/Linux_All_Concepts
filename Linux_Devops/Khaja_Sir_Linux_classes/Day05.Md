# Linux Software Installations
  - Any application is an executable
  - Installing sofware is all about ensuring executables are present in the system.
  - For doing this we have 3 approaches
     - **From Source code**
     - **From Binaries**
     - **From packages**
  - To simplify this we have package managers
## From binaries
   - We can try installing
     - openjdk
     - maven [Refer Here](https://maven.apache.org/download.cgi)
     - tomcat
## Linux Packages
  - In the linux world we have two popular packages
      - debian package (.deb)
         - sudo dpkg
      - redhad package (.rpm)
         - sudo rpm

## Applications on Linux
  - Standalone
  - Service/Daemons:
     - This is an application which runs in the background
     - This should start automatically when the system starts (Enable)
     - To configure services we will have to deal with service files and systemctl commands