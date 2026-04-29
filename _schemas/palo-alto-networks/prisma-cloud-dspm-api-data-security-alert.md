---
description: DataSecurityAlert schema from Palo Alto Networks Prisma Cloud DSPM API
layout: schema
name: DataSecurityAlert
properties_list:
- description: Unique alert identifier.
  name: id
  type: string
- description: Short description of the alert condition.
  name: title
  type: string
- description: Detailed alert description.
  name: description
  type: string
- description: Alert severity level.
  name: severity
  type: string
- description: Current alert status.
  name: status
  type: string
- description: Category of data security alert.
  name: alertType
  type: string
- description: Affected data store identifier.
  name: dataStoreId
  type: string
- description: Name of the affected data store.
  name: dataStoreName
  type: string
- description: Cloud provider of the affected data store.
  name: cloudProvider
  type: string
- description: Cloud account identifier.
  name: cloudAccountId
  type: string
- description: Cloud region of the affected data store.
  name: region
  type: string
- description: Data classification labels involved in the alert.
  name: affectedClassifications
  type: array
- description: Timestamp when the alert was generated.
  name: detectedAt
  type: string
- description: Timestamp when the alert was resolved. Null if still open.
  name: resolvedAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-dspm-api-data-security-alert-schema.json
slug: prisma-cloud-dspm-api-data-security-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSecurityAlert\",\n  \"description\": \"DataSecurityAlert schema from Palo Alto Networks Prisma Cloud DSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-data-security-alert-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique alert identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the alert condition.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed alert description.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\"\n      ],\n      \"description\": \"Alert severity level.\"\n    },\n    \"status\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"open\",\n        \"dismissed\",\n        \"resolved\"\n      ],\n      \"description\": \"Current alert status.\"\n    },\n    \"alertType\": {\n      \"type\": \"string\",\n      \"description\": \"Category of data security alert.\",\n      \"enum\": [\n        \"newPublicDataStore\",\n        \"newSensitiveData\",\n        \"accessAnomaly\",\n        \"policyViolation\",\n        \"dataExfiltration\"\n      ]\n    },\n    \"dataStoreId\": {\n      \"type\": \"string\",\n      \"description\": \"Affected data store identifier.\"\n    },\n    \"dataStoreName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the affected data store.\"\n    },\n    \"cloudProvider\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"aws\",\n        \"azure\",\n        \"gcp\"\n      ],\n      \"description\": \"Cloud provider of the affected data store.\"\n    },\n    \"cloudAccountId\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Cloud account identifier.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region of the affected data store.\"\n    },\n    \"affectedClassifications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Data classification labels involved in the alert.\"\n    },\n    \"detectedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alert was generated.\"\n    },\n    \"resolvedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alert was resolved. Null if still open.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-data-security-alert-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DataSecurityAlert
---
