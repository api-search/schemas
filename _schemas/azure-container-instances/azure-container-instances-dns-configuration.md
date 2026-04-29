---
description: DNS configuration for the container group.
layout: schema
name: DnsConfiguration
properties_list:
- description: The DNS servers for the container group.
  name: nameServers
  type: array
- description: The DNS options for the container group.
  name: options
  type: string
- description: The DNS search domains for hostname lookup in the container group.
  name: searchDomains
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-dns-configuration-schema.json
slug: azure-container-instances-dns-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-dns-configuration-schema.json\",\n  \"title\": \"DnsConfiguration\",\n  \"description\": \"DNS configuration for the container group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nameServers\": {\n      \"description\": \"The DNS servers for the container group.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"options\": {\n      \"description\": \"The DNS options for the container group.\",\n      \"type\": \"string\"\n    },\n    \"searchDomains\": {\n      \"description\": \"The DNS search domains for hostname lookup in the container group.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"nameServers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-dns-configuration-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: DnsConfiguration
---
