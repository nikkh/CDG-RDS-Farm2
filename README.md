# VNet and Comain Controllers

This template will deploy 2 new VMs (along with a new VNet, Storage Account and Load Balancer) and create a new  AD forest and domain, each VM will be created as a DC for the new domain and will be placed in an availability set. Each VM will also have an RDP endpoint added with a public load balanced IP address.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fnikkh%2FCDG-RDS-Farm2%2Fmaster%2FCDG-RDS-Farm2%2Fcreate-domain.json" target="_blank">
   Deploy VNet and Domain Controllers
</a>

# RDS Farm

This template deploys the following resources:

<ul><li>storage account;</li><li>RD Gateway/RD Web Access vm;</li><li>RD Connection Broker/RD Licensing Server vm;</li><li>a number of RD Session hosts (number defined by 'numberOfRdshInstances' parameter)</li></ul>

The template will use existing DC, join all vms to the domain and configure RDS roles in the deployment.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fnikkh%2FCDG-RDS-Farm2%2Fmaster%2FCDG-RDS-Farm2%2Fdeploy-rds-farm.json" target="_blank">
   Deploy RDS Farm
</a>
