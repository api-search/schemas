---
description: An AWS Supply Chain instance
layout: schema
name: Instance
properties_list:
- description: The unique identifier of the instance
  name: instanceId
  type: string
- description: The name of the instance
  name: instanceName
  type: string
- description: The description of the instance
  name: instanceDescription
  type: string
- description: The state of the instance
  name: instanceState
  type: string
- description: The KMS key ARN used to encrypt instance data
  name: kmsKeyArn
  type: string
- description: The DNS domain for the web application
  name: webAppDnsDomain
  type: string
- description: The creation timestamp
  name: createdTime
  type: string
- description: The last modification timestamp
  name: lastModifiedTime
  type: string
provider_name: Amazon Supply Chain
provider_slug: amazon-supply-chain
schema_file: json-schema/amazon-supply-chain-instance-schema.json
slug: amazon-supply-chain-instance
source_filename: amazon-supply-chain-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-instance-schema.json\",\n  \"title\": \"Instance\",\n  \"description\": \"An AWS Supply Chain instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the instance\",\n      \"example\": \"inst-abc12345\"\n    },\n    \"instanceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the instance\",\n      \"example\": \"MySupplyChainInstance\"\n    },\n    \"instanceDescription\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the instance\",\n      \"example\": \"Production supply chain instance\"\n    },\n    \"instanceState\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Initializing\",\n        \"Active\",\n\
  \        \"CreateFailed\",\n        \"DeleteFailed\",\n        \"Deleting\",\n        \"Deleted\"\n      ],\n      \"description\": \"The state of the instance\",\n      \"example\": \"Active\"\n    },\n    \"kmsKeyArn\": {\n      \"type\": \"string\",\n      \"description\": \"The KMS key ARN used to encrypt instance data\",\n      \"example\": \"arn:aws:kms:us-east-1:123456789012:key/abc12345\"\n    },\n    \"webAppDnsDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS domain for the web application\",\n      \"example\": \"instance.scn.amazonaws.com\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation timestamp\",\n      \"example\": \"2025-01-15T10:30:00Z\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last modification timestamp\",\n      \"example\": \"2025-03-01T08:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-instance-schema.json
tags:
- ERP Integration
- Logistics
- Machine Learning
- Supply Chain
title: Instance
---
