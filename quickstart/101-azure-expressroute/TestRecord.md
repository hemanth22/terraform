## 27 Jul 25 01:31 UTC

Success: false

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_pet.rg_name: Refreshing state... [id=rg-viable-monkfish][0m
	            	[0m[1mrandom_string.name: Refreshing state... [id=tenwphno][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish/providers/Microsoft.Network/virtualNetworks/vnet-tenwphno][0m
	            	[0m[1mazurerm_express_route_circuit.circuit: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish/providers/Microsoft.Network/expressRouteCircuits/erc-tenwphno][0m
	            	[0m[1mazurerm_public_ip.gateway_ip: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish/providers/Microsoft.Network/publicIPAddresses/pip-tenwphno][0m
	            	[0m[1mazurerm_subnet.gateway_subnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish/providers/Microsoft.Network/virtualNetworks/vnet-tenwphno/subnets/GatewaySubnet][0m
	            	[0m[1mazurerm_express_route_circuit_peering.private: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish/providers/Microsoft.Network/expressRouteCircuits/erc-tenwphno/peerings/AzurePrivatePeering][0m
	            	[0m[1mazurerm_virtual_network_gateway.gateway: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish/providers/Microsoft.Network/virtualNetworkGateways/gateway-tenwphno][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_virtual_network_gateway.gateway[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_virtual_network_gateway" "gateway" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish/providers/Microsoft.Network/virtualNetworkGateways/gateway-tenwphno"
	            	        name                                  = "gateway-tenwphno"
	            	        tags                                  = {}
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m ip_configuration {
	            	            name                          = "vnetGatewayConfig"
	            	          [32m+[0m[0m public_ip_address_id          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-viable-monkfish/providers/Microsoft.Network/publicIPAddresses/pip-tenwphno"
	            	            [90m# (2 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-azure-expressroute2730381298/src/quickstart/101-azure-expressroute/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-azure-expressroute2730381298/src/quickstart/101-azure-expressroute/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-azure-expressroute

FailNow

---

## 20 Jul 25 00:47 UTC

Success: false

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_pet.rg_name: Refreshing state... [id=rg-exact-cattle][0m
	            	[0m[1mrandom_string.name: Refreshing state... [id=ecnbeojn][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle][0m
	            	[0m[1mazurerm_express_route_circuit.circuit: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle/providers/Microsoft.Network/expressRouteCircuits/erc-ecnbeojn][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle/providers/Microsoft.Network/virtualNetworks/vnet-ecnbeojn][0m
	            	[0m[1mazurerm_public_ip.gateway_ip: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle/providers/Microsoft.Network/publicIPAddresses/pip-ecnbeojn][0m
	            	[0m[1mazurerm_subnet.gateway_subnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle/providers/Microsoft.Network/virtualNetworks/vnet-ecnbeojn/subnets/GatewaySubnet][0m
	            	[0m[1mazurerm_virtual_network_gateway.gateway: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle/providers/Microsoft.Network/virtualNetworkGateways/gateway-ecnbeojn][0m
	            	[0m[1mazurerm_express_route_circuit_peering.private: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle/providers/Microsoft.Network/expressRouteCircuits/erc-ecnbeojn/peerings/AzurePrivatePeering][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_virtual_network_gateway.gateway[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_virtual_network_gateway" "gateway" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle/providers/Microsoft.Network/virtualNetworkGateways/gateway-ecnbeojn"
	            	        name                                  = "gateway-ecnbeojn"
	            	        tags                                  = {}
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m ip_configuration {
	            	            name                          = "vnetGatewayConfig"
	            	          [32m+[0m[0m public_ip_address_id          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-exact-cattle/providers/Microsoft.Network/publicIPAddresses/pip-ecnbeojn"
	            	            [90m# (2 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-azure-expressroute2171152921/src/quickstart/101-azure-expressroute/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-azure-expressroute2171152921/src/quickstart/101-azure-expressroute/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-azure-expressroute

FailNow

---

## 13 Jul 25 02:00 UTC

Success: false

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_pet.rg_name: Refreshing state... [id=rg-loving-marmoset][0m
	            	[0m[1mrandom_string.name: Refreshing state... [id=fqxxlzie][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset/providers/Microsoft.Network/virtualNetworks/vnet-fqxxlzie][0m
	            	[0m[1mazurerm_public_ip.gateway_ip: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset/providers/Microsoft.Network/publicIPAddresses/pip-fqxxlzie][0m
	            	[0m[1mazurerm_express_route_circuit.circuit: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset/providers/Microsoft.Network/expressRouteCircuits/erc-fqxxlzie][0m
	            	[0m[1mazurerm_subnet.gateway_subnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset/providers/Microsoft.Network/virtualNetworks/vnet-fqxxlzie/subnets/GatewaySubnet][0m
	            	[0m[1mazurerm_express_route_circuit_peering.private: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset/providers/Microsoft.Network/expressRouteCircuits/erc-fqxxlzie/peerings/AzurePrivatePeering][0m
	            	[0m[1mazurerm_virtual_network_gateway.gateway: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset/providers/Microsoft.Network/virtualNetworkGateways/gateway-fqxxlzie][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_virtual_network_gateway.gateway[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_virtual_network_gateway" "gateway" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset/providers/Microsoft.Network/virtualNetworkGateways/gateway-fqxxlzie"
	            	        name                                  = "gateway-fqxxlzie"
	            	        tags                                  = {}
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m ip_configuration {
	            	            name                          = "vnetGatewayConfig"
	            	          [32m+[0m[0m public_ip_address_id          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-loving-marmoset/providers/Microsoft.Network/publicIPAddresses/pip-fqxxlzie"
	            	            [90m# (2 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-azure-expressroute442747611/src/quickstart/101-azure-expressroute/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-azure-expressroute442747611/src/quickstart/101-azure-expressroute/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-azure-expressroute

FailNow

---

## 06 Jul 25 01:18 UTC

Success: false

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_pet.rg_name: Refreshing state... [id=rg-enormous-starfish][0m
	            	[0m[1mrandom_string.name: Refreshing state... [id=tldcterr][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish/providers/Microsoft.Network/virtualNetworks/vnet-tldcterr][0m
	            	[0m[1mazurerm_express_route_circuit.circuit: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish/providers/Microsoft.Network/expressRouteCircuits/erc-tldcterr][0m
	            	[0m[1mazurerm_public_ip.gateway_ip: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish/providers/Microsoft.Network/publicIPAddresses/pip-tldcterr][0m
	            	[0m[1mazurerm_express_route_circuit_peering.private: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish/providers/Microsoft.Network/expressRouteCircuits/erc-tldcterr/peerings/AzurePrivatePeering][0m
	            	[0m[1mazurerm_subnet.gateway_subnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish/providers/Microsoft.Network/virtualNetworks/vnet-tldcterr/subnets/GatewaySubnet][0m
	            	[0m[1mazurerm_virtual_network_gateway.gateway: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish/providers/Microsoft.Network/virtualNetworkGateways/gateway-tldcterr][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_virtual_network_gateway.gateway[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_virtual_network_gateway" "gateway" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish/providers/Microsoft.Network/virtualNetworkGateways/gateway-tldcterr"
	            	        name                                  = "gateway-tldcterr"
	            	        tags                                  = {}
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m ip_configuration {
	            	            name                          = "vnetGatewayConfig"
	            	          [32m+[0m[0m public_ip_address_id          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-enormous-starfish/providers/Microsoft.Network/publicIPAddresses/pip-tldcterr"
	            	            [90m# (2 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-azure-expressroute4214565926/src/quickstart/101-azure-expressroute/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-azure-expressroute4214565926/src/quickstart/101-azure-expressroute/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-azure-expressroute

FailNow

---

## 29 Jun 25 01:36 UTC

Success: false

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_pet.rg_name: Refreshing state... [id=rg-inviting-rabbit][0m
	            	[0m[1mrandom_string.name: Refreshing state... [id=mhfjdffp][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit][0m
	            	[0m[1mazurerm_express_route_circuit.circuit: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit/providers/Microsoft.Network/expressRouteCircuits/erc-mhfjdffp][0m
	            	[0m[1mazurerm_public_ip.gateway_ip: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit/providers/Microsoft.Network/publicIPAddresses/pip-mhfjdffp][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit/providers/Microsoft.Network/virtualNetworks/vnet-mhfjdffp][0m
	            	[0m[1mazurerm_subnet.gateway_subnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit/providers/Microsoft.Network/virtualNetworks/vnet-mhfjdffp/subnets/GatewaySubnet][0m
	            	[0m[1mazurerm_virtual_network_gateway.gateway: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit/providers/Microsoft.Network/virtualNetworkGateways/gateway-mhfjdffp][0m
	            	[0m[1mazurerm_express_route_circuit_peering.private: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit/providers/Microsoft.Network/expressRouteCircuits/erc-mhfjdffp/peerings/AzurePrivatePeering][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_virtual_network_gateway.gateway[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_virtual_network_gateway" "gateway" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit/providers/Microsoft.Network/virtualNetworkGateways/gateway-mhfjdffp"
	            	        name                                  = "gateway-mhfjdffp"
	            	        tags                                  = {}
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m ip_configuration {
	            	            name                          = "vnetGatewayConfig"
	            	          [32m+[0m[0m public_ip_address_id          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-inviting-rabbit/providers/Microsoft.Network/publicIPAddresses/pip-mhfjdffp"
	            	            [90m# (2 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-azure-expressroute3121885574/src/quickstart/101-azure-expressroute/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-azure-expressroute3121885574/src/quickstart/101-azure-expressroute/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-azure-expressroute

FailNow

---

## 15 Jun 25 01:52 UTC

Success: true

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 08 Jun 25 01:40 UTC

Success: true

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 01 Jun 25 01:47 UTC

Success: true

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 25 May 25 01:25 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 18 May 25 01:19 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 11 May 25 01:39 UTC

Success: false

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_pet.rg_name: Refreshing state... [id=rg-proper-colt][0m
	            	[0m[1mrandom_string.name: Refreshing state... [id=wbdodqhx][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-proper-colt][0m
	            	[0m[1mazurerm_public_ip.gateway_ip: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-proper-colt/providers/Microsoft.Network/publicIPAddresses/pip-wbdodqhx][0m
	            	[0m[1mazurerm_express_route_circuit.circuit: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-proper-colt/providers/Microsoft.Network/expressRouteCircuits/erc-wbdodqhx][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-proper-colt/providers/Microsoft.Network/virtualNetworks/vnet-wbdodqhx][0m
	            	[0m[1mazurerm_subnet.gateway_subnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-proper-colt/providers/Microsoft.Network/virtualNetworks/vnet-wbdodqhx/subnets/GatewaySubnet][0m
	            	[0m[1mazurerm_virtual_network_gateway.gateway: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-proper-colt/providers/Microsoft.Network/virtualNetworkGateways/gateway-wbdodqhx][0m
	            	[0m[1mazurerm_express_route_circuit_peering.private: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-proper-colt/providers/Microsoft.Network/expressRouteCircuits/erc-wbdodqhx/peerings/AzurePrivatePeering][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_resource_group.rg[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_resource_group" "rg" {
	            	        id         = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-proper-colt"
	            	        name       = "rg-proper-colt"
	            	      [33m~[0m[0m tags       = {
	            	          [31m-[0m[0m "mapotfdemo" = "yes" [90m-> null[0m[0m
	            	        }
	            	        [90m# (2 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-azure-expressroute2562552062/src/quickstart/101-azure-expressroute/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-azure-expressroute2562552062/src/quickstart/101-azure-expressroute/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-azure-expressroute

FailNow

---

## 04 May 25 01:38 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 27 Apr 25 00:49 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 20 Apr 25 01:06 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 13 Apr 25 02:10 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 06 Apr 25 01:22 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 30 Mar 25 02:18 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 23 Mar 25 01:47 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 16 Mar 25 01:06 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 09 Mar 25 02:01 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 02 Mar 25 01:58 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 23 Feb 25 01:10 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 16 Feb 25 00:50 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 09 Feb 25 01:37 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 02 Feb 25 01:15 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 26 Jan 25 01:12 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 23 Jan 25 10:37 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 19 Jan 25 01:41 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 12 Jan 25 01:46 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 05 Jan 25 01:05 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Dec 24 00:41 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 22 Dec 24 00:42 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 15 Dec 24 02:09 UTC

Success: true

### Versions

Terraform v1.10.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

