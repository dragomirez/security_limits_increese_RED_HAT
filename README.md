Change User Max Proccesses

Usage:

ansible-playbook -i hosts change_nproc.yaml -e nodes=<enter names of all nodes>  -e 
user=mapr -e limit_type=soft -e limit_item=nproc -e limit=64000

You can specify on which cluster to apply the change as giving extra variable “nodes” as shown above.

Inventory groups:

nodes= <enter names of all nodes> 

Check current value for specified user:
ansible-playbook -i hosts check.yaml -e nodes=dpd -e user=mapr