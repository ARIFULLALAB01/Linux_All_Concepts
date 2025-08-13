# Process
  - OS create process to run application
  - Each process will have unique pid
  - on linux we use
      - ps
      - kill
      - top
      - htop
## Applications and Services in Linux
 - Application execution is generally on-demand, i.e. process gets created on user action (execution or double click)
 - There are certain processes which we want to run all the time
    - database
    - web
    - ssh
 - The above applications are referred as services or daemons as they run in the background
## Services
 - Terminology
     - state: running, stopped/exited
     - enabled/disabled
 - Linux we have two service initialization systems
    - sysvinit
         - older approach based on unix
         - we create scripts
    -systemd
      -modern where we create unit files
### Difference between ** sysvinit VS Systemd** -- Reseacrh in ChatGPT For This

 - **In summary, while SysVinit is known for its simplicity and compatibility, Systemd offers improved boot speed, parallel startup, automatic dependency management, socket activation, and centralized logging. However, Systemd is more complex and has a steeper learning curve compared to the simpler SysVinit approach**

 - Systemd requires a unit file
 - Exercise:
   - how to list services
   - sections of unit file
   - create a sample unit file for spring petclinic [Refer Here]()