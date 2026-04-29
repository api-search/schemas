---
description: ''
layout: schema
name: BillOfMaterial
properties_list:
- description: Bill sequence identifier
  name: billSequenceId
  type: integer
- description: Assembly item identifier
  name: assemblyItemId
  type: integer
- description: Assembly item number
  name: assemblyItemNumber
  type: string
- description: Organization identifier
  name: organizationId
  type: integer
- description: Alternate BOM designator
  name: alternateDesignator
  type: string
- description: Assembly type (1=Manufacturing, 2=Engineering)
  name: assemblyType
  type: integer
- description: Common bill sequence identifier
  name: commonBillSequenceId
  type: integer
- description: Assembly comment
  name: specificAssemblyComment
  type: string
- description: ''
  name: components
  type: array
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-bill-of-material-schema.json
slug: manufacturing-bill-of-material
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BillOfMaterial\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billSequenceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Bill sequence identifier\"\n    },\n    \"assemblyItemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Assembly item identifier\"\n    },\n    \"assemblyItemNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Assembly item number\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"alternateDesignator\": {\n      \"type\": \"string\",\n      \"description\": \"Alternate BOM designator\"\n    },\n    \"assemblyType\": {\n      \"type\": \"integer\",\n      \"description\": \"Assembly type (1=Manufacturing, 2=Engineering)\"\n    },\n    \"commonBillSequenceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Common bill sequence\
  \ identifier\"\n    },\n    \"specificAssemblyComment\": {\n      \"type\": \"string\",\n      \"description\": \"Assembly comment\"\n    },\n    \"components\": {\n      \"type\": \"array\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-bill-of-material-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: BillOfMaterial
---
