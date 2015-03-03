proxyapp

A combined service script that uses a configuration flat-file database
to define remote hosts and services that can be reached via ssh-proxying

The following services are currently supported:  
1. ssh  
2. sftp  
3. Microsoft remote-desktop (RDP)  
4. VNC remote desktop  


To install, follow these simple steps:  
1. Clone the GIT repository onto your system  
2. Move the 'proxyapp' into your preferred 'bin' directory (PATH-findable)  (OPTIONAL)  
3. Create symlinks to the proxyapp script:  
    ln -s [INSTALL_DIR]/proxyapp /usr/local/bin/proxyssh  
    ln -s [INSTALL_DIR]/proxyapp /usr/local/bin/proxyftp  
    ln -s [INSTALL_DIR]/proxyapp /usr/local/bin/proxyrdp  
    ln -s [INSTALL_DIR]/proxyapp /usr/local/bin/proxyvnc  
4. Copy the exampele proxies.cnf into your home directory as a 'hidden' file:  
    cp [INSTALL_DIR]/proxies.cnf ${HOME}/.proxies.cnf  
5. Customize the configuration file, following the examples.  
6. run one of the scripts with the "-L" option to validate that all the services are showing up correctly 
