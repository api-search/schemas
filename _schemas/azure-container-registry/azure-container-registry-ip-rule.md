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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-ip-rule-schema.json\",\n  \"title\": \"IPRule\",\n  \"description\": \"IP rule with specific IP or IP range in CIDR format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"default\": \"Allow\",\n      \"description\": \"The action of IP ACL rule.\",\n      \"enum\": [\n        \"Allow\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"Action\"\n      }\n    },\n    \"value\": {\n      \"description\": \"Specifies the IP or IP range in CIDR format. Only IPV4 address is allowed.\",\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"IPAddressOrRange\"\n    }\n  },\n  \"required\": [\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-ip-rule-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: IPRule
---
