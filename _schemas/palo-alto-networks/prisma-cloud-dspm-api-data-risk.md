---
description: DataRisk schema from Palo Alto Networks Prisma Cloud DSPM API
layout: schema
name: DataRisk
properties_list:
- description: Unique risk identifier.
  name: id
  type: string
- description: Short description of the risk.
  name: title
  type: string
- description: Detailed explanation of the risk and its potential impact.
  name: description
  type: string
- description: Severity of the risk.
  name: riskLevel
  type: string
- description: Category of the data security risk.
  name: riskCategory
  type: string
- description: Current status of the risk.
  name: status
  type: string
- description: Data store where the risk was identified.
  name: dataStoreId
  type: string
- description: Name of the affected data store.
  name: dataStoreName
  type: string
- description: Cloud provider of the affected data store.
  name: cloudProvider
  type: string
- description: Cloud account ID of the affected data store.
  name: cloudAccountId
  type: string
- description: Cloud region of the affected data store.
  name: region
  type: string
- description: Classification labels of sensitive data at risk.
  name: affectedClassifications
  type: array
- description: Number of data assets affected by this risk.
  name: affectedDataAssetCount
  type: integer
- description: Recommended remediation steps.
  name: remediation
  type: object
- description: Timestamp when the risk was first detected.
  name: detectedAt
  type: string
- description: Timestamp of the most recent risk evaluation.
  name: lastEvaluatedAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-dspm-api-data-risk-schema.json
slug: prisma-cloud-dspm-api-data-risk
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataRisk\",\n  \"description\": \"DataRisk schema from Palo Alto Networks Prisma Cloud DSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-data-risk-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique risk identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the risk.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed explanation of the risk and its potential impact.\"\n    },\n    \"riskLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\"\n      ],\n      \"description\": \"Severity of the risk.\"\n    },\n    \"riskCategory\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"publicExposure\",\n        \"encryptionMissing\",\n        \"excessivePermissions\",\n        \"dataResidency\",\n        \"auditLogging\",\n        \"backupMissing\",\n        \"crossAccountAccess\",\n        \"sensitiveDataExposure\"\n      ],\n      \"description\": \"Category of the data security risk.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"open\",\n        \"remediated\",\n        \"suppressed\",\n        \"acknowledged\"\n      ],\n      \"description\": \"Current status of the risk.\"\n    },\n    \"dataStoreId\": {\n      \"type\": \"string\",\n      \"description\": \"Data store where the risk was identified.\"\n    },\n    \"dataStoreName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the affected data store.\"\n    },\n    \"cloudProvider\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"aws\",\n        \"azure\",\n        \"gcp\"\
  \n      ],\n      \"description\": \"Cloud provider of the affected data store.\"\n    },\n    \"cloudAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud account ID of the affected data store.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region of the affected data store.\"\n    },\n    \"affectedClassifications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Classification labels of sensitive data at risk.\"\n    },\n    \"affectedDataAssetCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of data assets affected by this risk.\"\n    },\n    \"remediation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the recommended remediation.\"\n        },\n        \"steps\": {\n          \"type\": \"array\"\
  ,\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Step-by-step remediation instructions.\"\n        },\n        \"automatedRemediationAvailable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether automated remediation is available.\"\n        }\n      },\n      \"description\": \"Recommended remediation steps.\"\n    },\n    \"detectedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the risk was first detected.\"\n    },\n    \"lastEvaluatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent risk evaluation.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-data-risk-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DataRisk
---
