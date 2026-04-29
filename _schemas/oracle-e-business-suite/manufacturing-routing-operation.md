---
description: ''
layout: schema
name: RoutingOperation
properties_list:
- description: Operation sequence identifier
  name: operationSequenceId
  type: integer
- description: Operation sequence number
  name: operationSeqNum
  type: integer
- description: Operation description
  name: operationDescription
  type: string
- description: Standard operation code
  name: operationCode
  type: string
- description: Department identifier
  name: departmentId
  type: integer
- description: Department code
  name: departmentCode
  type: string
- description: ''
  name: effectivityDate
  type: string
- description: ''
  name: disableDate
  type: string
- description: ''
  name: minimumTransferQuantity
  type: number
- description: Count point type (1=Yes, 2=No, 3=Auto-charge)
  name: countPointType
  type: integer
- description: ''
  name: resources
  type: array
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-routing-operation-schema.json
slug: manufacturing-routing-operation
source_filename: manufacturing-routing-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RoutingOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operationSequenceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Operation sequence identifier\"\n    },\n    \"operationSeqNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Operation sequence number\"\n    },\n    \"operationDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Operation description\"\n    },\n    \"operationCode\": {\n      \"type\": \"string\",\n      \"description\": \"Standard operation code\"\n    },\n    \"departmentId\": {\n      \"type\": \"integer\",\n      \"description\": \"Department identifier\"\n    },\n    \"departmentCode\": {\n      \"type\": \"string\",\n      \"description\": \"Department code\"\n    },\n    \"effectivityDate\": {\n      \"type\": \"string\"\n    },\n    \"disableDate\": {\n      \"type\": \"string\"\n    },\n    \"minimumTransferQuantity\"\
  : {\n      \"type\": \"number\"\n    },\n    \"countPointType\": {\n      \"type\": \"integer\",\n      \"description\": \"Count point type (1=Yes, 2=No, 3=Auto-charge)\"\n    },\n    \"resources\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-routing-operation-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: RoutingOperation
---
