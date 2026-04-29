---
description: Fix schema from Palo Alto Networks Prisma Cloud Code Security API
layout: schema
name: Fix
properties_list:
- description: Unique fix suggestion identifier.
  name: fixId
  type: string
- description: Checkov policy ID associated with the fix.
  name: policyId
  type: string
- description: Human-readable policy name.
  name: policyName
  type: string
- description: Severity of the original finding.
  name: severity
  type: string
- description: IaC resource name where the fix applies.
  name: resourceName
  type: string
- description: Relative path to the file requiring the fix.
  name: filePath
  type: string
- description: Start and end line numbers of the code to be replaced.
  name: lineRange
  type: array
- description: Original code snippet that contains the misconfiguration.
  name: originalCode
  type: string
- description: Suggested replacement code that resolves the misconfiguration.
  name: suggestedCode
  type: string
- description: IaC framework of the affected file.
  name: framework
  type: string
- description: Repository where the fix applies.
  name: repositoryId
  type: string
- description: Branch where the fix applies.
  name: branch
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-code-security-api-fix-schema.json
slug: prisma-cloud-code-security-api-fix
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fix\",\n  \"description\": \"Fix schema from Palo Alto Networks Prisma Cloud Code Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-fix-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fixId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique fix suggestion identifier.\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Checkov policy ID associated with the fix.\"\n    },\n    \"policyName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable policy name.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CRITICAL\",\n        \"HIGH\",\n        \"MEDIUM\",\n        \"LOW\",\n        \"INFO\"\n      ],\n      \"description\": \"Severity of the original finding.\"\
  \n    },\n    \"resourceName\": {\n      \"type\": \"string\",\n      \"description\": \"IaC resource name where the fix applies.\"\n    },\n    \"filePath\": {\n      \"type\": \"string\",\n      \"description\": \"Relative path to the file requiring the fix.\"\n    },\n    \"lineRange\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2,\n      \"description\": \"Start and end line numbers of the code to be replaced.\"\n    },\n    \"originalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Original code snippet that contains the misconfiguration.\"\n    },\n    \"suggestedCode\": {\n      \"type\": \"string\",\n      \"description\": \"Suggested replacement code that resolves the misconfiguration.\"\n    },\n    \"framework\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Terraform\",\n        \"CloudFormation\",\n        \"Kubernetes\",\n        \"Helm\",\n        \"\
  Dockerfile\",\n        \"ARM\",\n        \"Bicep\"\n      ],\n      \"description\": \"IaC framework of the affected file.\"\n    },\n    \"repositoryId\": {\n      \"type\": \"string\",\n      \"description\": \"Repository where the fix applies.\"\n    },\n    \"branch\": {\n      \"type\": \"string\",\n      \"description\": \"Branch where the fix applies.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-fix-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Fix
---
