---
description: BrowserDeployment schema from Palo Alto Networks Prisma Access Browser Management API
layout: schema
name: BrowserDeployment
properties_list:
- description: Unique identifier of the deployment.
  name: deployment_id
  type: string
- description: Display name of the deployment.
  name: name
  type: string
- description: Description of the deployment configuration.
  name: description
  type: string
- description: Target operating system platform.
  name: platform
  type: string
- description: Default browser policy assigned to users in this deployment.
  name: policy_id
  type: string
- description: Browser update channel for this deployment.
  name: update_channel
  type: string
- description: Number of devices in this deployment.
  name: device_count
  type: integer
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-browser-api-browser-deployment-schema.json
slug: prisma-access-browser-api-browser-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrowserDeployment\",\n  \"description\": \"BrowserDeployment schema from Palo Alto Networks Prisma Access Browser Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-deployment-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployment_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the deployment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the deployment.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the deployment configuration.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"windows\",\n        \"macos\",\n        \"linux\",\n        \"chromeos\"\n      ],\n      \"description\"\
  : \"Target operating system platform.\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Default browser policy assigned to users in this deployment.\"\n    },\n    \"update_channel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"stable\",\n        \"beta\"\n      ],\n      \"description\": \"Browser update channel for this deployment.\"\n    },\n    \"device_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of devices in this deployment.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-deployment-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BrowserDeployment
---
