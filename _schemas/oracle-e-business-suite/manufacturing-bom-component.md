---
description: ''
layout: schema
name: BomComponent
properties_list:
- description: Component sequence identifier
  name: componentSequenceId
  type: integer
- description: Component item identifier
  name: componentItemId
  type: integer
- description: Component item number
  name: componentItemNumber
  type: string
- description: Component item description
  name: itemDescription
  type: string
- description: Operation sequence number where component is consumed
  name: operationSeqNum
  type: integer
- description: Component quantity per assembly
  name: componentQuantity
  type: number
- description: Component yield factor
  name: componentYieldFactor
  type: number
- description: Effective date
  name: effectivityDate
  type: string
- description: Disable date
  name: disableDate
  type: string
- description: WIP supply type (1=Push, 2=Assembly Pull, 3=Operation Pull, 4=Bulk, 5=Supplier, 6=Phantom)
  name: wipSupplyType
  type: integer
- description: Optional flag (1=Yes, 2=No)
  name: optional
  type: integer
- description: Quantity related flag
  name: quantityRelated
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-bom-component-schema.json
slug: manufacturing-bom-component
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BomComponent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentSequenceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Component sequence identifier\"\n    },\n    \"componentItemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Component item identifier\"\n    },\n    \"componentItemNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Component item number\"\n    },\n    \"itemDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Component item description\"\n    },\n    \"operationSeqNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Operation sequence number where component is consumed\"\n    },\n    \"componentQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"Component quantity per assembly\"\n    },\n    \"componentYieldFactor\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Component yield factor\"\n    },\n    \"effectivityDate\": {\n      \"type\": \"string\",\n      \"description\": \"Effective date\"\n    },\n    \"disableDate\": {\n      \"type\": \"string\",\n      \"description\": \"Disable date\"\n    },\n    \"wipSupplyType\": {\n      \"type\": \"integer\",\n      \"description\": \"WIP supply type (1=Push, 2=Assembly Pull, 3=Operation Pull, 4=Bulk, 5=Supplier, 6=Phantom)\"\n    },\n    \"optional\": {\n      \"type\": \"integer\",\n      \"description\": \"Optional flag (1=Yes, 2=No)\"\n    },\n    \"quantityRelated\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity related flag\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-bom-component-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: BomComponent
---
