---
description: BatchModel schema from Avalara API
layout: schema
name: BatchModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: companyId
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: recordCount
  type: integer
- description: ''
  name: currentRecord
  type: integer
- description: ''
  name: createdDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-batch-model-schema.json
slug: avatax-rest-batch-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-batch-model-schema.json\",\n  \"title\": \"BatchModel\",\n  \"description\": \"BatchModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AvaCertUpdate\",\n        \"AvaCertUpdateAll\",\n        \"BatchMaintenance\",\n        \"CompanyLocationImport\",\n        \"DocumentImport\",\n        \"ExemptCertImport\",\n        \"ItemImport\",\n        \"SalesAuditExport\",\n        \"SstpTestDeckImport\",\n        \"TaxRuleImport\",\n        \"TransactionImport\",\n        \"UPCBulkImport\",\n        \"UPCBulkDelete\"\n      ]\n    },\n    \"status\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Waiting\",\n        \"SystemErrors\",\n        \"Cancelled\",\n        \"Completed\",\n        \"Creating\",\n        \"Deleted\",\n        \"Errors\",\n        \"Paused\",\n        \"Processing\",\n        \"ReadyToDelete\"\n      ]\n    },\n    \"recordCount\": {\n      \"type\": \"integer\"\n    },\n    \"currentRecord\": {\n      \"type\": \"integer\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-batch-model-schema.json
tags:
- Taxes
title: BatchModel
---
