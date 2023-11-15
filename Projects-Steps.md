## Create Virtual Machine ##

1. Login to Azure Portal at [Azure Portal](www.portal.azure.com)

After a successful login, you should have a page like this:
![Azure Portal home page](azure_portal_homepage.png)

2. **Create a Resource Group to which the VM will belong**
   Click on Resource Group icon
   ![Resource Group](resource_group.png)
   Provide the Resource Group name and create it
   ![](create-resourcegroup.png)

3. **Create a Virtual Machine**
   Login to the Azure Portal
   Select Create a Resource
   ![](create-resource.png)

   Search for Virtual Machine in the new page
   ![](search_vm.png)

   Click on Virtual Machine tab

   ![](search_result1.png)

   Complete the Basic tab of the Virtual Machine configuration according to your requirements

   ![](vm_basic_config.png)

   Cycle through all the tabs (Disk, Networking, etc.) to complete the VM configuration
   You will need to create vnet and IP address subnet to be used on the vnet
   ![](vnet_ipaddress.png)
   
   Click Create to create the Virtual Machine
   Wait until deployment is complete. May take some time.

   ![](vm_dep_complete.png)

4. **Create a Hub network with VNet peering**
   Create a hub network with VNet peering to the Service_Test_Network, all inside a new resource group, ready for an Azure Standard Firewall deployment.
   To complete this task, we will create a Resource Group, a Hub Vnet, a subnet

   Create a resource group named Services_Security

   ![](resource_grp2.png)

   Now, create the Vnet
   Click create resource tab and search for Virtual Networks service, then create
   
   ![](virt_netw.png)

   ![](virt_netwip.png)


5. **VNet Peering**

   Select Virtual Networks
   Select "Services_Hub" virtual network
   Select "Peering" tab

   ![](vnet_peering.png)

   Click on +Add on the Peering page to add a new VNet Peer

   ![](vnet_peering_config.png)

   Completed VNet looks like this:

   ![](peering_completed.png)

6. **Azure Standard Firewall deployment**

   From the Azure Portal home, search for Firewall
   Click on Create firewall tab

   ![](create_firewall.png)

   Supply required details of the Firewall

   ![](firewall_config.png)
   

   
   
   

   
   
