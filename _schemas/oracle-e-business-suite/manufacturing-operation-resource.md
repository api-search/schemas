---
description: ''
layout: schema
name: OperationResource
properties_list:
- description: Resource sequence number
  name: resourceSeqNum
  type: integer
- description: Resource identifier
  name: resourceId
  type: integer
- description: Resource code
  name: resourceCode
  type: string
- description: Resource usage rate or amount
  name: usageRateOrAmount
  type: number
- description: Basis type (1=Item, 2=Lot, 3=Resource Units, 4=Resource Value)
  name: basisType
  type: integer
- description: Schedule flag
  name: scheduleFlag
  type: integer
- description: Auto-charge type
  name: autochargeType
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-operation-resource-schema.json
slug: manufacturing-operation-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OperationResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceSeqNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Resource sequence number\"\n    },\n    \"resourceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Resource identifier\"\n    },\n    \"resourceCode\": {\n      \"type\": \"string\",\n      \"description\": \"Resource code\"\n    },\n    \"usageRateOrAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Resource usage rate or amount\"\n    },\n    \"basisType\": {\n      \"type\": \"integer\",\n      \"description\": \"Basis type (1=Item, 2=Lot, 3=Resource Units, 4=Resource Value)\"\n    },\n    \"scheduleFlag\": {\n      \"type\": \"integer\",\n      \"description\": \"Schedule flag\"\n    },\n    \"autochargeType\": {\n      \"type\": \"integer\",\n      \"description\": \"Auto-charge type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-operation-resource-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: OperationResource
---
