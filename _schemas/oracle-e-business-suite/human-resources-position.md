---
description: ''
layout: schema
name: Position
properties_list:
- description: Position identifier
  name: positionId
  type: integer
- description: Position name
  name: name
  type: string
- description: Job identifier
  name: jobId
  type: integer
- description: Organization identifier
  name: organizationId
  type: integer
- description: ''
  name: effectiveStartDate
  type: string
- description: ''
  name: effectiveEndDate
  type: string
- description: Position status
  name: status
  type: string
- description: ''
  name: availabilityStatusId
  type: integer
- description: ''
  name: businessGroupId
  type: integer
- description: ''
  name: locationId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-position-schema.json
slug: human-resources-position
source_filename: human-resources-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Position\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"positionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Position identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Position name\"\n    },\n    \"jobId\": {\n      \"type\": \"integer\",\n      \"description\": \"Job identifier\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"effectiveStartDate\": {\n      \"type\": \"string\"\n    },\n    \"effectiveEndDate\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Position status\"\n    },\n    \"availabilityStatusId\": {\n      \"type\": \"integer\"\n    },\n    \"businessGroupId\": {\n      \"type\": \"integer\"\n    },\n    \"locationId\": {\n      \"type\": \"integer\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-position-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Position
---
