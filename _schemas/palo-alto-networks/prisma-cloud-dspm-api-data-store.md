---
description: DataStore schema from Palo Alto Networks Prisma Cloud DSPM API
layout: schema
name: DataStore
properties_list:
- description: Unique data store identifier in Prisma Cloud.
  name: id
  type: string
- description: Name of the data store as it appears in the cloud provider.
  name: name
  type: string
- description: Cloud provider where the data store is hosted.
  name: cloudProvider
  type: string
- description: Cloud account ID that owns the data store.
  name: cloudAccountId
  type: string
- description: Cloud region where the data store is located.
  name: region
  type: string
- description: Category of the data store service.
  name: serviceType
  type: string
- description: Specific cloud service name (e.g., Amazon S3, Amazon RDS).
  name: serviceName
  type: string
- description: Whether encryption at rest is enabled.
  name: encryptionEnabled
  type: boolean
- description: Whether the data store is accessible from the public internet.
  name: isPubliclyAccessible
  type: boolean
- description: Overall risk level computed from data sensitivity and security posture.
  name: riskLevel
  type: string
- description: Number of sensitive data assets found in this data store.
  name: sensitiveDataCount
  type: integer
- description: Distinct classification labels found in the data store.
  name: classificationLabels
  type: array
- description: Total number of data assets discovered in this data store.
  name: dataAssetCount
  type: integer
- description: Timestamp when the data store was first discovered by DSPM.
  name: discoveredAt
  type: string
- description: Timestamp of the most recent data classification scan.
  name: lastScannedAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-dspm-api-data-store-schema.json
slug: prisma-cloud-dspm-api-data-store
source_filename: prisma-cloud-dspm-api-data-store-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataStore\",\n  \"description\": \"DataStore schema from Palo Alto Networks Prisma Cloud DSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-data-store-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique data store identifier in Prisma Cloud.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the data store as it appears in the cloud provider.\"\n    },\n    \"cloudProvider\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"aws\",\n        \"azure\",\n        \"gcp\"\n      ],\n      \"description\": \"Cloud provider where the data store is hosted.\"\n    },\n    \"cloudAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud account ID that owns\
  \ the data store.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region where the data store is located.\"\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"relationalDatabase\",\n        \"noSqlDatabase\",\n        \"objectStorage\",\n        \"fileShare\",\n        \"dataWarehouse\",\n        \"dataLake\",\n        \"cache\",\n        \"messageQueue\"\n      ],\n      \"description\": \"Category of the data store service.\"\n    },\n    \"serviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Specific cloud service name (e.g., Amazon S3, Amazon RDS).\"\n    },\n    \"encryptionEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether encryption at rest is enabled.\"\n    },\n    \"isPubliclyAccessible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the data store is accessible from the public internet.\"\n    },\n    \"riskLevel\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\"\n      ],\n      \"description\": \"Overall risk level computed from data sensitivity and security posture.\"\n    },\n    \"sensitiveDataCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of sensitive data assets found in this data store.\"\n    },\n    \"classificationLabels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Distinct classification labels found in the data store.\"\n    },\n    \"dataAssetCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of data assets discovered in this data store.\"\n    },\n    \"discoveredAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the data store was first discovered by DSPM.\"\n    },\n    \"lastScannedAt\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent data classification scan.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-data-store-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DataStore
---
