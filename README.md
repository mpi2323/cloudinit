# Sample files for different Cloud-init use cases

cloud_config_sample.yml

simple example for cloud config - for customizing of AHV VMs for example

--

cloud_config_ubuntu_hostnamesample.yml

cloud_config_ubuntu_ipsample.yml

not tried yet...work in progress

--

rancher_cloudinit_centos_npp

example for rancher vspere node template using network profiles

template prep: 
installed cloud-init, docker
Run echo 'network: {config: disabled}' > /etc/cloud/cloud.cfg.d/99-disable-network-config.cfg
Run  cloud-init clean -s -l
disable vmtoolsd agent: systemctl disable vmtoolsd