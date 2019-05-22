# ansible-disks-aws
Installs a list of packages from repos and local package files.  Supports provisioning RedHat, Debian, or a mixed group.

##### Instructions
1. Define var `package_list` in vars/RedHat.yml, vars/Debian.yml, group_vars, or host_vars with a list of packages to be installed from repos
2. Put any packages for local install into the files/ directory
3. Define var `package_list` in vars/RedHat.yml, vars/Debian.yml, group_vars, or host_vars with a list of local package filenames


#####  Task Overview
1. Installs a list of packages as defined by var `package_list`
2. Copies deb or rpm packages to /tmp target server
3. Installs deb or rpm packages

##### Assumptions
None
