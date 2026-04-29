---
description: ''
layout: schema
name: DiscreteJobCreate
properties_list:
- description: ''
  name: wipEntityName
  type: string
- description: ''
  name: primaryItemId
  type: integer
- description: ''
  name: organizationId
  type: integer
- description: ''
  name: statusType
  type: integer
- description: ''
  name: jobType
  type: integer
- description: ''
  name: startQuantity
  type: number
- description: ''
  name: scheduledStartDate
  type: string
- description: ''
  name: scheduledCompletionDate
  type: string
- description: ''
  name: classCode
  type: string
- description: ''
  name: bomRevision
  type: string
- description: ''
  name: routingRevision
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: firmPlannedFlag
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-discrete-job-create-schema.json
slug: manufacturing-discrete-job-create
source_filename: manufacturing-discrete-job-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DiscreteJobCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"wipEntityName\": {\n      \"type\": \"string\"\n    },\n    \"primaryItemId\": {\n      \"type\": \"integer\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\"\n    },\n    \"statusType\": {\n      \"type\": \"integer\"\n    },\n    \"jobType\": {\n      \"type\": \"integer\"\n    },\n    \"startQuantity\": {\n      \"type\": \"number\"\n    },\n    \"scheduledStartDate\": {\n      \"type\": \"string\"\n    },\n    \"scheduledCompletionDate\": {\n      \"type\": \"string\"\n    },\n    \"classCode\": {\n      \"type\": \"string\"\n    },\n    \"bomRevision\": {\n      \"type\": \"string\"\n    },\n    \"routingRevision\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"firmPlannedFlag\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-discrete-job-create-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: DiscreteJobCreate
---
