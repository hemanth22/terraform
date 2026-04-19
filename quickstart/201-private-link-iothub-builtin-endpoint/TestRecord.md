## 19 Apr 26 00:38 UTC

Success: false

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:50
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_string.suffix: Refreshing state... [id=eg0x2][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/virtualNetworks/iothub-vnet-eg0x2][0m
	            	[0m[1mazurerm_private_dns_zone.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net][0m
	            	[0m[1mazurerm_private_dns_zone.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net][0m
	            	[0m[1mazurerm_private_dns_zone.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net][0m
	            	[0m[1mazurerm_iothub.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Devices/iotHubs/iothub-eg0x2][0m
	            	[0m[1mazurerm_subnet.snet: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/virtualNetworks/iothub-vnet-eg0x2/subnets/iothub-snet-eg0x2][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/virtualNetworkLinks/vnet-link-eventhub-eg0x2][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net/virtualNetworkLinks/vnet-link-iothub-eg0x2][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net/virtualNetworkLinks/vnet-link-dps-eg0x2][0m
	            	[0m[1mazurerm_private_endpoint.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateEndpoints/pep-iothub-eg0x2][0m
	            	[0m[1mazurerm_iothub_shared_access_policy.iothub_policy: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Devices/iotHubs/iothub-eg0x2/iotHubKeys/iothub-policy][0m
	            	[0m[1mazurerm_private_dns_a_record.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-eg0-67259645-2f2fa2544b][0m
	            	[0m[1mazurerm_iothub_dps.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Devices/provisioningServices/test-device-eg0x2][0m
	            	[0m[1mazurerm_private_endpoint.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateEndpoints/pep-dps-eg0x2][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	[31m-[0m/[32m+[0m destroy and then create replacement[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_iothub.iothub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_iothub" "iothub" {
	            	      [33m~[0m[0m endpoint                      = [] -> (known after apply)
	            	      [33m~[0m[0m enrichment                    = [] -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_endpoint     = "sb://iothub-ns-iothub-eg0-67259645-2f2fa2544b.servicebus.windows.net/" -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_namespace    = "iothub-ns-iothub-eg0-67259645-2f2fa2544b" -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_path         = "iothub-eg0x2" -> (known after apply)
	            	      [32m+[0m[0m event_hub_operations_endpoint = (known after apply)
	            	      [32m+[0m[0m event_hub_operations_path     = (known after apply)
	            	      [33m~[0m[0m event_hub_partition_count     = 4 -> (known after apply)
	            	      [33m~[0m[0m event_hub_retention_in_days   = 1 -> (known after apply)
	            	      [33m~[0m[0m hostname                      = "iothub-eg0x2.azure-devices.net" -> (known after apply)
	            	      [33m~[0m[0m id                            = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Devices/iotHubs/iothub-eg0x2" -> (known after apply)
	            	      [31m-[0m[0m min_tls_version               = "1.2" [90m-> null[0m[0m [31m# forces replacement[0m[0m
	            	        name                          = "iothub-eg0x2"
	            	      [33m~[0m[0m route                         = [] -> (known after apply)
	            	      [33m~[0m[0m shared_access_policy          = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "iothubowner"
	            	              [31m-[0m[0m permissions   = "RegistryWrite, ServiceConnect, DeviceConnect"
	            	              [31m-[0m[0m primary_key   = "6XgQZ8VigODPabN3/yRx7qNSMrkk2LyUbAIoTDiKr/M="
	            	              [31m-[0m[0m secondary_key = "ko1y/vIgdzFK0ZqeOuHfz+NsGHkhEX8GYAIoTLe1jyQ="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "service"
	            	              [31m-[0m[0m permissions   = "ServiceConnect"
	            	              [31m-[0m[0m primary_key   = "/++noKUyZeGW00iBbPpe9bJYrrhuTvD6eAIoTO3VtaI="
	            	              [31m-[0m[0m secondary_key = "N7Di8ecHDk9yHJhRCkd+NFkqtId4fBMzmAIoTAUltXs="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "device"
	            	              [31m-[0m[0m permissions   = "DeviceConnect"
	            	              [31m-[0m[0m primary_key   = "hzgPfFTHIoArGnBnhggYWU0+gTKvQhEKtAIoTMHtjLc="
	            	              [31m-[0m[0m secondary_key = "IholUcVVCYX/IP/QPAevsk7t0EcA/GURtAIoTHpEGCM="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "registryRead"
	            	              [31m-[0m[0m permissions   = "RegistryRead"
	            	              [31m-[0m[0m primary_key   = "tAFPd32LtGP1/xaZaaKQO0LGmsKyCR03fAIoTBjU8Jc="
	            	              [31m-[0m[0m secondary_key = "z+ZI40c35DD7TlzSVQs3D0NffGStTSuyFAIoTAxbbII="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "registryReadWrite"
	            	              [31m-[0m[0m permissions   = "RegistryWrite"
	            	              [31m-[0m[0m primary_key   = "ywbah1GZk9cCQbc2BbApTptJSHgEM3nL4AIoTLaLKF8="
	            	              [31m-[0m[0m secondary_key = "9GV1hSOb/rGXNm+dCojdmmTHvDhwSsaVoAIoTOj17xs="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "iothub-policy"
	            	              [31m-[0m[0m permissions   = "RegistryWrite, ServiceConnect"
	            	              [31m-[0m[0m primary_key   = "/aHvkNsYK7/6XXYVaL32ByXJysOI/kIg1AIoTIeUpbs="
	            	              [31m-[0m[0m secondary_key = "sgxaFpT4NDICCXn6i3hS7h8rreu+m8A71AIoTJcrasI="
	            	            },
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                          = {} [90m-> null[0m[0m
	            	      [33m~[0m[0m type                          = "Microsoft.Devices/IotHubs" -> (known after apply)
	            	        [90m# (4 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m fallback_route (known after apply)
	            	      [31m-[0m[0m fallback_route {
	            	          [31m-[0m[0m condition      = "true" [90m-> null[0m[0m
	            	          [31m-[0m[0m enabled        = true [90m-> null[0m[0m
	            	          [31m-[0m[0m endpoint_names = [
	            	              [31m-[0m[0m "events",
	            	            ] [90m-> null[0m[0m
	            	          [31m-[0m[0m source         = "DeviceMessages" [90m-> null[0m[0m
	            	        }
	            	
	            	        [90m# (2 unchanged blocks hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_private_dns_a_record.eventhub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_private_dns_a_record" "eventhub" {
	            	      [33m~[0m[0m fqdn                = "iothub-ns-iothub-eg0-67259645-2f2fa2544b.privatelink.servicebus.windows.net." -> (known after apply)
	            	      [33m~[0m[0m id                  = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-eg0-67259645-2f2fa2544b" -> (known after apply)
	            	      [33m~[0m[0m name                = "iothub-ns-iothub-eg0-67259645-2f2fa2544b" -> (known after apply) [31m# forces replacement[0m[0m
	            	      [33m~[0m[0m records             = [
	            	          [31m-[0m[0m "10.0.3.5",
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                = {} [90m-> null[0m[0m
	            	        [90m# (3 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_private_endpoint.iothub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_private_endpoint" "iothub" {
	            	      [33m~[0m[0m custom_dns_configs            = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m fqdn         = "iothub-ns-iothub-eg0-67259645-2f2fa2544b.servicebus.windows.net"
	            	              [31m-[0m[0m ip_addresses = [
	            	                  [31m-[0m[0m "10.0.3.5",
	            	                ]
	            	            },
	            	        ] -> (known after apply)
	            	      [33m~[0m[0m id                            = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateEndpoints/pep-iothub-eg0x2" -> (known after apply)
	            	        name                          = "pep-iothub-eg0x2"
	            	      [33m~[0m[0m network_interface             = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m id   = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/networkInterfaces/pep-iothub-eg0x2.nic.46da5b21-6191-4809-bede-8e245e7f794c"
	            	              [31m-[0m[0m name = "pep-iothub-eg0x2.nic.46da5b21-6191-4809-bede-8e245e7f794c"
	            	            },
	            	        ] -> (known after apply)
	            	      [33m~[0m[0m private_dns_zone_configs      = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m id                  = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateEndpoints/pep-iothub-eg0x2/privateDnsZoneGroups/privateDNSZoneGroup/privateDnsZoneConfigs/privatelink.azure-devices.net"
	            	              [31m-[0m[0m name                = "privatelink.azure-devices.net"
	            	              [31m-[0m[0m private_dns_zone_id = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net"
	            	              [31m-[0m[0m record_sets         = [
	            	                  [31m-[0m[0m {
	            	                      [31m-[0m[0m fqdn         = "iothub-eg0x2.privatelink.azure-devices.net"
	            	                      [31m-[0m[0m ip_addresses = [
	            	                          [31m-[0m[0m "10.0.3.4",
	            	                        ]
	            	                      [31m-[0m[0m name         = "iothub-eg0x2"
	            	                      [31m-[0m[0m ttl          = 10
	            	                      [31m-[0m[0m type         = "A"
	            	                    },
	            	                ]
	            	            },
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                          = {} [90m-> null[0m[0m
	            	        [90m# (4 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m private_dns_zone_group {
	            	          [33m~[0m[0m id                   = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Network/privateEndpoints/pep-iothub-eg0x2/privateDnsZoneGroups/privateDNSZoneGroup" -> (known after apply)
	            	            name                 = "privateDNSZoneGroup"
	            	            [90m# (1 unchanged attribute hidden)[0m[0m
	            	        }
	            	
	            	      [33m~[0m[0m private_service_connection {
	            	            name                              = "psc-iothub-eg0x2"
	            	          [33m~[0m[0m private_connection_resource_id    = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-eg0x2/providers/Microsoft.Devices/iotHubs/iothub-eg0x2" -> (known after apply) [31m# forces replacement[0m[0m
	            	          [33m~[0m[0m private_ip_address                = "10.0.3.4" -> (known after apply)
	            	            [90m# (4 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 3 to add, 0 to change, 3 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/201-private-link-iothub-builtin-endpoint776071557/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/201-private-link-iothub-builtin-endpoint776071557/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan"
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 12 Apr 26 00:36 UTC

Success: false

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:50
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_string.suffix: Refreshing state... [id=l1pes][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/virtualNetworks/iothub-vnet-l1pes][0m
	            	[0m[1mazurerm_private_dns_zone.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net][0m
	            	[0m[1mazurerm_private_dns_zone.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net][0m
	            	[0m[1mazurerm_private_dns_zone.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net][0m
	            	[0m[1mazurerm_iothub.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Devices/iotHubs/iothub-l1pes][0m
	            	[0m[1mazurerm_subnet.snet: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/virtualNetworks/iothub-vnet-l1pes/subnets/iothub-snet-l1pes][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/virtualNetworkLinks/vnet-link-eventhub-l1pes][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net/virtualNetworkLinks/vnet-link-dps-l1pes][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net/virtualNetworkLinks/vnet-link-iothub-l1pes][0m
	            	[0m[1mazurerm_private_endpoint.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateEndpoints/pep-iothub-l1pes][0m
	            	[0m[1mazurerm_iothub_shared_access_policy.iothub_policy: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Devices/iotHubs/iothub-l1pes/iotHubKeys/iothub-policy][0m
	            	[0m[1mazurerm_private_dns_a_record.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-l1p-67194045-46545f880e][0m
	            	[0m[1mazurerm_iothub_dps.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Devices/provisioningServices/test-device-l1pes][0m
	            	[0m[1mazurerm_private_endpoint.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateEndpoints/pep-dps-l1pes][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	[31m-[0m/[32m+[0m destroy and then create replacement[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_iothub.iothub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_iothub" "iothub" {
	            	      [33m~[0m[0m endpoint                      = [] -> (known after apply)
	            	      [33m~[0m[0m enrichment                    = [] -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_endpoint     = "sb://iothub-ns-iothub-l1p-67194045-46545f880e.servicebus.windows.net/" -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_namespace    = "iothub-ns-iothub-l1p-67194045-46545f880e" -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_path         = "iothub-l1pes" -> (known after apply)
	            	      [32m+[0m[0m event_hub_operations_endpoint = (known after apply)
	            	      [32m+[0m[0m event_hub_operations_path     = (known after apply)
	            	      [33m~[0m[0m event_hub_partition_count     = 4 -> (known after apply)
	            	      [33m~[0m[0m event_hub_retention_in_days   = 1 -> (known after apply)
	            	      [33m~[0m[0m hostname                      = "iothub-l1pes.azure-devices.net" -> (known after apply)
	            	      [33m~[0m[0m id                            = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Devices/iotHubs/iothub-l1pes" -> (known after apply)
	            	      [31m-[0m[0m min_tls_version               = "1.2" [90m-> null[0m[0m [31m# forces replacement[0m[0m
	            	        name                          = "iothub-l1pes"
	            	      [33m~[0m[0m route                         = [] -> (known after apply)
	            	      [33m~[0m[0m shared_access_policy          = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "iothubowner"
	            	              [31m-[0m[0m permissions   = "RegistryWrite, ServiceConnect, DeviceConnect"
	            	              [31m-[0m[0m primary_key   = "+pUE282IDWO9/Gh8Ovbqc+YdUN+BE15LfAIoTEoMLmY="
	            	              [31m-[0m[0m secondary_key = "gXPOeytM7V+Tb2NRU2LrgtLunc5ooQDilAIoTC8VfEI="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "service"
	            	              [31m-[0m[0m permissions   = "ServiceConnect"
	            	              [31m-[0m[0m primary_key   = "3NqCBHJuQY5ZRxDcvNx5x1jY1rE4wYBjZAIoTPfLDaU="
	            	              [31m-[0m[0m secondary_key = "I81XBeXbJhoKPKNStoCqiTJ/2qk8/y/D4AIoTNwlICQ="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "device"
	            	              [31m-[0m[0m permissions   = "DeviceConnect"
	            	              [31m-[0m[0m primary_key   = "G7O1ILE+JPrFuC/0pQk1DPyxr3CY0TShVAIoTKjsSGg="
	            	              [31m-[0m[0m secondary_key = "n9K3AS28ih8qGXMdFUuDpiWKR6+AMPUblAIoTI9kKn0="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "registryRead"
	            	              [31m-[0m[0m permissions   = "RegistryRead"
	            	              [31m-[0m[0m primary_key   = "0sDfJM8hd1zd7Psuol4ubCfDxsKYGAqA8AIoTImHhA8="
	            	              [31m-[0m[0m secondary_key = "q/vJqrnxW3X2fM74BTwoMUlAVJDZvaQnLAIoTLw41u8="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "registryReadWrite"
	            	              [31m-[0m[0m permissions   = "RegistryWrite"
	            	              [31m-[0m[0m primary_key   = "gD68qnX57QUHLmUYP6LWcyC3jxvAtj08xAIoTFA8EXw="
	            	              [31m-[0m[0m secondary_key = "skz/4PhYvwxKulSMtitBATgV10cHxzwa4AIoTHkOniQ="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "iothub-policy"
	            	              [31m-[0m[0m permissions   = "RegistryWrite, ServiceConnect"
	            	              [31m-[0m[0m primary_key   = "h8a26x+6uLYwVAcazjInxDH//QW0shzAyAIoTAd7E10="
	            	              [31m-[0m[0m secondary_key = "5B3iOv4QRzntkAUdvF1bWp8og00JriM2aAIoTC2af04="
	            	            },
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                          = {} [90m-> null[0m[0m
	            	      [33m~[0m[0m type                          = "Microsoft.Devices/IotHubs" -> (known after apply)
	            	        [90m# (4 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m fallback_route (known after apply)
	            	      [31m-[0m[0m fallback_route {
	            	          [31m-[0m[0m condition      = "true" [90m-> null[0m[0m
	            	          [31m-[0m[0m enabled        = true [90m-> null[0m[0m
	            	          [31m-[0m[0m endpoint_names = [
	            	              [31m-[0m[0m "events",
	            	            ] [90m-> null[0m[0m
	            	          [31m-[0m[0m source         = "DeviceMessages" [90m-> null[0m[0m
	            	        }
	            	
	            	        [90m# (2 unchanged blocks hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_private_dns_a_record.eventhub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_private_dns_a_record" "eventhub" {
	            	      [33m~[0m[0m fqdn                = "iothub-ns-iothub-l1p-67194045-46545f880e.privatelink.servicebus.windows.net." -> (known after apply)
	            	      [33m~[0m[0m id                  = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-l1p-67194045-46545f880e" -> (known after apply)
	            	      [33m~[0m[0m name                = "iothub-ns-iothub-l1p-67194045-46545f880e" -> (known after apply) [31m# forces replacement[0m[0m
	            	      [33m~[0m[0m records             = [
	            	          [31m-[0m[0m "10.0.3.5",
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                = {} [90m-> null[0m[0m
	            	        [90m# (3 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_private_endpoint.iothub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_private_endpoint" "iothub" {
	            	      [33m~[0m[0m custom_dns_configs            = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m fqdn         = "iothub-ns-iothub-l1p-67194045-46545f880e.servicebus.windows.net"
	            	              [31m-[0m[0m ip_addresses = [
	            	                  [31m-[0m[0m "10.0.3.5",
	            	                ]
	            	            },
	            	        ] -> (known after apply)
	            	      [33m~[0m[0m id                            = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateEndpoints/pep-iothub-l1pes" -> (known after apply)
	            	        name                          = "pep-iothub-l1pes"
	            	      [33m~[0m[0m network_interface             = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m id   = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/networkInterfaces/pep-iothub-l1pes.nic.0489addc-8d7e-4c93-bb36-31f844e65555"
	            	              [31m-[0m[0m name = "pep-iothub-l1pes.nic.0489addc-8d7e-4c93-bb36-31f844e65555"
	            	            },
	            	        ] -> (known after apply)
	            	      [33m~[0m[0m private_dns_zone_configs      = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m id                  = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateEndpoints/pep-iothub-l1pes/privateDnsZoneGroups/privateDNSZoneGroup/privateDnsZoneConfigs/privatelink.azure-devices.net"
	            	              [31m-[0m[0m name                = "privatelink.azure-devices.net"
	            	              [31m-[0m[0m private_dns_zone_id = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net"
	            	              [31m-[0m[0m record_sets         = [
	            	                  [31m-[0m[0m {
	            	                      [31m-[0m[0m fqdn         = "iothub-l1pes.privatelink.azure-devices.net"
	            	                      [31m-[0m[0m ip_addresses = [
	            	                          [31m-[0m[0m "10.0.3.4",
	            	                        ]
	            	                      [31m-[0m[0m name         = "iothub-l1pes"
	            	                      [31m-[0m[0m ttl          = 10
	            	                      [31m-[0m[0m type         = "A"
	            	                    },
	            	                ]
	            	            },
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                          = {} [90m-> null[0m[0m
	            	        [90m# (4 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m private_dns_zone_group {
	            	          [33m~[0m[0m id                   = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Network/privateEndpoints/pep-iothub-l1pes/privateDnsZoneGroups/privateDNSZoneGroup" -> (known after apply)
	            	            name                 = "privateDNSZoneGroup"
	            	            [90m# (1 unchanged attribute hidden)[0m[0m
	            	        }
	            	
	            	      [33m~[0m[0m private_service_connection {
	            	            name                              = "psc-iothub-l1pes"
	            	          [33m~[0m[0m private_connection_resource_id    = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-l1pes/providers/Microsoft.Devices/iotHubs/iothub-l1pes" -> (known after apply) [31m# forces replacement[0m[0m
	            	          [33m~[0m[0m private_ip_address                = "10.0.3.4" -> (known after apply)
	            	            [90m# (4 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 3 to add, 0 to change, 3 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/201-private-link-iothub-builtin-endpoint518407640/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/201-private-link-iothub-builtin-endpoint518407640/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan"
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 05 Apr 26 00:43 UTC

Success: false

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:50
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_string.suffix: Refreshing state... [id=swaxz][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/virtualNetworks/iothub-vnet-swaxz][0m
	            	[0m[1mazurerm_private_dns_zone.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net][0m
	            	[0m[1mazurerm_private_dns_zone.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net][0m
	            	[0m[1mazurerm_private_dns_zone.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net][0m
	            	[0m[1mazurerm_iothub.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Devices/iotHubs/iothub-swaxz][0m
	            	[0m[1mazurerm_subnet.snet: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/virtualNetworks/iothub-vnet-swaxz/subnets/iothub-snet-swaxz][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net/virtualNetworkLinks/vnet-link-iothub-swaxz][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/virtualNetworkLinks/vnet-link-eventhub-swaxz][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net/virtualNetworkLinks/vnet-link-dps-swaxz][0m
	            	[0m[1mazurerm_private_endpoint.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateEndpoints/pep-iothub-swaxz][0m
	            	[0m[1mazurerm_private_dns_a_record.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-swa-67128565-2d20e9e245][0m
	            	[0m[1mazurerm_iothub_shared_access_policy.iothub_policy: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Devices/iotHubs/iothub-swaxz/iotHubKeys/iothub-policy][0m
	            	[0m[1mazurerm_iothub_dps.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Devices/provisioningServices/test-device-swaxz][0m
	            	[0m[1mazurerm_private_endpoint.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateEndpoints/pep-dps-swaxz][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	[31m-[0m/[32m+[0m destroy and then create replacement[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_iothub.iothub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_iothub" "iothub" {
	            	      [33m~[0m[0m endpoint                      = [] -> (known after apply)
	            	      [33m~[0m[0m enrichment                    = [] -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_endpoint     = "sb://iothub-ns-iothub-swa-67128565-2d20e9e245.servicebus.windows.net/" -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_namespace    = "iothub-ns-iothub-swa-67128565-2d20e9e245" -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_path         = "iothub-swaxz" -> (known after apply)
	            	      [32m+[0m[0m event_hub_operations_endpoint = (known after apply)
	            	      [32m+[0m[0m event_hub_operations_path     = (known after apply)
	            	      [33m~[0m[0m event_hub_partition_count     = 4 -> (known after apply)
	            	      [33m~[0m[0m event_hub_retention_in_days   = 1 -> (known after apply)
	            	      [33m~[0m[0m hostname                      = "iothub-swaxz.azure-devices.net" -> (known after apply)
	            	      [33m~[0m[0m id                            = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Devices/iotHubs/iothub-swaxz" -> (known after apply)
	            	      [31m-[0m[0m min_tls_version               = "1.2" [90m-> null[0m[0m [31m# forces replacement[0m[0m
	            	        name                          = "iothub-swaxz"
	            	      [33m~[0m[0m route                         = [] -> (known after apply)
	            	      [33m~[0m[0m shared_access_policy          = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "iothubowner"
	            	              [31m-[0m[0m permissions   = "RegistryWrite, ServiceConnect, DeviceConnect"
	            	              [31m-[0m[0m primary_key   = "Olzu9V0vCzjnTZ/SGH8m5rQu6G7a96LvxAIoTCrazp8="
	            	              [31m-[0m[0m secondary_key = "wVrBJSmFQWd21KrsJvSDrl2bEyvHUHLhHAIoTApKkaU="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "service"
	            	              [31m-[0m[0m permissions   = "ServiceConnect"
	            	              [31m-[0m[0m primary_key   = "Wwl6bD8ioV8o2rheY022nP+DCfrq6n2rbAIoTLn64mU="
	            	              [31m-[0m[0m secondary_key = "0TmyuRekh4sypvwPU7WbTT24uAh8x4wSfAIoTPxrMW8="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "device"
	            	              [31m-[0m[0m permissions   = "DeviceConnect"
	            	              [31m-[0m[0m primary_key   = "scy1iCbRWC9sUgSfbz/JzJLuL66XV7IwgAIoTDPoVc8="
	            	              [31m-[0m[0m secondary_key = "Hm8vluktVDkwhk9vLnh3hmXybp5aD9hxRAIoTLTcpss="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "registryRead"
	            	              [31m-[0m[0m permissions   = "RegistryRead"
	            	              [31m-[0m[0m primary_key   = "pThTaGndD3LAyoOWO0UQDhfwpL8sCwqcDAIoTGRMt6Q="
	            	              [31m-[0m[0m secondary_key = "jZCaI7WeNzB3gGndUEvb/R34df5AZNqLxAIoTFGcK0U="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "registryReadWrite"
	            	              [31m-[0m[0m permissions   = "RegistryWrite"
	            	              [31m-[0m[0m primary_key   = "gSK4YAFqq0y1VIUxbv4JB/bRwhNcRHOKjAIoTMD/gKY="
	            	              [31m-[0m[0m secondary_key = "MzUYs0gtSPz1ub4WcD99HHVGLj8qP/ofiAIoTAybXfA="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "iothub-policy"
	            	              [31m-[0m[0m permissions   = "RegistryWrite, ServiceConnect"
	            	              [31m-[0m[0m primary_key   = "okh0LBwSDcGrrZJC4oZ7pbarAOVtqDApwAIoTMGDsgc="
	            	              [31m-[0m[0m secondary_key = "LbHE1fHevT3r9emThxHOGbdXbBfuaW43SAIoTBksAFA="
	            	            },
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                          = {} [90m-> null[0m[0m
	            	      [33m~[0m[0m type                          = "Microsoft.Devices/IotHubs" -> (known after apply)
	            	        [90m# (4 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m fallback_route (known after apply)
	            	      [31m-[0m[0m fallback_route {
	            	          [31m-[0m[0m condition      = "true" [90m-> null[0m[0m
	            	          [31m-[0m[0m enabled        = true [90m-> null[0m[0m
	            	          [31m-[0m[0m endpoint_names = [
	            	              [31m-[0m[0m "events",
	            	            ] [90m-> null[0m[0m
	            	          [31m-[0m[0m source         = "DeviceMessages" [90m-> null[0m[0m
	            	        }
	            	
	            	        [90m# (2 unchanged blocks hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_private_dns_a_record.eventhub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_private_dns_a_record" "eventhub" {
	            	      [33m~[0m[0m fqdn                = "iothub-ns-iothub-swa-67128565-2d20e9e245.privatelink.servicebus.windows.net." -> (known after apply)
	            	      [33m~[0m[0m id                  = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-swa-67128565-2d20e9e245" -> (known after apply)
	            	      [33m~[0m[0m name                = "iothub-ns-iothub-swa-67128565-2d20e9e245" -> (known after apply) [31m# forces replacement[0m[0m
	            	      [33m~[0m[0m records             = [
	            	          [31m-[0m[0m "10.0.3.5",
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                = {} [90m-> null[0m[0m
	            	        [90m# (3 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_private_endpoint.iothub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_private_endpoint" "iothub" {
	            	      [33m~[0m[0m custom_dns_configs            = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m fqdn         = "iothub-ns-iothub-swa-67128565-2d20e9e245.servicebus.windows.net"
	            	              [31m-[0m[0m ip_addresses = [
	            	                  [31m-[0m[0m "10.0.3.5",
	            	                ]
	            	            },
	            	        ] -> (known after apply)
	            	      [33m~[0m[0m id                            = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateEndpoints/pep-iothub-swaxz" -> (known after apply)
	            	        name                          = "pep-iothub-swaxz"
	            	      [33m~[0m[0m network_interface             = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m id   = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/networkInterfaces/pep-iothub-swaxz.nic.215ccbbc-8d21-4029-9bf2-79a9c1f56fb7"
	            	              [31m-[0m[0m name = "pep-iothub-swaxz.nic.215ccbbc-8d21-4029-9bf2-79a9c1f56fb7"
	            	            },
	            	        ] -> (known after apply)
	            	      [33m~[0m[0m private_dns_zone_configs      = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m id                  = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateEndpoints/pep-iothub-swaxz/privateDnsZoneGroups/privateDNSZoneGroup/privateDnsZoneConfigs/privatelink.azure-devices.net"
	            	              [31m-[0m[0m name                = "privatelink.azure-devices.net"
	            	              [31m-[0m[0m private_dns_zone_id = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net"
	            	              [31m-[0m[0m record_sets         = [
	            	                  [31m-[0m[0m {
	            	                      [31m-[0m[0m fqdn         = "iothub-swaxz.privatelink.azure-devices.net"
	            	                      [31m-[0m[0m ip_addresses = [
	            	                          [31m-[0m[0m "10.0.3.4",
	            	                        ]
	            	                      [31m-[0m[0m name         = "iothub-swaxz"
	            	                      [31m-[0m[0m ttl          = 10
	            	                      [31m-[0m[0m type         = "A"
	            	                    },
	            	                ]
	            	            },
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                          = {} [90m-> null[0m[0m
	            	        [90m# (4 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m private_dns_zone_group {
	            	          [33m~[0m[0m id                   = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Network/privateEndpoints/pep-iothub-swaxz/privateDnsZoneGroups/privateDNSZoneGroup" -> (known after apply)
	            	            name                 = "privateDNSZoneGroup"
	            	            [90m# (1 unchanged attribute hidden)[0m[0m
	            	        }
	            	
	            	      [33m~[0m[0m private_service_connection {
	            	            name                              = "psc-iothub-swaxz"
	            	          [33m~[0m[0m private_connection_resource_id    = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-swaxz/providers/Microsoft.Devices/iotHubs/iothub-swaxz" -> (known after apply) [31m# forces replacement[0m[0m
	            	          [33m~[0m[0m private_ip_address                = "10.0.3.4" -> (known after apply)
	            	            [90m# (4 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 3 to add, 0 to change, 3 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/201-private-link-iothub-builtin-endpoint1460658613/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/201-private-link-iothub-builtin-endpoint1460658613/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan"
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 29 Mar 26 01:03 UTC

Success: false

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:50
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_string.suffix: Refreshing state... [id=fnfyh][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh][0m
	            	[0m[1mazurerm_private_dns_zone.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/virtualNetworks/iothub-vnet-fnfyh][0m
	            	[0m[1mazurerm_private_dns_zone.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net][0m
	            	[0m[1mazurerm_private_dns_zone.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net][0m
	            	[0m[1mazurerm_iothub.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Devices/iotHubs/iothub-fnfyh][0m
	            	[0m[1mazurerm_subnet.snet: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/virtualNetworks/iothub-vnet-fnfyh/subnets/iothub-snet-fnfyh][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net/virtualNetworkLinks/vnet-link-dps-fnfyh][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/virtualNetworkLinks/vnet-link-eventhub-fnfyh][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net/virtualNetworkLinks/vnet-link-iothub-fnfyh][0m
	            	[0m[1mazurerm_private_endpoint.iothub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateEndpoints/pep-iothub-fnfyh][0m
	            	[0m[1mazurerm_private_dns_a_record.eventhub: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-fnf-67063045-c985517e9c][0m
	            	[0m[1mazurerm_iothub_shared_access_policy.iothub_policy: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Devices/iotHubs/iothub-fnfyh/iotHubKeys/iothub-policy][0m
	            	[0m[1mazurerm_iothub_dps.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Devices/provisioningServices/test-device-fnfyh][0m
	            	[0m[1mazurerm_private_endpoint.dps: Refreshing state... [id=/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateEndpoints/pep-dps-fnfyh][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	[31m-[0m/[32m+[0m destroy and then create replacement[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_iothub.iothub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_iothub" "iothub" {
	            	      [33m~[0m[0m endpoint                      = [] -> (known after apply)
	            	      [33m~[0m[0m enrichment                    = [] -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_endpoint     = "sb://iothub-ns-iothub-fnf-67063045-c985517e9c.servicebus.windows.net/" -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_namespace    = "iothub-ns-iothub-fnf-67063045-c985517e9c" -> (known after apply)
	            	      [33m~[0m[0m event_hub_events_path         = "iothub-fnfyh" -> (known after apply)
	            	      [32m+[0m[0m event_hub_operations_endpoint = (known after apply)
	            	      [32m+[0m[0m event_hub_operations_path     = (known after apply)
	            	      [33m~[0m[0m event_hub_partition_count     = 4 -> (known after apply)
	            	      [33m~[0m[0m event_hub_retention_in_days   = 1 -> (known after apply)
	            	      [33m~[0m[0m hostname                      = "iothub-fnfyh.azure-devices.net" -> (known after apply)
	            	      [33m~[0m[0m id                            = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Devices/iotHubs/iothub-fnfyh" -> (known after apply)
	            	      [31m-[0m[0m min_tls_version               = "1.2" [90m-> null[0m[0m [31m# forces replacement[0m[0m
	            	        name                          = "iothub-fnfyh"
	            	      [33m~[0m[0m route                         = [] -> (known after apply)
	            	      [33m~[0m[0m shared_access_policy          = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "iothubowner"
	            	              [31m-[0m[0m permissions   = "RegistryWrite, ServiceConnect, DeviceConnect"
	            	              [31m-[0m[0m primary_key   = "xpdNlcS6ZrHNfZZ++JnKdR4TWpg9a+QpaAIoTLNB1ZI="
	            	              [31m-[0m[0m secondary_key = "5fpYB1Xu2HdQDCxxpLzfk+fj4xNv2bD32AIoTMSpUfU="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "service"
	            	              [31m-[0m[0m permissions   = "ServiceConnect"
	            	              [31m-[0m[0m primary_key   = "LTHTV5aMZbRxbBpUNxQf9vrj6TGP2t+adAIoTNhXGeQ="
	            	              [31m-[0m[0m secondary_key = "0hlkQS+1RFfgVrPNNNdMcHVjb760fN1sIAIoTIRFj6M="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "device"
	            	              [31m-[0m[0m permissions   = "DeviceConnect"
	            	              [31m-[0m[0m primary_key   = "sMEWeJrQka2Fi2IzX6VJPt12kdjy4gNmvAIoTLdvWo8="
	            	              [31m-[0m[0m secondary_key = "pGTC6b03qqB7SXPTIkANmbxXH3fGMAMMiAIoTMtHDoE="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "registryRead"
	            	              [31m-[0m[0m permissions   = "RegistryRead"
	            	              [31m-[0m[0m primary_key   = "8Ssu8kMMeuG+JpLZC6jWpfWSI7x6GSohRAIoTICrbmQ="
	            	              [31m-[0m[0m secondary_key = "RlpAvZdxEfUTApO++RplFaSrJhg1aIvvkAIoTFcUfL4="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "registryReadWrite"
	            	              [31m-[0m[0m permissions   = "RegistryWrite"
	            	              [31m-[0m[0m primary_key   = "Pg6YxEosuJIY5FWN+n2/plg1O+8MN0z0MAIoTEaVj9s="
	            	              [31m-[0m[0m secondary_key = "BIHM2sRnUwaLTHpkkpQMKLLCe20QTzFoUAIoTA6jWYU="
	            	            },
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m key_name      = "iothub-policy"
	            	              [31m-[0m[0m permissions   = "RegistryWrite, ServiceConnect"
	            	              [31m-[0m[0m primary_key   = "jLru10VDfQ5oY58kzLMeKzXSpzODshZyGAIoTLtS71w="
	            	              [31m-[0m[0m secondary_key = "aafR9btOfDvmGhdukSU7sULsgbvNJLeCcAIoTHfh8FM="
	            	            },
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                          = {} [90m-> null[0m[0m
	            	      [33m~[0m[0m type                          = "Microsoft.Devices/IotHubs" -> (known after apply)
	            	        [90m# (4 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m fallback_route (known after apply)
	            	      [31m-[0m[0m fallback_route {
	            	          [31m-[0m[0m condition      = "true" [90m-> null[0m[0m
	            	          [31m-[0m[0m enabled        = true [90m-> null[0m[0m
	            	          [31m-[0m[0m endpoint_names = [
	            	              [31m-[0m[0m "events",
	            	            ] [90m-> null[0m[0m
	            	          [31m-[0m[0m source         = "DeviceMessages" [90m-> null[0m[0m
	            	        }
	            	
	            	        [90m# (2 unchanged blocks hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_private_dns_a_record.eventhub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_private_dns_a_record" "eventhub" {
	            	      [33m~[0m[0m fqdn                = "iothub-ns-iothub-fnf-67063045-c985517e9c.privatelink.servicebus.windows.net." -> (known after apply)
	            	      [33m~[0m[0m id                  = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-fnf-67063045-c985517e9c" -> (known after apply)
	            	      [33m~[0m[0m name                = "iothub-ns-iothub-fnf-67063045-c985517e9c" -> (known after apply) [31m# forces replacement[0m[0m
	            	      [33m~[0m[0m records             = [
	            	          [31m-[0m[0m "10.0.3.5",
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                = {} [90m-> null[0m[0m
	            	        [90m# (3 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_private_endpoint.iothub[0m must be [1m[31mreplaced[0m
	            	[0m[31m-[0m/[32m+[0m[0m resource "azurerm_private_endpoint" "iothub" {
	            	      [33m~[0m[0m custom_dns_configs            = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m fqdn         = "iothub-ns-iothub-fnf-67063045-c985517e9c.servicebus.windows.net"
	            	              [31m-[0m[0m ip_addresses = [
	            	                  [31m-[0m[0m "10.0.3.5",
	            	                ]
	            	            },
	            	        ] -> (known after apply)
	            	      [33m~[0m[0m id                            = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateEndpoints/pep-iothub-fnfyh" -> (known after apply)
	            	        name                          = "pep-iothub-fnfyh"
	            	      [33m~[0m[0m network_interface             = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m id   = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/networkInterfaces/pep-iothub-fnfyh.nic.0b847b10-e5a2-404b-b8a9-d83f6abfd38a"
	            	              [31m-[0m[0m name = "pep-iothub-fnfyh.nic.0b847b10-e5a2-404b-b8a9-d83f6abfd38a"
	            	            },
	            	        ] -> (known after apply)
	            	      [33m~[0m[0m private_dns_zone_configs      = [
	            	          [31m-[0m[0m {
	            	              [31m-[0m[0m id                  = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateEndpoints/pep-iothub-fnfyh/privateDnsZoneGroups/privateDNSZoneGroup/privateDnsZoneConfigs/privatelink.azure-devices.net"
	            	              [31m-[0m[0m name                = "privatelink.azure-devices.net"
	            	              [31m-[0m[0m private_dns_zone_id = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net"
	            	              [31m-[0m[0m record_sets         = [
	            	                  [31m-[0m[0m {
	            	                      [31m-[0m[0m fqdn         = "iothub-fnfyh.privatelink.azure-devices.net"
	            	                      [31m-[0m[0m ip_addresses = [
	            	                          [31m-[0m[0m "10.0.3.4",
	            	                        ]
	            	                      [31m-[0m[0m name         = "iothub-fnfyh"
	            	                      [31m-[0m[0m ttl          = 10
	            	                      [31m-[0m[0m type         = "A"
	            	                    },
	            	                ]
	            	            },
	            	        ] -> (known after apply)
	            	      [31m-[0m[0m tags                          = {} [90m-> null[0m[0m
	            	        [90m# (4 unchanged attributes hidden)[0m[0m
	            	
	            	      [33m~[0m[0m private_dns_zone_group {
	            	          [33m~[0m[0m id                   = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Network/privateEndpoints/pep-iothub-fnfyh/privateDnsZoneGroups/privateDNSZoneGroup" -> (known after apply)
	            	            name                 = "privateDNSZoneGroup"
	            	            [90m# (1 unchanged attribute hidden)[0m[0m
	            	        }
	            	
	            	      [33m~[0m[0m private_service_connection {
	            	            name                              = "psc-iothub-fnfyh"
	            	          [33m~[0m[0m private_connection_resource_id    = "/subscriptions/18ca8bf0-e7e9-4450-83da-2124ec1ce0cb/resourceGroups/rg-iothub-fnfyh/providers/Microsoft.Devices/iotHubs/iothub-fnfyh" -> (known after apply) [31m# forces replacement[0m[0m
	            	          [33m~[0m[0m private_ip_address                = "10.0.3.4" -> (known after apply)
	            	            [90m# (4 unchanged attributes hidden)[0m[0m
	            	        }
	            	    }
	            	
	            	[1mPlan:[0m 3 to add, 0 to change, 3 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/201-private-link-iothub-builtin-endpoint3177356296/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/201-private-link-iothub-builtin-endpoint3177356296/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan"
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 22 Mar 26 00:30 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

No error was found.

---

## 15 Mar 26 00:40 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

No error was found.

---

## 08 Mar 26 01:00 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

No error was found.

---

## 01 Mar 26 00:58 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

No error was found.

---

## 22 Feb 26 00:44 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

No error was found.

---

## 15 Feb 26 00:52 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

No error was found.

---

## 08 Feb 26 00:26 UTC

Success: false

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:50
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mbuilding account: could not acquire access token to parse claims: clientCredentialsToken: received HTTP status 401 with response: {"error":"invalid_client","error_description":"AADSTS700213: No matching federated identity record found for presented assertion subject 'repository_owner_id:6844498:repository_id:117169328:environment:crontests'. Check your federated identity credential Subject, Audience and Issuer against the presented assertion. https://learn.microsoft.com/entra/workload-id/workload-identity-federation Trace ID: 812bf84e-0162-4cdb-9ecc-e7cb68d42a00 Correlation ID: 57808fb1-4411-420c-a71f-c59e00d85974 Timestamp: 2026-02-08 00:26:52Z","error_codes":[700213],"timestamp":"2026-02-08 00:26:52Z","trace_id":"812bf84e-0162-4cdb-9ecc-e7cb68d42a00","correlation_id":"57808fb1-4411-420c-a71f-c59e00d85974","error_uri":"https://login.microsoftonline.com/error?code=700213"}[0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with provider["registry.terraform.io/hashicorp/azurerm"],
	            	[31m│[0m [0m  on provider.tf line 11, in provider "azurerm":
	            	[31m│[0m [0m  11: provider "azurerm" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 01 Feb 26 00:14 UTC

Success: false

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:50
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mbuilding account: could not acquire access token to parse claims: clientCredentialsToken: received HTTP status 401 with response: {"error":"invalid_client","error_description":"AADSTS700213: No matching federated identity record found for presented assertion subject 'repository_owner_id:6844498:repository_id:117169328:environment:crontests'. Check your federated identity credential Subject, Audience and Issuer against the presented assertion. https://learn.microsoft.com/entra/workload-id/workload-identity-federation Trace ID: dbbcc1b1-ef84-4621-9d83-eb2fa0022c00 Correlation ID: 438fafcf-ee26-414a-9361-8e1ee1ef150f Timestamp: 2026-02-01 00:14:44Z","error_codes":[700213],"timestamp":"2026-02-01 00:14:44Z","trace_id":"dbbcc1b1-ef84-4621-9d83-eb2fa0022c00","correlation_id":"438fafcf-ee26-414a-9361-8e1ee1ef150f","error_uri":"https://login.microsoftonline.com/error?code=700213"}[0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with provider["registry.terraform.io/hashicorp/azurerm"],
	            	[31m│[0m [0m  on provider.tf line 11, in provider "azurerm":
	            	[31m│[0m [0m  11: provider "azurerm" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 25 Jan 26 00:14 UTC

Success: false

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.0

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:50
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mbuilding account: could not acquire access token to parse claims: clientCredentialsToken: received HTTP status 401 with response: {"error":"invalid_client","error_description":"AADSTS700213: No matching federated identity record found for presented assertion subject 'repository_owner_id:6844498:repository_id:117169328:environment:crontests'. Check your federated identity credential Subject, Audience and Issuer against the presented assertion. https://learn.microsoft.com/entra/workload-id/workload-identity-federation Trace ID: 260493ef-ab9b-4730-aeed-628181161200 Correlation ID: 5ea5a605-6067-4a03-8467-dcf9dcb98533 Timestamp: 2026-01-25 00:14:17Z","error_codes":[700213],"timestamp":"2026-01-25 00:14:17Z","trace_id":"260493ef-ab9b-4730-aeed-628181161200","correlation_id":"5ea5a605-6067-4a03-8467-dcf9dcb98533","error_uri":"https://login.microsoftonline.com/error?code=700213"}[0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with provider["registry.terraform.io/hashicorp/azurerm"],
	            	[31m│[0m [0m  on provider.tf line 11, in provider "azurerm":
	            	[31m│[0m [0m  11: provider "azurerm" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 18 Jan 26 00:17 UTC

Success: false

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.8.0

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:50
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mbuilding account: could not acquire access token to parse claims: clientCredentialsToken: received HTTP status 401 with response: {"error":"invalid_client","error_description":"AADSTS700213: No matching federated identity record found for presented assertion subject 'repository_owner_id:6844498:repository_id:117169328:environment:crontests'. Check your federated identity credential Subject, Audience and Issuer against the presented assertion. https://learn.microsoft.com/entra/workload-id/workload-identity-federation Trace ID: 799d22ec-96b9-4689-be9f-f005d7131d00 Correlation ID: 36ea40e5-2728-48f0-a18b-9ce4c597bf50 Timestamp: 2026-01-18 00:17:14Z","error_codes":[700213],"timestamp":"2026-01-18 00:17:14Z","trace_id":"799d22ec-96b9-4689-be9f-f005d7131d00","correlation_id":"36ea40e5-2728-48f0-a18b-9ce4c597bf50","error_uri":"https://login.microsoftonline.com/error?code=700213"}[0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with provider["registry.terraform.io/hashicorp/azurerm"],
	            	[31m│[0m [0m  on provider.tf line 11, in provider "azurerm":
	            	[31m│[0m [0m  11: provider "azurerm" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 11 Jan 26 01:41 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 04 Jan 26 01:02 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 28 Dec 25 01:27 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 21 Dec 25 01:49 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 14 Dec 25 01:20 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 07 Dec 25 01:20 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 30 Nov 25 01:27 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 02 Nov 25 01:07 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 26 Oct 25 01:05 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 19 Oct 25 01:38 UTC

Success: true

### Versions

Terraform v1.13.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 12 Oct 25 00:50 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 05 Oct 25 00:35 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 28 Sep 25 01:05 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 21 Sep 25 01:18 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 14 Sep 25 00:43 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 07 Sep 25 00:29 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 31 Aug 25 00:27 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 24 Aug 25 01:04 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 17 Aug 25 01:35 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 10 Aug 25 00:33 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 03 Aug 25 02:04 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 27 Jul 25 00:57 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 20 Jul 25 00:53 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 13 Jul 25 00:30 UTC

Success: true

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 06 Jul 25 00:42 UTC

Success: true

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 29 Jun 25 00:50 UTC

Success: true

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 15 Jun 25 00:35 UTC

Success: true

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 08 Jun 25 00:27 UTC

Success: true

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 01 Jun 25 00:58 UTC

Success: true

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 25 May 25 00:38 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 18 May 25 00:41 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 11 May 25 00:26 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_string.suffix: Refreshing state... [id=uzujt][0m
	            	[0m[1mazurerm_resource_group.rg: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt][0m
	            	[0m[1mazurerm_virtual_network.vnet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/virtualNetworks/iothub-vnet-uzujt][0m
	            	[0m[1mazurerm_private_dns_zone.iothub: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net][0m
	            	[0m[1mazurerm_private_dns_zone.dps: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net][0m
	            	[0m[1mazurerm_private_dns_zone.eventhub: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net][0m
	            	[0m[1mazurerm_iothub.iothub: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Devices/iotHubs/iothub-uzujt][0m
	            	[0m[1mazurerm_subnet.snet: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/virtualNetworks/iothub-vnet-uzujt/subnets/iothub-snet-uzujt][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.eventhub: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/virtualNetworkLinks/vnet-link-eventhub-uzujt][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.iothub: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices.net/virtualNetworkLinks/vnet-link-iothub-uzujt][0m
	            	[0m[1mazurerm_private_dns_zone_virtual_network_link.dps: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateDnsZones/privatelink.azure-devices-provisioning.net/virtualNetworkLinks/vnet-link-dps-uzujt][0m
	            	[0m[1mazurerm_private_endpoint.iothub: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateEndpoints/pep-iothub-uzujt][0m
	            	[0m[1mazurerm_private_dns_a_record.eventhub: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateDnsZones/privatelink.servicebus.windows.net/A/iothub-ns-iothub-uzu-64110445-0ab6325e19][0m
	            	[0m[1mazurerm_iothub_shared_access_policy.iothub_policy: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Devices/iotHubs/iothub-uzujt/iotHubKeys/iothub-policy][0m
	            	[0m[1mazurerm_iothub_dps.dps: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Devices/provisioningServices/test-device-uzujt][0m
	            	[0m[1mazurerm_private_endpoint.dps: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt/providers/Microsoft.Network/privateEndpoints/pep-dps-uzujt][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_resource_group.rg[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_resource_group" "rg" {
	            	        id         = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/rg-iothub-uzujt"
	            	        name       = "rg-iothub-uzujt"
	            	      [33m~[0m[0m tags       = {
	            	          [31m-[0m[0m "mapotfdemo" = "yes" [90m-> null[0m[0m
	            	        }
	            	        [90m# (2 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/201-private-link-iothub-builtin-endpoint603540912/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/201-private-link-iothub-builtin-endpoint603540912/src/quickstart/201-private-link-iothub-builtin-endpoint/tf.plan"
	Test:       	Test_Quickstarts/quickstart/201-private-link-iothub-builtin-endpoint

FailNow

---

## 04 May 25 00:30 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 27 Apr 25 00:33 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

No error was found.

---

## 20 Apr 25 01:25 UTC

Success: true

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 13 Apr 25 00:51 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 06 Apr 25 01:16 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 30 Mar 25 00:46 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 23 Mar 25 01:18 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 16 Mar 25 01:43 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 09 Mar 25 01:30 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 02 Mar 25 00:27 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 23 Feb 25 00:57 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 16 Feb 25 00:34 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 09 Feb 25 01:28 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 02 Feb 25 02:00 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 26 Jan 25 02:04 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 23 Jan 25 09:12 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 19 Jan 25 01:01 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 12 Jan 25 00:22 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 05 Jan 25 01:27 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Dec 24 01:02 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 22 Dec 24 01:03 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 15 Dec 24 03:00 UTC

Success: true

### Versions

Terraform v1.10.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 08 Dec 24 00:12 UTC

Success: false

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 01 Dec 24 00:10 UTC

Success: false

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 24 Nov 24 00:26 UTC

Success: true

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 17 Nov 24 02:50 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 10 Nov 24 03:09 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 03 Nov 24 00:27 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 27 Oct 24 00:56 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 20 Oct 24 00:58 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 13 Oct 24 00:39 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 06 Oct 24 02:10 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 03:14 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 02:44 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 00:12 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 27 Sep 24 07:22 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 22 Sep 24 00:10 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 18 Sep 24 03:24 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 08 Sep 24 00:33 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 01 Sep 24 00:33 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 25 Aug 24 00:34 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 18 Aug 24 00:32 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 11 Aug 24 00:39 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.115.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 04 Aug 24 00:36 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.114.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 01 Aug 24 01:13 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.113.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

