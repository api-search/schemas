---
description: IP address for the container group.
layout: schema
name: IpAddress
properties_list:
- description: The Dns name label for the IP.
  name: dnsNameLabel
  type: string
- description: The FQDN for the IP.
  name: fqdn
  type: string
- description: The IP exposed to the public internet.
  name: ip
  type: string
- description: The list of ports exposed on the container group.
  name: ports
  type: array
- description: Specifies if the IP is exposed to the public internet or private VNET.
  name: type
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-ip-address-schema.json
slug: azure-container-instances-ip-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-ip-address-schema.json\",\n  \"title\": \"IpAddress\",\n  \"description\": \"IP address for the container group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dnsNameLabel\": {\n      \"description\": \"The Dns name label for the IP.\",\n      \"type\": \"string\"\n    },\n    \"fqdn\": {\n      \"description\": \"The FQDN for the IP.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"ip\": {\n      \"description\": \"The IP exposed to the public internet.\",\n      \"type\": \"string\"\n    },\n    \"ports\": {\n      \"description\": \"The list of ports exposed on the container group.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Port\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\":\
  \ \"Specifies if the IP is exposed to the public internet or private VNET.\",\n      \"enum\": [\n        \"Public\",\n        \"Private\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ContainerGroupIpAddressType\"\n      }\n    }\n  },\n  \"required\": [\n    \"ports\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-ip-address-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: IpAddress
---
