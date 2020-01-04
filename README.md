This packer file creates a Ubuntu template leveraging the [JetBrains vSphere-ISO builder](https://github.com/jetbrains-infra/packer-builder-vsphere).

It will install Ubuntu from the ISO located in the iso_paths variable block, and pulls down the following packages required for the use of cloud-init, and the dependencies for the [VMware guestinfo datasource for cloud-init](https://github.com/vmware/cloud-init-vmware-guestinfo):
* open-vm-tools
* openssh-server
* curl
* python3-pip
* cloud-init

Note that you will need to install the JetBrains plugin linked above to use this definition.