## 27 Jul 25 01:30 UTC

Success: false

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-wired-seagull-plan" / Resource Group "web-app-linux-java-wired-seagull-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed." Details=[{"Message":"Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"70007","Message":"Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","MessageTemplate":"Operation cannot be completed without additional quota. \r\nAdditional details - Location: {0} \r\nCurrent Limit ({1}): {2} \r\nCurrent Usage: {3}\r\nAmount required for this deployment ({1}): {4} \r\n(Minimum) New Limit that you should request to enable this deployment: {5}. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","Parameters":["","Standard VMs","0","0","0","0"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 20 Jul 25 01:33 UTC

Success: false

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-fair-quetzal-plan" / Resource Group "web-app-linux-java-fair-quetzal-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed." Details=[{"Message":"Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"70007","Message":"Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","MessageTemplate":"Operation cannot be completed without additional quota. \r\nAdditional details - Location: {0} \r\nCurrent Limit ({1}): {2} \r\nCurrent Usage: {3}\r\nAmount required for this deployment ({1}): {4} \r\n(Minimum) New Limit that you should request to enable this deployment: {5}. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","Parameters":["","Standard VMs","0","0","0","0"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 13 Jul 25 00:48 UTC

Success: false

### Versions

Terraform v1.12.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-sincere-worm-plan" / Resource Group "web-app-linux-java-sincere-worm-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed." Details=[{"Message":"Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"70007","Message":"Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","MessageTemplate":"Operation cannot be completed without additional quota. \r\nAdditional details - Location: {0} \r\nCurrent Limit ({1}): {2} \r\nCurrent Usage: {3}\r\nAmount required for this deployment ({1}): {4} \r\n(Minimum) New Limit that you should request to enable this deployment: {5}. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","Parameters":["","Standard VMs","0","0","0","0"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 06 Jul 25 01:38 UTC

Success: false

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-main-marlin-plan" / Resource Group "web-app-linux-java-main-marlin-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed." Details=[{"Message":"Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"70007","Message":"Operation cannot be completed without additional quota. \r\nAdditional details - Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","MessageTemplate":"Operation cannot be completed without additional quota. \r\nAdditional details - Location: {0} \r\nCurrent Limit ({1}): {2} \r\nCurrent Usage: {3}\r\nAmount required for this deployment ({1}): {4} \r\n(Minimum) New Limit that you should request to enable this deployment: {5}. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","Parameters":["","Standard VMs","0","0","0","0"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 29 Jun 25 01:13 UTC

Success: false

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-robust-woodcock-plan" / Resource Group "web-app-linux-java-robust-woodcock-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="Operation cannot be completed without additional quota. \r\nAdditional details- Location: East US \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed." Details=[{"Message":"Operation cannot be completed without additional quota. \r\nAdditional details- Location: East US \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"70007","Message":"Operation cannot be completed without additional quota. \r\nAdditional details- Location: East US \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","MessageTemplate":"Operation cannot be completed without additional quota. \r\nAdditional details- Location: {0} \r\nCurrent Limit ({1}): {2} \r\nCurrent Usage: {3}\r\nAmount required for this deployment ({1}): {4} \r\n(Minimum) New Limit that you should request to enable this deployment: {5}. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","Parameters":["East US","Standard VMs","0","0","0","0"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 15 Jun 25 01:15 UTC

Success: false

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-quiet-albacore-plan" / Resource Group "web-app-linux-java-quiet-albacore-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="Operation cannot be completed without additional quota. \r\nAdditional details- Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed." Details=[{"Message":"Operation cannot be completed without additional quota. \r\nAdditional details- Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"70007","Message":"Operation cannot be completed without additional quota. \r\nAdditional details- Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","MessageTemplate":"Operation cannot be completed without additional quota. \r\nAdditional details- Location: {0} \r\nCurrent Limit ({1}): {2} \r\nCurrent Usage: {3}\r\nAmount required for this deployment ({1}): {4} \r\n(Minimum) New Limit that you should request to enable this deployment: {5}. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","Parameters":["","Standard VMs","0","0","0","0"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 08 Jun 25 00:29 UTC

Success: false

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-trusty-wolf-plan" / Resource Group "web-app-linux-java-trusty-wolf-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="Operation cannot be completed without additional quota. \r\nAdditional details- Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed." Details=[{"Message":"Operation cannot be completed without additional quota. \r\nAdditional details- Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"70007","Message":"Operation cannot be completed without additional quota. \r\nAdditional details- Location:  \r\nCurrent Limit (Standard VMs): 0 \r\nCurrent Usage: 0\r\nAmount required for this deployment (Standard VMs): 0 \r\n(Minimum) New Limit that you should request to enable this deployment: 0. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","MessageTemplate":"Operation cannot be completed without additional quota. \r\nAdditional details- Location: {0} \r\nCurrent Limit ({1}): {2} \r\nCurrent Usage: {3}\r\nAmount required for this deployment ({1}): {4} \r\n(Minimum) New Limit that you should request to enable this deployment: {5}. \r\nNote that if you experience multiple scaling operations failing (in addition to this one) and need to accommodate the aggregate quota requirements of these operations, you will need to request a higher quota limit than the one currently displayed.","Parameters":["","Standard VMs","0","0","0","0"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 01 Jun 25 01:09 UTC

Success: false

### Versions

Terraform v1.12.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-credible-skink-plan" / Resource Group "web-app-linux-java-credible-skink-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 25 May 25 01:45 UTC

Success: false

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-premium-sculpin-plan" / Resource Group "web-app-linux-java-premium-sculpin-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 18 May 25 01:38 UTC

Success: false

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-sincere-cicada-plan" / Resource Group "web-app-linux-java-sincere-cicada-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 11 May 25 00:23 UTC

Success: false

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-choice-stinkbug-plan" / Resource Group "web-app-linux-java-choice-stinkbug-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 04 May 25 00:43 UTC

Success: false

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-select-ladybug-plan" / Resource Group "web-app-linux-java-select-ladybug-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 27 Apr 25 01:22 UTC

Success: false

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.2

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-related-mackerel-plan" / Resource Group "web-app-linux-java-related-mackerel-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 20 Apr 25 01:37 UTC

Success: false

### Versions

Terraform v1.11.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-known-guinea-plan" / Resource Group "web-app-linux-java-known-guinea-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 13 Apr 25 00:51 UTC

Success: false

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-model-bunny-plan" / Resource Group "web-app-linux-java-model-bunny-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 06 Apr 25 00:52 UTC

Success: false

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-special-grouse-plan" / Resource Group "web-app-linux-java-special-grouse-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 30 Mar 25 00:29 UTC

Success: false

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:52
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-first-sheep-plan" / Resource Group "web-app-linux-java-first-sheep-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 23 Mar 25 00:59 UTC

Success: false

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:51
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-star-parrot-plan" / Resource Group "web-app-linux-java-star-parrot-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 16 Mar 25 02:04 UTC

Success: false

### Versions

Terraform v1.11.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

### Error

Error:
	Error Trace:	/home/runtimeuser/go/pkg/mod/github.com/gruntwork-io/terratest@v0.48.1/modules/terraform/apply.go:34
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:111
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:91
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:59
	            				/home/runtimeuser/go/pkg/mod/github.com/!azure/terraform-module-test-helper@v0.31.0/e2etest.go:55
	            				/src/test/e2e/quickstart_test.go:51
	Error:      	Received unexpected error:
	            	FatalError{Underlying: error while running command: exit status 1; [31m╷[0m[0m
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-amused-chow-plan" / Resource Group "web-app-linux-java-amused-chow-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 09 Mar 25 00:20 UTC

Success: false

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

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
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-sacred-boar-plan" / Resource Group "web-app-linux-java-sacred-boar-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 02 Mar 25 00:41 UTC

Success: false

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.1
+ provider registry.terraform.io/hashicorp/random v3.7.1

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
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-patient-pig-plan" / Resource Group "web-app-linux-java-patient-pig-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 23 Feb 25 01:27 UTC

Success: false

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

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
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-adapting-monitor-plan" / Resource Group "web-app-linux-java-adapting-monitor-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 16 Feb 25 01:13 UTC

Success: false

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

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
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-obliging-werewolf-plan" / Resource Group "web-app-linux-java-obliging-werewolf-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 09 Feb 25 01:48 UTC

Success: false

### Versions

Terraform v1.10.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

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
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-neat-adder-plan" / Resource Group "web-app-linux-java-neat-adder-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 02 Feb 25 01:33 UTC

Success: false

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

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
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-worthy-honeybee-plan" / Resource Group "web-app-linux-java-worthy-honeybee-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 26 Jan 25 00:28 UTC

Success: false

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

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
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-current-crayfish-plan" / Resource Group "web-app-linux-java-current-crayfish-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 23 Jan 25 09:26 UTC

Success: false

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

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
	            	[31m│[0m [0m[1m[31mError: [0m[0m[1mcreating/updating App Service Plan: (Server Farm Name "web-app-linux-java-funny-wren-plan" / Resource Group "web-app-linux-java-funny-wren-dev-rg"): web.AppServicePlansClient#CreateOrUpdate: Failure sending request: StatusCode=401 -- Original Error: Code="Unauthorized" Message="This region has quota of 0 instances for your subscription. Try selecting different region or SKU." Details=[{"Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU."},{"Code":"Unauthorized"},{"ErrorEntity":{"Code":"Unauthorized","ExtendedCode":"52039","Message":"This region has quota of 0 instances for your subscription. Try selecting different region or SKU.","MessageTemplate":"{0}. Try selecting different region or SKU.","Parameters":["This region has quota of 0 instances for your subscription"]}}][0m
	            	[31m│[0m [0m
	            	[31m│[0m [0m[0m  with azurerm_app_service_plan.default,
	            	[31m│[0m [0m  on app_service.tf line 2, in resource "azurerm_app_service_plan" "default":
	            	[31m│[0m [0m   2: resource "azurerm_app_service_plan" "default" [4m{[0m[0m
	            	[31m│[0m [0m
	            	[31m╵[0m[0m}
	Test:       	Test_Quickstarts/quickstart/101-web-app-linux-java

FailNow

---

## 19 Jan 25 00:27 UTC

Success: false

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 12 Jan 25 00:24 UTC

Success: false

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 05 Jan 25 00:15 UTC

Success: false

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Dec 24 01:54 UTC

Success: false

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 22 Dec 24 01:25 UTC

Success: false

### Versions

Terraform v1.10.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 15 Dec 24 01:29 UTC

Success: false

### Versions

Terraform v1.10.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 08 Dec 24 00:14 UTC

Success: false

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 01 Dec 24 00:12 UTC

Success: false

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 24 Nov 24 01:59 UTC

Success: false

### Versions

Terraform v1.9.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 17 Nov 24 01:45 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 10 Nov 24 02:48 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.117.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 03 Nov 24 00:39 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 27 Oct 24 01:48 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 20 Oct 24 02:22 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 13 Oct 24 00:56 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 06 Oct 24 02:49 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 03:26 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 02:46 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 29 Sep 24 00:13 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 27 Sep 24 08:22 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 22 Sep 24 00:15 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 18 Sep 24 03:28 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.3

### Error



---

## 08 Sep 24 00:43 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 01 Sep 24 00:44 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 25 Aug 24 00:47 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 18 Aug 24 00:43 UTC

Success: false

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.116.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 11 Aug 24 00:50 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.115.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 04 Aug 24 00:46 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.114.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 01 Aug 24 01:25 UTC

Success: true

### Versions

Terraform v1.9.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.113.0
+ provider registry.terraform.io/hashicorp/random v3.6.2

### Error



---

## 28 Jan 24 00:49 UTC

Success: true

### Versions

Terraform v1.6.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.89.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 21 Jan 24 05:10 UTC

Success: false

### Versions

Terraform v1.6.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.88.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 14 Jan 24 00:44 UTC

Success: true

### Versions

Terraform v1.6.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.87.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 07 Jan 24 00:40 UTC

Success: true

### Versions

Terraform v1.6.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.86.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 31 Dec 23 00:40 UTC

Success: true

### Versions

Terraform v1.6.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.85.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 24 Dec 23 01:15 UTC

Success: true

### Versions

Terraform v1.6.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.85.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 17 Dec 23 00:45 UTC

Success: true

### Versions

Terraform v1.6.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.85.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 10 Dec 23 00:28 UTC

Success: true

### Versions

Terraform v1.6.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.84.0
+ provider registry.terraform.io/hashicorp/random v3.6.0

### Error



---

## 04 Dec 23 02:42 UTC

Success: true

### Versions

Terraform v1.6.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.83.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 26 Nov 23 03:59 UTC

Success: true

### Versions

Terraform v1.6.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.82.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 19 Nov 23 05:55 UTC

Success: true

### Versions

Terraform v1.6.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.81.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 12 Nov 23 02:22 UTC

Success: true

### Versions

Terraform v1.6.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.80.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 05 Nov 23 02:50 UTC

Success: true

### Versions

Terraform v1.6.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.79.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 29 Oct 23 02:28 UTC

Success: true

### Versions

Terraform v1.6.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.78.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 22 Oct 23 07:05 UTC

Success: true

### Versions

Terraform v1.5.7
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.77.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 15 Oct 23 06:50 UTC

Success: true

### Versions

Terraform v1.5.7
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.76.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 08 Oct 23 06:27 UTC

Success: true

### Versions

Terraform v1.5.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.75.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 01 Oct 23 01:58 UTC

Success: true

### Versions

Terraform v1.5.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.75.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 24 Sep 23 06:08 UTC

Success: true

### Versions

Terraform v1.5.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.74.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 20 Sep 23 12:28 UTC

Success: true

### Versions

Terraform v1.5.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.73.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 17 Sep 23 06:10 UTC

Success: false

### Versions



### Error


[0m[1mInitializing the backend...[0m

[0m[1mInitializing provider plugins...[0m
- Finding hashicorp/random versions matching ">= 3.0.0"...
- Finding hashicorp/azurerm versions matching ">= 3.0.0, < 4.0.0"...
- Installing hashicorp/azurerm v3.73.0...
- Installing hashicorp/random v3.5.1...
- Installed hashicorp/random v3.5.1 (signed by HashiCorp)
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mFailed to install provider[0m
[31m│[0m [0m
[31m│[0m [0m[0mError while installing hashicorp/azurerm v3.73.0: write
[31m│[0m [0m.terraform/providers/registry.terraform.io/hashicorp/azurerm/3.73.0/linux_amd64/terraform-provider-azurerm_v3.73.0_x5:
[31m│[0m [0mno space left on device
[31m╵[0m[0m
[0m[0m

---

## 10 Sep 23 06:21 UTC

Success: true

### Versions

Terraform v1.5.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.72.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 03 Sep 23 01:34 UTC

Success: true

### Versions

Terraform v1.5.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.71.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 27 Aug 23 06:39 UTC

Success: true

### Versions

Terraform v1.5.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.71.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 20 Aug 23 01:25 UTC

Success: true

### Versions

Terraform v1.5.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.70.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 13 Aug 23 01:21 UTC

Success: true

### Versions

Terraform v1.5.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.69.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 06 Aug 23 01:32 UTC

Success: true

### Versions

Terraform v1.5.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.68.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 30 Jul 23 01:21 UTC

Success: true

### Versions

Terraform v1.5.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.67.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 16 Jul 23 05:56 UTC

Success: true

### Versions

Terraform v1.5.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.65.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 09 Jul 23 01:27 UTC

Success: true

### Versions

Terraform v1.5.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.64.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 02 Jul 23 01:24 UTC

Success: true

### Versions

Terraform v1.5.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.63.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 25 Jun 23 03:50 UTC

Success: true

### Versions

Terraform v1.5.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.62.1
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 18 Jun 23 01:30 UTC

Success: true

### Versions

Terraform v1.4.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.61.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 11 Jun 23 01:28 UTC

Success: true

### Versions

Terraform v1.4.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.60.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 04 Jun 23 01:30 UTC

Success: true

### Versions

Terraform v1.4.6
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.59.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 28 May 23 01:18 UTC

Success: true

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.58.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 21 May 23 00:12 UTC

Success: true

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.57.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 14 May 23 00:12 UTC

Success: true

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.56.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 07 May 23 01:31 UTC

Success: true

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.55.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 30 Apr 23 01:32 UTC

Success: true

### Versions

Terraform v1.4.5
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.54.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 23 Apr 23 00:14 UTC

Success: true

### Versions

Terraform v1.4.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.53.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 16 Apr 23 01:39 UTC

Success: true

### Versions

Terraform v1.4.3
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.52.0
+ provider registry.terraform.io/hashicorp/random v3.5.1

### Error



---

## 09 Apr 23 01:44 UTC

Success: true

### Versions

Terraform v1.4.2
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.51.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 02 Apr 23 00:23 UTC

Success: true

### Versions

Terraform v1.4.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.50.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 26 Mar 23 00:55 UTC

Success: true

### Versions

Terraform v1.4.1
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.49.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 19 Mar 23 00:27 UTC

Success: true

### Versions

Terraform v1.4.0
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.48.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 12 Mar 23 00:26 UTC

Success: true

### Versions

Terraform v1.3.8
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.47.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 08 Mar 23 15:06 UTC

Success: true

### Versions

Terraform v1.3.8
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.46.0
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 24 Feb 23 07:09 UTC

Success: true

### Versions

Terraform v1.3.8
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v3.44.1
+ provider registry.terraform.io/hashicorp/random v3.4.3

### Error



---

## 19 Feb 23 00:53 UTC

Success: false

### Versions



### Error

[31m[0mThere are some problems with the configuration, described below.

The Terraform configuration must be valid before initialization so that
Terraform can determine which modules and providers need to be installed.[0m[0m
[33m[33m╷[0m[0m
[33m│[0m [0m[1m[33mWarning: [0m[0m[1mVersion constraints inside provider configuration blocks are deprecated[0m
[33m│[0m [0m
[33m│[0m [0m[0m  on main.tf line 2, in provider "azurerm":
[33m│[0m [0m   2:   version = [4m"=1.36.0"[0m[0m
[33m│[0m [0m
[33m│[0m [0mTerraform 0.13 and earlier allowed provider version constraints inside the
[33m│[0m [0mprovider configuration block, but that is now deprecated and will be
[33m│[0m [0mremoved in a future version of Terraform. To silence this warning, move the
[33m│[0m [0mprovider version constraint into the required_providers block.
[33m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 2, in variable "name":
[31m│[0m [0m   2:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 8, in variable "environment":
[31m│[0m [0m   8:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 14, in variable "location":
[31m│[0m [0m  14:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 20, in variable "dns_prefix":
[31m│[0m [0m  20:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 26, in variable "plan_tier":
[31m│[0m [0m  26:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 32, in variable "plan_sku":
[31m│[0m [0m  32:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m

---

## 12 Feb 23 00:39 UTC

Success: false

### Versions



### Error

[31m[0mThere are some problems with the configuration, described below.

The Terraform configuration must be valid before initialization so that
Terraform can determine which modules and providers need to be installed.[0m[0m
[33m[33m╷[0m[0m
[33m│[0m [0m[1m[33mWarning: [0m[0m[1mVersion constraints inside provider configuration blocks are deprecated[0m
[33m│[0m [0m
[33m│[0m [0m[0m  on main.tf line 2, in provider "azurerm":
[33m│[0m [0m   2:   version = [4m"=1.36.0"[0m[0m
[33m│[0m [0m
[33m│[0m [0mTerraform 0.13 and earlier allowed provider version constraints inside the
[33m│[0m [0mprovider configuration block, but that is now deprecated and will be
[33m│[0m [0mremoved in a future version of Terraform. To silence this warning, move the
[33m│[0m [0mprovider version constraint into the required_providers block.
[33m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 2, in variable "name":
[31m│[0m [0m   2:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 8, in variable "environment":
[31m│[0m [0m   8:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 14, in variable "location":
[31m│[0m [0m  14:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 20, in variable "dns_prefix":
[31m│[0m [0m  20:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 26, in variable "plan_tier":
[31m│[0m [0m  26:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 32, in variable "plan_sku":
[31m│[0m [0m  32:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m

---

## 05 Feb 23 00:14 UTC

Success: false

### Versions



### Error

[31m[0mThere are some problems with the configuration, described below.

The Terraform configuration must be valid before initialization so that
Terraform can determine which modules and providers need to be installed.[0m[0m
[33m[33m╷[0m[0m
[33m│[0m [0m[1m[33mWarning: [0m[0m[1mVersion constraints inside provider configuration blocks are deprecated[0m
[33m│[0m [0m
[33m│[0m [0m[0m  on main.tf line 2, in provider "azurerm":
[33m│[0m [0m   2:   version = [4m"=1.36.0"[0m[0m
[33m│[0m [0m
[33m│[0m [0mTerraform 0.13 and earlier allowed provider version constraints inside the
[33m│[0m [0mprovider configuration block, but that is now deprecated and will be
[33m│[0m [0mremoved in a future version of Terraform. To silence this warning, move the
[33m│[0m [0mprovider version constraint into the required_providers block.
[33m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 2, in variable "name":
[31m│[0m [0m   2:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 8, in variable "environment":
[31m│[0m [0m   8:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 14, in variable "location":
[31m│[0m [0m  14:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 20, in variable "dns_prefix":
[31m│[0m [0m  20:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 26, in variable "plan_tier":
[31m│[0m [0m  26:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m
[31m[31m╷[0m[0m
[31m│[0m [0m[1m[31mError: [0m[0m[1mInvalid quoted type constraints[0m
[31m│[0m [0m
[31m│[0m [0m[0m  on variables.tf line 32, in variable "plan_sku":
[31m│[0m [0m  32:   type        = [4m"string"[0m[0m
[31m│[0m [0m
[31m│[0m [0mTerraform 0.11 and earlier required type constraints to be given in quotes,
[31m│[0m [0mbut that form is now deprecated and will be removed in a future version of
[31m│[0m [0mTerraform. Remove the quotes around "string".
[31m╵[0m[0m
[0m[0m

---

