---
type: docs
title: "rad group CLI reference"
linkTitle: "rad group"
slug: rad_group
url: /reference/cli/rad_group/
description: "Details on the rad group Radius CLI command"
---
## rad group

Manage resource groups

### Synopsis

Manage resource groups
		
Resource groups are used to organize and manage Radius resources. They often contain resources that share a common lifecycle or unit of deployment.

A Radius Application and its resources can span one or more resource groups, and do not have to be in the same resource group as the Radius Environment into which it's being deployed into.

Note that these resource groups are separate from the Azure cloud provider and Azure resource groups configured with the cloud provider.


### Examples

```

# List resource groups in default workspace
rad group list

# Create resource group in specified workspace
rad group create prod -w localWorkspace

# Delete resource group in default workspace
rad group delete prod

# Show details of resource group in default workspace
rad group show dev

```

### Options

```
  -h, --help   help for group
```

### Options inherited from parent commands

```
      --config string   config file (default "$HOME/.rad/config.yaml")
  -o, --output string   output format (supported formats are json, table) (default "table")
```

### SEE ALSO

* [rad]({{< ref rad.md >}})	 - Radius CLI
* [rad group create]({{< ref rad_group_create.md >}})	 - Create a new resource group
* [rad group delete]({{< ref rad_group_delete.md >}})	 - Delete a resource group
* [rad group list]({{< ref rad_group_list.md >}})	 - List resource groups within current/specified workspace
* [rad group show]({{< ref rad_group_show.md >}})	 - Show the details of a resource group
* [rad group switch]({{< ref rad_group_switch.md >}})	 - Switch default resource group scope

