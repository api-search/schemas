---
description: IP rule with specific IP or IP range in CIDR format.
layout: schema
name: IPRule
properties_list:
- description: The action of IP ACL rule.
  name: action
  type: string
- description: Specifies the IP or IP range in CIDR format. Only IPV4 address is allowed.
  name: value
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-ip-rule-schema.json
slug: azure-container-registry-ip-rule
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: IPRule
---
