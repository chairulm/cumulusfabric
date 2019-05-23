# cumulusfabric

4 File to create Cumulus Fabric Initial Installation

Preparation Step:
- Edit the Configuration in create_hostfile.py
- Make sure you can SSH all the switches from the machine which this script will be executed.

Executing Step :
1. python create_hostfile.py
This will create ansible host in current directory named fabric_host

2. ansible-playbook -i fabric_host create_fabric.yml
This will execute the fabric config to all the switch

Note:
- This script only been tested to 2 Level Spine-Leaf Configuration
