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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-network-rule-set-schema.json\",\n  \"title\": \"NetworkRuleSet\",\n  \"description\": \"The network rule set for a container registry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultAction\": {\n      \"default\": \"Allow\",\n      \"description\": \"The default action of allow or deny when no other rules match.\",\n      \"enum\": [\n        \"Allow\",\n        \"Deny\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"DefaultAction\"\n      }\n    },\n    \"ipRules\": {\n      \"description\": \"The IP ACL rules.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/IPRule\"\n      },\n      \"type\": \"array\"\n    },\n    \"virtualNetworkRules\": {\n      \"description\": \"The\
  \ virtual network rules.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/VirtualNetworkRule\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"defaultAction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-network-rule-set-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: NetworkRuleSet
---
