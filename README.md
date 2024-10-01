
# Deploys tf-module-az-resource-group for an Azure resource
Deploys the tf-module-az-resource-group into the Azure Subscription


Reference the module to a specific version (recommended):
```hcl
"git::https://github.com/BrettOJ/tf-az-module-resource-group?ref=main"
```

Manages a Resource Group.

## [Example Usage](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#example-usage)

```hcl
resource "azurerm_resource_group" "example" { name = "example" location = "West Europe" }
```

## [Arguments Reference](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#arguments-reference)

The following arguments are supported:

-   [`location`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#location) - (Required) The Azure Region where the Resource Group should exist. Changing this forces a new Resource Group to be created.
    
-   [`name`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#name) - (Required) The Name which should be used for this Resource Group. Changing this forces a new Resource Group to be created.
    

___

-   [`managed_by`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#managed_by) - (Optional) The ID of the resource or application that manages this Resource Group.
    
-   [`tags`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#tags) - (Optional) A mapping of tags which should be assigned to the Resource Group.
    

## [Attributes Reference](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#attributes-reference)

In addition to the Arguments listed above - the following Attributes are exported:

-   [`id`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#id) - The ID of the Resource Group.

## [Timeouts](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#timeouts)

The `timeouts` block allows you to specify [timeouts](https://www.terraform.io/language/resources/syntax#operation-timeouts) for certain actions:

-   [`create`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#create) - (Defaults to 90 minutes) Used when creating the Resource Group.
-   [`read`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#read) - (Defaults to 5 minutes) Used when retrieving the Resource Group.
-   [`update`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#update) - (Defaults to 90 minutes) Used when updating the Resource Group.
-   [`delete`](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#delete) - (Defaults to 90 minutes) Used when deleting the Resource Group.

## [Import](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group#import)

Resource Groups can be imported using the `resource id`, e.g.

```shell
terraform import azurerm_resource_group.example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/group1
```