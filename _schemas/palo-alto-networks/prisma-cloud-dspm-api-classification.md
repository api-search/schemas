---
description: Classification schema from Palo Alto Networks Prisma Cloud DSPM API
layout: schema
name: Classification
properties_list:
- description: Unique classification identifier.
  name: id
  type: string
- description: Classification label name.
  name: name
  type: string
- description: Detailed description of what the classification detects.
  name: description
  type: string
- description: Broad category of the classification.
  name: category
  type: string
- description: Default sensitivity level for data matching this classification.
  name: sensitivityLevel
  type: string
- description: Whether this is a built-in or custom classification.
  name: isBuiltIn
  type: boolean
- description: Regulatory frameworks referencing this data classification.
  name: regulatoryFrameworks
  type: array
- description: Number of data stores where matching data has been found.
  name: dataStoreCount
  type: integer
- description: Number of data assets matching this classification.
  name: dataAssetCount
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-dspm-api-classification-schema.json
slug: prisma-cloud-dspm-api-classification
source_filename: prisma-cloud-dspm-api-classification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Classification\",\n  \"description\": \"Classification schema from Palo Alto Networks Prisma Cloud DSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-classification-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique classification identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Classification label name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of what the classification detects.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PII\",\n        \"PHI\",\n        \"PCI\",\n        \"Financial\",\n        \"Credentials\",\n        \"Intellectual Property\",\n     \
  \   \"Custom\"\n      ],\n      \"description\": \"Broad category of the classification.\"\n    },\n    \"sensitivityLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"public\",\n        \"internal\",\n        \"confidential\",\n        \"restricted\"\n      ],\n      \"description\": \"Default sensitivity level for data matching this classification.\"\n    },\n    \"isBuiltIn\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a built-in or custom classification.\"\n    },\n    \"regulatoryFrameworks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"GDPR\",\n          \"CCPA\",\n          \"HIPAA\",\n          \"PCI-DSS\",\n          \"SOX\",\n          \"GLBA\",\n          \"FERPA\"\n        ]\n      },\n      \"description\": \"Regulatory frameworks referencing this data classification.\"\n    },\n    \"dataStoreCount\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Number of data stores where matching data has been found.\"\n    },\n    \"dataAssetCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of data assets matching this classification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-classification-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Classification
---
