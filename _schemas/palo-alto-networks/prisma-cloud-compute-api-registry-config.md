---
description: RegistryConfig schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: RegistryConfig
properties_list:
- description: Registry type identifier.
  name: version
  type: string
- description: Registry URL or hostname.
  name: registry
  type: string
- description: Registry namespace or organization name.
  name: namespace
  type: string
- description: Credential store identifier for registry authentication.
  name: credentialID
  type: string
- description: Base OS for scanned images.
  name: os
  type: string
- description: Maximum number of images to scan from this registry.
  name: cap
  type: integer
- description: Number of scanner instances to use.
  name: scanners
  type: integer
- description: Specific tag to scan. Scans all tags if omitted.
  name: tag
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-registry-config-schema.json
slug: prisma-cloud-compute-api-registry-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RegistryConfig\",\n  \"description\": \"RegistryConfig schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-registry-config-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Registry type identifier.\",\n      \"enum\": [\n        \"dockerhub\",\n        \"aws\",\n        \"azure\",\n        \"gcr\",\n        \"jfrog\",\n        \"quay\",\n        \"other\"\n      ]\n    },\n    \"registry\": {\n      \"type\": \"string\",\n      \"description\": \"Registry URL or hostname.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Registry namespace or organization name.\"\n    },\n    \"credentialID\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Credential store identifier for registry authentication.\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"linux\",\n        \"windows\"\n      ],\n      \"default\": \"linux\",\n      \"description\": \"Base OS for scanned images.\"\n    },\n    \"cap\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of images to scan from this registry.\"\n    },\n    \"scanners\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of scanner instances to use.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Specific tag to scan. Scans all tags if omitted.\"\n    }\n  },\n  \"required\": [\n    \"version\",\n    \"registry\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-registry-config-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RegistryConfig
---
