---
description: The network rule set for a container registry.
layout: schema
name: NetworkRuleSet
properties_list:
- description: The default action of allow or deny when no other rules match.
  name: defaultAction
  type: string
- description: The IP ACL rules.
  name: ipRules
  type: array
- description: The virtual network rules.
  name: virtualNetworkRules
  type: array
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-network-rule-set-schema.json
slug: azure-container-registry-network-rule-set
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: NetworkRuleSet
---
