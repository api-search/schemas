---
description: A bill of materials import job
layout: schema
name: BillOfMaterialsImportJob
properties_list:
- description: The instance identifier
  name: instanceId
  type: string
- description: The job identifier
  name: jobId
  type: string
- description: The job status
  name: status
  type: string
- description: The S3 URI of the import file
  name: s3uri
  type: string
- description: Status message
  name: message
  type: string
provider_name: Amazon Supply Chain
provider_slug: amazon-supply-chain
schema_file: json-schema/amazon-supply-chain-bill-of-materials-import-job-schema.json
slug: amazon-supply-chain-bill-of-materials-import-job
source_filename: amazon-supply-chain-bill-of-materials-import-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-bill-of-materials-import-job-schema.json\",\n  \"title\": \"BillOfMaterialsImportJob\",\n  \"description\": \"A bill of materials import job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The instance identifier\",\n      \"example\": \"inst-abc12345\"\n    },\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"The job identifier\",\n      \"example\": \"job-abc12345\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"New\",\n        \"Failed\",\n        \"InProgress\",\n        \"Queued\",\n        \"Success\"\n      ],\n      \"description\": \"The job status\",\n      \"example\": \"Success\"\n    },\n    \"s3uri\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The S3 URI of the import file\",\n      \"example\": \"s3://my-bucket/bom-data.csv\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Status message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-bill-of-materials-import-job-schema.json
tags:
- AWS
- ERP Integration
- Logistics
- Machine Learning
- Supply Chain
title: BillOfMaterialsImportJob
---
