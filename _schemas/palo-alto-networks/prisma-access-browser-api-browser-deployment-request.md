---
description: BrowserDeploymentRequest schema from Palo Alto Networks Prisma Access Browser Management API
layout: schema
name: BrowserDeploymentRequest
properties_list:
- description: Display name for the deployment.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Target operating system platform.
  name: platform
  type: string
- description: Default browser policy ID for this deployment.
  name: policy_id
  type: string
- description: ''
  name: update_channel
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-browser-api-browser-deployment-request-schema.json
slug: prisma-access-browser-api-browser-deployment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrowserDeploymentRequest\",\n  \"description\": \"BrowserDeploymentRequest schema from Palo Alto Networks Prisma Access Browser Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-deployment-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the deployment.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"windows\",\n        \"macos\",\n        \"linux\",\n        \"chromeos\"\n      ],\n      \"description\": \"Target operating system platform.\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Default browser policy ID for this deployment.\"\n\
  \    },\n    \"update_channel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"stable\",\n        \"beta\"\n      ],\n      \"default\": \"stable\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"platform\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-deployment-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BrowserDeploymentRequest
---
