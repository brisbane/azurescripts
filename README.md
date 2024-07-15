# azurescripts
### azure scripts ###
#### clone_VM ####



This clones a virtual machine via disk snapshots.  The new machine has the same sku as the old. It may not work to clone over regions due to limitations on snapshots in Azure.

It also clones the network security group and expects the VM to have only one NIC and requires the VM to have at least one NIC and one and only one NSG

Some of the settings are propagated, such as if the machine has a public IP on its first NIC and if ip forwarding is enabled.

##### Prerequisites #####

The destination resource group, vnet and subnet must exist

