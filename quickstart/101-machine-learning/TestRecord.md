## 27 Jul 25 00:30 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-brave-pelican][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=79405340][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=bfjihaqy][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg/providers/Microsoft.KeyVault/vaults/mldev79405340kv][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg/providers/Microsoft.Insights/components/ml-brave-pelican-appi][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg/providers/Microsoft.ContainerRegistry/registries/mldev79405340cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg/providers/Microsoft.Storage/storageAccounts/mldev79405340st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-brave-pelican-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-brave-pelican-mlw/computes/bfjihaqyinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-brave-pelican-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-brave-pelican-rg/providers/Microsoft.Insights/components/ml-brave-pelican-appi"
	            	        name                                  = "ml-brave-pelican-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-brave-pelican-appi_bd816e45-4a64-4f8b-b6e6-71a309055f11_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-brave-pelican-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning3185897753/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning3185897753/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 20 Jul 25 00:31 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_integer.suffix: Refreshing state... [id=97543532][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=enzapqkq][0m
	            	[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-sought-wren][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg/providers/Microsoft.KeyVault/vaults/mldev97543532kv][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg/providers/Microsoft.Insights/components/ml-sought-wren-appi][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg/providers/Microsoft.ContainerRegistry/registries/mldev97543532cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg/providers/Microsoft.Storage/storageAccounts/mldev97543532st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-sought-wren-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-sought-wren-mlw/computes/enzapqkqinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-sought-wren-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sought-wren-rg/providers/Microsoft.Insights/components/ml-sought-wren-appi"
	            	        name                                  = "ml-sought-wren-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-sought-wren-appi_2d5dc9f4-0026-4946-840d-85998c0fc855_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-sought-wren-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning2049806498/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning2049806498/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 13 Jul 25 01:12 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_integer.suffix: Refreshing state... [id=50327323][0m
	            	[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-assured-krill][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=mxjtzxxb][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg/providers/Microsoft.Insights/components/ml-assured-krill-appi][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg/providers/Microsoft.KeyVault/vaults/mldev50327323kv][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg/providers/Microsoft.ContainerRegistry/registries/mldev50327323cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg/providers/Microsoft.Storage/storageAccounts/mldev50327323st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-assured-krill-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-assured-krill-mlw/computes/cpu-cluster][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-assured-krill-mlw/computes/mxjtzxxbinstance][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-assured-krill-rg/providers/Microsoft.Insights/components/ml-assured-krill-appi"
	            	        name                                  = "ml-assured-krill-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-assured-krill-appi_c347589e-57c4-4b9b-8d0a-1ff03a8d6e33_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-assured-krill-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning1370009981/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning1370009981/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 06 Jul 25 01:21 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-superb-pika][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=yeltqrng][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=73379267][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg/providers/Microsoft.KeyVault/vaults/mldev73379267kv][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg/providers/Microsoft.Insights/components/ml-superb-pika-appi][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg/providers/Microsoft.ContainerRegistry/registries/mldev73379267cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg/providers/Microsoft.Storage/storageAccounts/mldev73379267st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-superb-pika-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-superb-pika-mlw/computes/yeltqrnginstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-superb-pika-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-superb-pika-rg/providers/Microsoft.Insights/components/ml-superb-pika-appi"
	            	        name                                  = "ml-superb-pika-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-superb-pika-appi_1ae1fc7b-1587-4726-a4ee-f171c97a1a37_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-superb-pika-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning900873431/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning900873431/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 29 Jun 25 00:35 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-crisp-pelican][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=27474494][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=lloogust][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg/providers/Microsoft.Insights/components/ml-crisp-pelican-appi][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg/providers/Microsoft.ContainerRegistry/registries/mldev27474494cr][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg/providers/Microsoft.KeyVault/vaults/mldev27474494kv][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg/providers/Microsoft.Storage/storageAccounts/mldev27474494st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-crisp-pelican-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-crisp-pelican-mlw/computes/lloogustinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-crisp-pelican-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-crisp-pelican-rg/providers/Microsoft.Insights/components/ml-crisp-pelican-appi"
	            	        name                                  = "ml-crisp-pelican-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-crisp-pelican-appi_1a29358b-c16c-4d69-b69a-e95c666443f6_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-crisp-pelican-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning841793309/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning841793309/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 15 Jun 25 00:30 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-faithful-chipmunk][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=71179821][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=grchnnum][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg/providers/Microsoft.ContainerRegistry/registries/mldev71179821cr][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg/providers/Microsoft.Insights/components/ml-faithful-chipmunk-appi][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg/providers/Microsoft.KeyVault/vaults/mldev71179821kv][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg/providers/Microsoft.Storage/storageAccounts/mldev71179821st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-faithful-chipmunk-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-faithful-chipmunk-mlw/computes/grchnnuminstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-faithful-chipmunk-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-faithful-chipmunk-rg/providers/Microsoft.Insights/components/ml-faithful-chipmunk-appi"
	            	        name                                  = "ml-faithful-chipmunk-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-faithful-chipmunk-appi_79ba2f70-05e2-4eec-9f1d-43703c51dde3_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-faithful-chipmunk-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning492860234/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning492860234/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 08 Jun 25 00:31 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_integer.suffix: Refreshing state... [id=63909606][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=qcxloepx][0m
	            	[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-united-jawfish][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg/providers/Microsoft.Insights/components/ml-united-jawfish-appi][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg/providers/Microsoft.KeyVault/vaults/mldev63909606kv][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg/providers/Microsoft.ContainerRegistry/registries/mldev63909606cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg/providers/Microsoft.Storage/storageAccounts/mldev63909606st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-united-jawfish-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-united-jawfish-mlw/computes/qcxloepxinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-united-jawfish-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-united-jawfish-rg/providers/Microsoft.Insights/components/ml-united-jawfish-appi"
	            	        name                                  = "ml-united-jawfish-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-united-jawfish-appi_575adbbb-3171-4085-ad09-0e1f4bdb89b6_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-united-jawfish-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning3575544495/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning3575544495/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 01 Jun 25 00:31 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-related-bird][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=mvabsyql][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=78367437][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg/providers/Microsoft.Insights/components/ml-related-bird-appi][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg/providers/Microsoft.KeyVault/vaults/mldev78367437kv][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg/providers/Microsoft.ContainerRegistry/registries/mldev78367437cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg/providers/Microsoft.Storage/storageAccounts/mldev78367437st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-related-bird-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-related-bird-mlw/computes/mvabsyqlinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-related-bird-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-related-bird-rg/providers/Microsoft.Insights/components/ml-related-bird-appi"
	            	        name                                  = "ml-related-bird-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-related-bird-appi_cbd18c88-8f7d-4291-b320-a88fdca2d507_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-related-bird-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning4290057470/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning4290057470/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 25 May 25 00:30 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-sweeping-porpoise][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=40980662][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=mkeqygax][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg/providers/Microsoft.Insights/components/ml-sweeping-porpoise-appi][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg/providers/Microsoft.KeyVault/vaults/mldev40980662kv][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg/providers/Microsoft.ContainerRegistry/registries/mldev40980662cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg/providers/Microsoft.Storage/storageAccounts/mldev40980662st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-sweeping-porpoise-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-sweeping-porpoise-mlw/computes/mkeqygaxinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-sweeping-porpoise-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-sweeping-porpoise-rg/providers/Microsoft.Insights/components/ml-sweeping-porpoise-appi"
	            	        name                                  = "ml-sweeping-porpoise-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-sweeping-porpoise-appi_6f174191-2f9a-473d-8618-0d8bd0ecefdd_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-sweeping-porpoise-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning3559415773/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning3559415773/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 18 May 25 00:29 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-proven-haddock][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=89875015][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=lugxwehl][0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg/providers/Microsoft.Insights/components/ml-proven-haddock-appi][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg/providers/Microsoft.KeyVault/vaults/mldev89875015kv][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg/providers/Microsoft.ContainerRegistry/registries/mldev89875015cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg/providers/Microsoft.Storage/storageAccounts/mldev89875015st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-proven-haddock-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-proven-haddock-mlw/computes/lugxwehlinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-proven-haddock-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-proven-haddock-rg/providers/Microsoft.Insights/components/ml-proven-haddock-appi"
	            	        name                                  = "ml-proven-haddock-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-proven-haddock-appi_465d35db-ba13-4dd8-a94a-892412f4d4ae_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-proven-haddock-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning3445511446/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning3445511446/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 11 May 25 00:50 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-merry-mink][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=32198024][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=btjoxrpf][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg/providers/Microsoft.KeyVault/vaults/mldev32198024kv][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg/providers/Microsoft.Insights/components/ml-merry-mink-appi][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg/providers/Microsoft.ContainerRegistry/registries/mldev32198024cr][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg/providers/Microsoft.Storage/storageAccounts/mldev32198024st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-merry-mink-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-merry-mink-mlw/computes/btjoxrpfinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-merry-mink-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg/providers/Microsoft.Insights/components/ml-merry-mink-appi"
	            	        name                                  = "ml-merry-mink-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-merry-mink-appi_e7d374ef-304f-4a0d-9348-c3f629d5ed81_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-merry-mink-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1m  # azurerm_resource_group.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_resource_group" "default" {
	            	        id         = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-merry-mink-rg"
	            	        name       = "ml-merry-mink-rg"
	            	      [33m~[0m[0m tags       = {
	            	          [31m-[0m[0m "mapotfdemo" = "yes" [90m-> null[0m[0m
	            	        }
	            	        [90m# (2 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 2 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning1074358128/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning1074358128/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 04 May 25 01:13 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-choice-seagull][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=vtncmvlg][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=50424482][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg/providers/Microsoft.ContainerRegistry/registries/mldev50424482cr][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg/providers/Microsoft.KeyVault/vaults/mldev50424482kv][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg/providers/Microsoft.Insights/components/ml-choice-seagull-appi][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg/providers/Microsoft.Storage/storageAccounts/mldev50424482st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-choice-seagull-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-choice-seagull-mlw/computes/vtncmvlginstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-choice-seagull-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-choice-seagull-rg/providers/Microsoft.Insights/components/ml-choice-seagull-appi"
	            	        name                                  = "ml-choice-seagull-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-choice-seagull-appi_8d6159a3-7f5d-4688-a6c9-5c5cd0decd34_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-choice-seagull-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning767159625/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning767159625/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 27 Apr 25 01:47 UTC

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
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-genuine-monitor][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=spaejodt][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=82729231][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg/providers/Microsoft.ContainerRegistry/registries/mldev82729231cr][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg/providers/Microsoft.KeyVault/vaults/mldev82729231kv][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg/providers/Microsoft.Insights/components/ml-genuine-monitor-appi][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg/providers/Microsoft.Storage/storageAccounts/mldev82729231st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-genuine-monitor-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-genuine-monitor-mlw/computes/spaejodtinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-genuine-monitor-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-genuine-monitor-rg/providers/Microsoft.Insights/components/ml-genuine-monitor-appi"
	            	        name                                  = "ml-genuine-monitor-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-genuine-monitor-appi_080ab021-b61e-48b5-b18a-4292a91c48a5_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-genuine-monitor-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning2966778375/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning2966778375/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 20 Apr 25 00:30 UTC

Success: false

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_integer.suffix: Refreshing state... [id=10087554][0m
	            	[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-magnetic-bluebird][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=mkvqgxcx][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg/providers/Microsoft.Insights/components/ml-magnetic-bluebird-appi][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg/providers/Microsoft.ContainerRegistry/registries/mldev10087554cr][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg/providers/Microsoft.KeyVault/vaults/mldev10087554kv][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg/providers/Microsoft.Storage/storageAccounts/mldev10087554st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-magnetic-bluebird-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-magnetic-bluebird-mlw/computes/mkvqgxcxinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-magnetic-bluebird-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-magnetic-bluebird-rg/providers/Microsoft.Insights/components/ml-magnetic-bluebird-appi"
	            	        name                                  = "ml-magnetic-bluebird-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-magnetic-bluebird-appi_5ca9edae-a385-481a-b5cd-d0893b630083_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-magnetic-bluebird-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning3249404419/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning3249404419/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 13 Apr 25 00:54 UTC

Success: false

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:96
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	terraform configuration not idempotent:[0m[1mrandom_pet.prefix: Refreshing state... [id=ml-fit-camel][0m
	            	[0m[1mrandom_integer.suffix: Refreshing state... [id=43283616][0m
	            	[0m[1mrandom_string.ci_prefix: Refreshing state... [id=uyqcieie][0m
	            	[0m[1mdata.azurerm_client_config.current: Reading...[0m[0m
	            	[0m[1mazurerm_resource_group.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg][0m
	            	[0m[1mdata.azurerm_client_config.current: Read complete after 0s [id=Y2xpZW50Q29uZmlncy9jbGllbnRJZD0wYThiOTgyNC05NWIzLTQ0OGMtYWJhOC05NjcwZTUxMTRhOTI7b2JqZWN0SWQ9YzRhZmRkNGMtNzU2NS00MmI3LWI5ODQtZTZhMjI0ZDEyMDQ3O3N1YnNjcmlwdGlvbklkPWY3YTYzMmE1LTQ5ZGItNGM1ZS05ODI4LWNkNjJjYjc1Mzk3MTt0ZW5hbnRJZD1mYzJiZjk2Ni1hOTg0LTQzOGMtOTNiNy1iYzVhMDZmZTdmMGQ=][0m
	            	[0m[1mazurerm_application_insights.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg/providers/Microsoft.Insights/components/ml-fit-camel-appi][0m
	            	[0m[1mazurerm_container_registry.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg/providers/Microsoft.ContainerRegistry/registries/mldev43283616cr][0m
	            	[0m[1mazurerm_key_vault.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg/providers/Microsoft.KeyVault/vaults/mldev43283616kv][0m
	            	[0m[1mazurerm_storage_account.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg/providers/Microsoft.Storage/storageAccounts/mldev43283616st][0m
	            	[0m[1mazurerm_machine_learning_workspace.default: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-fit-camel-mlw][0m
	            	[0m[1mazurerm_machine_learning_compute_instance.main: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-fit-camel-mlw/computes/uyqcieieinstance][0m
	            	[0m[1mazurerm_machine_learning_compute_cluster.compute: Refreshing state... [id=/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg/providers/Microsoft.MachineLearningServices/workspaces/ml-fit-camel-mlw/computes/cpu-cluster][0m
	            	
	            	Terraform used the selected providers to generate the following execution
	            	plan. Resource actions are indicated with the following symbols:
	            	  [33m~[0m update in-place[0m
	            	
	            	Terraform will perform the following actions:
	            	
	            	[1m  # azurerm_application_insights.default[0m will be updated in-place
	            	[0m  [33m~[0m[0m resource "azurerm_application_insights" "default" {
	            	        id                                    = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ml-fit-camel-rg/providers/Microsoft.Insights/components/ml-fit-camel-appi"
	            	        name                                  = "ml-fit-camel-appi"
	            	        tags                                  = {}
	            	      [31m-[0m[0m workspace_id                          = "/subscriptions/f7a632a5-49db-4c5e-9828-cd62cb753971/resourceGroups/ai_ml-fit-camel-appi_786508be-e68c-4c43-baf0-1c2911dd71dc_managed/providers/Microsoft.OperationalInsights/workspaces/managed-ml-fit-camel-appi-ws" [90m-> null[0m[0m
	            	        [90m# (15 unchanged attributes hidden)[0m[0m
	            	    }
	            	
	            	[1mPlan:[0m 0 to add, 1 to change, 0 to destroy.
	            	[0m[33m╷[0m[0m
	            	[33m│[0m [0m[1m[33mWarning: [0m[0m[1mArgument is deprecated[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0m[0m  with azurerm_machine_learning_compute_instance.main,
	            	[33m│[0m [0m  on compute.tf line 12, in resource "azurerm_machine_learning_compute_instance" "main":
	            	[33m│[0m [0m  12:   location                      = [4mazurerm_resource_group.default.location[0m[0m
	            	[33m│[0m [0m
	            	[33m│[0m [0mThe `azurerm_machine_learning_compute_instance` must be deployed to the
	            	[33m│[0m [0msame location as the associated `azurerm_machine_learning_workspace`
	            	[33m│[0m [0mresource, as the `location` fields must be the same the `location` field no
	            	[33m│[0m [0mlonger has any effect and will be removed in version 4.0 of the AzureRM
	            	[33m│[0m [0mProvider
	            	[33m╵[0m[0m
	            	[90m
	            	─────────────────────────────────────────────────────────────────────────────[0m
	            	
	            	Saved the plan to:
	            	/tmp/101-machine-learning392785915/src/quickstart/101-machine-learning/tf.plan
	            	
	            	To perform exactly these actions, run the following command to apply:
	            	    terraform apply "/tmp/101-machine-learning392785915/src/quickstart/101-machine-learning/tf.plan"
	Test:       	Test_Quickstarts/quickstart/101-machine-learning

FailNow

---

## 06 Apr 25 00:28 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 30 Mar 25 01:11 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 23 Mar 25 00:29 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 16 Mar 25 01:21 UTC

Success: true

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 09 Mar 25 00:46 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 02 Mar 25 01:08 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

No error was found.

---

## 23 Feb 25 01:58 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 16 Feb 25 01:36 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 09 Feb 25 00:29 UTC

Success: true

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 02 Feb 25 00:29 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 26 Jan 25 01:08 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 23 Jan 25 09:46 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error

No error was found.

---

## 19 Jan 25 01:05 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 12 Jan 25 00:43 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 05 Jan 25 00:36 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Dec 24 00:35 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 22 Dec 24 00:41 UTC

Success: true

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 15 Dec 24 00:25 UTC

Success: true

### Versions

Terraform v1.10.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 08 Dec 24 00:15 UTC

Success: false

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 01 Dec 24 00:13 UTC

Success: false

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 24 Nov 24 00:35 UTC

Success: true

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 17 Nov 24 02:20 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 10 Nov 24 00:25 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 03 Nov 24 01:03 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 27 Oct 24 01:12 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 20 Oct 24 00:38 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 13 Oct 24 01:26 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 06 Oct 24 00:40 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 03:46 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 02:47 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 00:14 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 27 Sep 24 08:08 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 22 Sep 24 00:12 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 18 Sep 24 03:26 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 08 Sep 24 01:10 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 01 Sep 24 01:10 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 25 Aug 24 01:08 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 18 Aug 24 01:10 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 11 Aug 24 01:02 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.115.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 04 Aug 24 01:07 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.114.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 01 Aug 24 01:51 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.113.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 28 Jan 24 01:07 UTC

Success: true

### Versions

Terraform v1.6.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.89.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 21 Jan 24 00:27 UTC

Success: true

### Versions

Terraform v1.6.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.88.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 14 Jan 24 01:00 UTC

Success: true

### Versions

Terraform v1.6.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.87.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 07 Jan 24 00:59 UTC

Success: true

### Versions

Terraform v1.6.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.86.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 31 Dec 23 00:54 UTC

Success: true

### Versions

Terraform v1.6.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.85.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 24 Dec 23 00:29 UTC

Success: true

### Versions

Terraform v1.6.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.85.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 17 Dec 23 01:03 UTC

Success: true

### Versions

Terraform v1.6.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.85.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 10 Dec 23 00:50 UTC

Success: true

### Versions

Terraform v1.6.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.84.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 04 Dec 23 02:58 UTC

Success: true

### Versions

Terraform v1.6.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.83.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 26 Nov 23 04:17 UTC

Success: true

### Versions

Terraform v1.6.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.82.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 19 Nov 23 01:02 UTC

Success: true

### Versions

Terraform v1.6.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.81.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 14 Nov 23 14:43 UTC

Success: true

### Versions

Terraform v1.6.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.80.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 12 Nov 23 03:19 UTC

Success: false

### Versions

Terraform v1.6.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.80.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 05 Nov 23 03:46 UTC

Success: false

### Versions

Terraform v1.6.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.79.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 29 Oct 23 03:49 UTC

Success: true

### Versions

Terraform v1.6.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.78.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 22 Oct 23 01:12 UTC

Success: false

### Versions

Terraform v1.5.7
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.77.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 15 Oct 23 01:03 UTC

Success: true

### Versions

Terraform v1.5.7
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.76.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 08 Oct 23 00:56 UTC

Success: true

### Versions

Terraform v1.5.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.75.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 01 Oct 23 02:47 UTC

Success: false

### Versions

Terraform v1.5.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.75.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 24 Sep 23 00:52 UTC

Success: false

### Versions

Terraform v1.5.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.74.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 20 Sep 23 07:05 UTC

Success: true

### Versions

Terraform v1.5.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.73.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 17 Sep 23 00:53 UTC

Success: true

### Versions

Terraform v1.5.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.73.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 10 Sep 23 00:58 UTC

Success: true

### Versions

Terraform v1.5.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.72.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 03 Sep 23 02:05 UTC

Success: true

### Versions

Terraform v1.5.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.71.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 27 Aug 23 01:00 UTC

Success: true

### Versions

Terraform v1.5.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.71.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 20 Aug 23 02:06 UTC

Success: true

### Versions

Terraform v1.5.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.70.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 13 Aug 23 02:00 UTC

Success: true

### Versions

Terraform v1.5.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.69.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 06 Aug 23 02:24 UTC

Success: true

### Versions

Terraform v1.5.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.68.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 30 Jul 23 02:06 UTC

Success: true

### Versions

Terraform v1.5.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.67.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 16 Jul 23 01:00 UTC

Success: true

### Versions

Terraform v1.5.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.65.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 09 Jul 23 02:24 UTC

Success: true

### Versions

Terraform v1.5.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.64.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 02 Jul 23 02:12 UTC

Success: true

### Versions

Terraform v1.5.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.63.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 25 Jun 23 01:36 UTC

Success: true

### Versions

Terraform v1.5.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.62.1
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 18 Jun 23 02:21 UTC

Success: true

### Versions

Terraform v1.4.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.61.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 11 Jun 23 02:03 UTC

Success: false

### Versions

Terraform v1.4.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.60.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 04 Jun 23 02:18 UTC

Success: true

### Versions

Terraform v1.4.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.59.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 28 May 23 01:52 UTC

Success: false

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.58.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 21 May 23 00:56 UTC

Success: true

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.57.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 14 May 23 00:53 UTC

Success: true

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.56.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 07 May 23 02:25 UTC

Success: true

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.55.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 30 Apr 23 01:59 UTC

Success: false

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.54.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 23 Apr 23 00:53 UTC

Success: true

### Versions

Terraform v1.4.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.53.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 16 Apr 23 02:13 UTC

Success: true

### Versions

Terraform v1.4.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.52.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 09 Apr 23 02:11 UTC

Success: true

### Versions

Terraform v1.4.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.51.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 02 Apr 23 00:51 UTC

Success: true

### Versions

Terraform v1.4.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.50.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 26 Mar 23 01:28 UTC

Success: true

### Versions

Terraform v1.4.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.49.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 19 Mar 23 00:58 UTC

Success: true

### Versions

Terraform v1.4.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.48.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 12 Mar 23 00:54 UTC

Success: true

### Versions

Terraform v1.3.8
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.47.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 08 Mar 23 15:33 UTC

Success: true

### Versions

Terraform v1.3.8
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.46.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 27 Feb 23 02:30 UTC

Success: true

### Versions

Terraform v1.3.8
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.45.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 19 Feb 23 00:52 UTC

Success: false

### Versions

Terraform v1.3.7
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v2.76.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 12 Feb 23 00:47 UTC

Success: false

### Versions

Terraform v1.3.7
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v2.76.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 05 Feb 23 00:19 UTC

Success: false

### Versions

Terraform v1.3.7
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v2.76.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

