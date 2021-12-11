# Lab 3: Manage Azure disks with the Azure CLI

1. Default Azure disks
2. Azure data disks
3. VM disk types
4. Launch Azure Cloud Shell
5. Create and attach disks
6. Prepare data disks
7. Take a disk snapshot

### Notes:

## this lab exercise has thought me a great deal on how to determine and create VM with appropriate disk sizes that will be effective for my workload

## I completed all the task successfully but though needs hands on deck for mastering

# however i was unable to debbug the error message while trying to create a VM with addtional disk
used the below code
az vm create \
--resource-group okyGroupDisk \
--name okydiskVM \
--image UbuntuLTS \
--size Standard_DS2_v2 \
--admin-username okydisk \
--generate-ssh-keys \
--data-disk-sizes-gb 128 128
there was an error message, but when i visited my dashboard i found out that the additinal dis of 128 was successfuly created

Quickstart: Manage Azure disks
* https://docs.microsoft.com/en-us/azure/virtual-machines/linux/tutorial-manage-disks

Quickstart for Bash in Azure Cloud Shell
* https://docs.microsoft.com/en-us/azure/cloud-shell/quickstart