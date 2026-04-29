---
description: DataAsset schema from Palo Alto Networks Prisma Cloud DSPM API
layout: schema
name: DataAsset
properties_list:
- description: Unique data asset identifier.
  name: id
  type: string
- description: Parent data store identifier.
  name: dataStoreId
  type: string
- description: Name of the parent data store.
  name: dataStoreName
  type: string
- description: Name of the data asset (e.g., table name, column name, object prefix, directory name).
  name: name
  type: string
- description: Type of data asset.
  name: assetType
  type: string
- description: Full path to the data asset within the data store.
  name: path
  type: string
- description: Classification labels applied to this data asset.
  name: classificationLabels
  type: array
- description: Sensitivity level based on the most sensitive classification.
  name: sensitivityLevel
  type: string
- description: Sample data patterns found during classification.
  name: sampleFindings
  type: array
- description: Approximate number of records in this data asset.
  name: recordCount
  type: integer
- description: Timestamp when the data asset was first discovered.
  name: discoveredAt
  type: string
- description: Timestamp of the most recent classification scan.
  name: lastScannedAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-dspm-api-data-asset-schema.json
slug: prisma-cloud-dspm-api-data-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataAsset\",\n  \"description\": \"DataAsset schema from Palo Alto Networks Prisma Cloud DSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-data-asset-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique data asset identifier.\"\n    },\n    \"dataStoreId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent data store identifier.\"\n    },\n    \"dataStoreName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the parent data store.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the data asset (e.g., table name, column name, object prefix, directory name).\"\n    },\n    \"assetType\": {\n      \"type\": \"string\",\n      \"enum\": [\n       \
  \ \"table\",\n        \"column\",\n        \"objectPrefix\",\n        \"directory\",\n        \"file\",\n        \"collection\",\n        \"index\",\n        \"schema\"\n      ],\n      \"description\": \"Type of data asset.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Full path to the data asset within the data store.\"\n    },\n    \"classificationLabels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Classification labels applied to this data asset.\"\n    },\n    \"sensitivityLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"public\",\n        \"internal\",\n        \"confidential\",\n        \"restricted\"\n      ],\n      \"description\": \"Sensitivity level based on the most sensitive classification.\"\n    },\n    \"sampleFindings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"\
  classificationLabel\": {\n            \"type\": \"string\",\n            \"description\": \"Classification label matched.\"\n          },\n          \"pattern\": {\n            \"type\": \"string\",\n            \"description\": \"Pattern description.\"\n          },\n          \"count\": {\n            \"type\": \"integer\",\n            \"description\": \"Approximate number of matching records.\"\n          },\n          \"sampleValue\": {\n            \"type\": \"string\",\n            \"description\": \"Masked sample value showing the pattern match.\"\n          }\n        }\n      },\n      \"description\": \"Sample data patterns found during classification.\"\n    },\n    \"recordCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate number of records in this data asset.\"\n    },\n    \"discoveredAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the data asset was first discovered.\"\n    },\n\
  \    \"lastScannedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent classification scan.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-data-asset-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DataAsset
---
