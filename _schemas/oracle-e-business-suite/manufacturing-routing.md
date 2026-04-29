---
description: ''
layout: schema
name: Routing
properties_list:
- description: Routing sequence identifier
  name: routingSequenceId
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
- description: Alternate routing designator
  name: alternateDesignator
  type: string
- description: Routing type (1=Manufacturing, 2=Engineering)
  name: routingType
  type: integer
- description: ''
  name: operations
  type: array
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-routing-schema.json
slug: manufacturing-routing
source_filename: manufacturing-routing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Routing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"routingSequenceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Routing sequence identifier\"\n    },\n    \"assemblyItemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Assembly item identifier\"\n    },\n    \"assemblyItemNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Assembly item number\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"alternateDesignator\": {\n      \"type\": \"string\",\n      \"description\": \"Alternate routing designator\"\n    },\n    \"routingType\": {\n      \"type\": \"integer\",\n      \"description\": \"Routing type (1=Manufacturing, 2=Engineering)\"\n    },\n    \"operations\": {\n      \"type\": \"array\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\
  \n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-routing-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Routing
---
