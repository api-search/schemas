---
description: Repository schema from Palo Alto Networks Prisma Cloud Code Security API
layout: schema
name: Repository
properties_list:
- description: Unique repository identifier in Prisma Cloud.
  name: id
  type: string
- description: Repository name.
  name: name
  type: string
- description: Repository owner or organization name.
  name: owner
  type: string
- description: Full repository name in owner/repo format.
  name: fullName
  type: string
- description: VCS provider type.
  name: sourceType
  type: string
- description: Default branch of the repository.
  name: defaultBranch
  type: string
- description: URL to the repository in the VCS provider.
  name: url
  type: string
- description: Whether the repository is publicly accessible.
  name: isPublic
  type: boolean
- description: Timestamp of the most recent scan.
  name: lastScanDate
  type: string
- description: Status of the most recent scan.
  name: lastScanStatus
  type: string
- description: Count of open errors by severity.
  name: errorCounts
  type: object
- description: Timestamp when the repository was connected.
  name: createdAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-code-security-api-repository-schema.json
slug: prisma-cloud-code-security-api-repository
source_filename: prisma-cloud-code-security-api-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Repository\",\n  \"description\": \"Repository schema from Palo Alto Networks Prisma Cloud Code Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-repository-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique repository identifier in Prisma Cloud.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Repository name.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Repository owner or organization name.\"\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full repository name in owner/repo format.\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Github\",\n        \"\
  Gitlab\",\n        \"Bitbucket\",\n        \"AzureRepos\",\n        \"githubEnterprise\",\n        \"gitlabEnterprise\",\n        \"bitbucketEnterprise\"\n      ],\n      \"description\": \"VCS provider type.\"\n    },\n    \"defaultBranch\": {\n      \"type\": \"string\",\n      \"description\": \"Default branch of the repository.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the repository in the VCS provider.\"\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is publicly accessible.\"\n    },\n    \"lastScanDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent scan.\"\n    },\n    \"lastScanStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"completed\",\n        \"running\",\n        \"failed\",\n        \"pending\"\n      ],\n      \"description\": \"Status of the most recent scan.\"\n    },\n\
  \    \"errorCounts\": {\n      \"type\": \"object\",\n      \"description\": \"Count of open errors by severity.\",\n      \"properties\": {\n        \"critical\": {\n          \"type\": \"integer\"\n        },\n        \"high\": {\n          \"type\": \"integer\"\n        },\n        \"medium\": {\n          \"type\": \"integer\"\n        },\n        \"low\": {\n          \"type\": \"integer\"\n        },\n        \"info\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the repository was connected.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-repository-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Repository
---
