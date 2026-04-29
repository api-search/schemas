---
description: ScanIntegration schema from Palo Alto Networks Prisma Cloud Code Security API
layout: schema
name: ScanIntegration
properties_list:
- description: Unique integration identifier.
  name: id
  type: string
- description: Integration name.
  name: name
  type: string
- description: CI/CD platform type.
  name: type
  type: string
- description: Repository this integration is associated with.
  name: repositoryId
  type: string
- description: Whether the integration is active.
  name: enabled
  type: boolean
- description: ''
  name: createdAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-code-security-api-scan-integration-schema.json
slug: prisma-cloud-code-security-api-scan-integration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanIntegration\",\n  \"description\": \"ScanIntegration schema from Palo Alto Networks Prisma Cloud Code Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-scan-integration-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique integration identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Integration name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"CI/CD platform type.\",\n      \"enum\": [\n        \"jenkins\",\n        \"github_actions\",\n        \"gitlab_ci\",\n        \"circleci\",\n        \"azure_pipelines\",\n        \"bitbucket_pipelines\",\n        \"other\"\n      ]\n    },\n    \"repositoryId\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Repository this integration is associated with.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the integration is active.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-scan-integration-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScanIntegration
---
