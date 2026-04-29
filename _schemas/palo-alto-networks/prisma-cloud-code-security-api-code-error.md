---
description: CodeError schema from Palo Alto Networks Prisma Cloud Code Security API
layout: schema
name: CodeError
properties_list:
- description: Unique error identifier.
  name: errorId
  type: string
- description: Checkov policy ID that triggered the error (e.g., CKV_AWS_18).
  name: policyId
  type: string
- description: Human-readable name of the violated policy.
  name: policyName
  type: string
- description: Error severity level.
  name: severity
  type: string
- description: Error category based on the type of scan that detected it.
  name: category
  type: string
- description: Current status of the error.
  name: status
  type: string
- description: Name of the IaC resource where the error was detected.
  name: resourceName
  type: string
- description: Type of the IaC resource.
  name: resourceType
  type: string
- description: Relative path to the file containing the error.
  name: filePath
  type: string
- description: Start and end line numbers of the affected code block.
  name: fileLineRange
  type: array
- description: Repository where the error was found.
  name: repositoryId
  type: string
- description: Branch where the error was detected.
  name: branch
  type: string
- description: URL to documentation explaining the policy and remediation steps.
  name: guideline
  type: string
- description: Timestamp when the error was first detected.
  name: firstDetected
  type: string
- description: Timestamp of the most recent scan where the error was found.
  name: lastDetected
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-code-security-api-code-error-schema.json
slug: prisma-cloud-code-security-api-code-error
source_filename: prisma-cloud-code-security-api-code-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CodeError\",\n  \"description\": \"CodeError schema from Palo Alto Networks Prisma Cloud Code Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-code-error-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique error identifier.\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Checkov policy ID that triggered the error (e.g., CKV_AWS_18).\"\n    },\n    \"policyName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the violated policy.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CRITICAL\",\n        \"HIGH\",\n        \"MEDIUM\",\n        \"LOW\",\n        \"INFO\"\n      ],\n      \"description\"\
  : \"Error severity level.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IAC\",\n        \"SCA\",\n        \"SECRETS\",\n        \"CICD\"\n      ],\n      \"description\": \"Error category based on the type of scan that detected it.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OPEN\",\n        \"SUPPRESSED\",\n        \"FIXED\"\n      ],\n      \"description\": \"Current status of the error.\"\n    },\n    \"resourceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the IaC resource where the error was detected.\"\n    },\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the IaC resource.\"\n    },\n    \"filePath\": {\n      \"type\": \"string\",\n      \"description\": \"Relative path to the file containing the error.\"\n    },\n    \"fileLineRange\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n\
  \      \"minItems\": 2,\n      \"maxItems\": 2,\n      \"description\": \"Start and end line numbers of the affected code block.\"\n    },\n    \"repositoryId\": {\n      \"type\": \"string\",\n      \"description\": \"Repository where the error was found.\"\n    },\n    \"branch\": {\n      \"type\": \"string\",\n      \"description\": \"Branch where the error was detected.\"\n    },\n    \"guideline\": {\n      \"type\": \"string\",\n      \"description\": \"URL to documentation explaining the policy and remediation steps.\"\n    },\n    \"firstDetected\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the error was first detected.\"\n    },\n    \"lastDetected\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent scan where the error was found.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-code-error-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CodeError
---
