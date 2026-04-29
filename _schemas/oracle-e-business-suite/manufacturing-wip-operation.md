---
description: ''
layout: schema
name: WipOperation
properties_list:
- description: WIP entity identifier
  name: wipEntityId
  type: integer
- description: Operation sequence number
  name: operationSeqNum
  type: integer
- description: Organization identifier
  name: organizationId
  type: integer
- description: Department identifier
  name: departmentId
  type: integer
- description: ''
  name: departmentCode
  type: string
- description: Operation description
  name: operationDescription
  type: string
- description: ''
  name: scheduledQuantity
  type: number
- description: Quantity in queue
  name: quantityInQueue
  type: number
- description: Quantity running
  name: quantityRunning
  type: number
- description: Quantity completed
  name: quantityCompleted
  type: number
- description: Quantity scrapped
  name: quantityScrapped
  type: number
- description: ''
  name: firstUnitStartDate
  type: string
- description: ''
  name: lastUnitCompletionDate
  type: string
- description: ''
  name: countPointType
  type: integer
- description: ''
  name: backflushFlag
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-wip-operation-schema.json
slug: manufacturing-wip-operation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WipOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"wipEntityId\": {\n      \"type\": \"integer\",\n      \"description\": \"WIP entity identifier\"\n    },\n    \"operationSeqNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Operation sequence number\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"departmentId\": {\n      \"type\": \"integer\",\n      \"description\": \"Department identifier\"\n    },\n    \"departmentCode\": {\n      \"type\": \"string\"\n    },\n    \"operationDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Operation description\"\n    },\n    \"scheduledQuantity\": {\n      \"type\": \"number\"\n    },\n    \"quantityInQueue\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity in queue\"\n    },\n    \"quantityRunning\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Quantity running\"\n    },\n    \"quantityCompleted\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity completed\"\n    },\n    \"quantityScrapped\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity scrapped\"\n    },\n    \"firstUnitStartDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUnitCompletionDate\": {\n      \"type\": \"string\"\n    },\n    \"countPointType\": {\n      \"type\": \"integer\"\n    },\n    \"backflushFlag\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-wip-operation-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: WipOperation
---
