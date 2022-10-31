# A10-Ansible-Examples
Example yml files for ansible to make changes to A10 ADC devices

The samply yml files are based on the A10 Ansible ACOS modules
Please install the ACOS AXAPI Ansible modules from https://github.com/a10networks/a10-acos-axapi

This is a set of example Ansible yml files to install an A10 (v)Thunder instances 
the a10.inv files contain the Ansible inventory of the Thunder device for configuration 
and all the parameters needed to deploy the yml files.  

Sample ansible command: ansible-playbook -i a10.inv deploy-a10.yml -vvv

The files perform the following functions (all parameters red from the a10.inv file):

a10-set-hostname.yml
a10-set-DNS.yml
a10-set-timezone.yml
a10-set-NTP.yml
a10-set-vlan.yml
a10-set-ip.yml
a10-set-dfg.yml
a10-set-license.yml
a10-wr-mem.yml

deploy-a10.yml - aggrigated playbook, from the list above, to deploy a (v)Thunder device.


