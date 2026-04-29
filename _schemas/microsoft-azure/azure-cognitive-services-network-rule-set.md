---
description: A set of rules governing the network accessibility.
layout: schema
name: NetworkRuleSet
properties_list:
- description: The default action when no rule matches.
  name: defaultAction
  type: string
- description: The list of IP address rules.
  name: ipRules
  type: array
- description: The list of virtual network rules.
  name: virtualNetworkRules
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-network-rule-set-schema.json
slug: azure-cognitive-services-network-rule-set
source_filename: azure-cognitive-services-network-rule-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkRuleSet\",\n  \"type\": \"object\",\n  \"description\": \"A set of rules governing the network accessibility.\",\n  \"properties\": {\n    \"defaultAction\": {\n      \"type\": \"string\",\n      \"description\": \"The default action when no rule matches.\"\n    },\n    \"ipRules\": {\n      \"type\": \"array\",\n      \"description\": \"The list of IP address rules.\"\n    },\n    \"virtualNetworkRules\": {\n      \"type\": \"array\",\n      \"description\": \"The list of virtual network rules.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-network-rule-set-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: NetworkRuleSet
---
