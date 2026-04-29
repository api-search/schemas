---
description: A parameter defined within a mapping.
layout: schema
name: MappingParameter
properties_list:
- description: The parameter identifier.
  name: id
  type: integer
- description: The parameter name.
  name: name
  type: string
- description: The parameter data type.
  name: type
  type: string
- description: A description of the parameter.
  name: description
  type: string
- description: The mapplet ID for mapplet-type parameters.
  name: customFuncId
  type: string
- description: Display configuration including connection type, logical connection, order, visibility, editability, and control type.
  name: uiProperties
  type: string
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-mapping-parameter-schema.json
slug: informatica-platform-rest-mapping-parameter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingParameter\",\n  \"type\": \"object\",\n  \"description\": \"A parameter defined within a mapping.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The parameter identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The parameter name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The parameter data type.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the parameter.\"\n    },\n    \"customFuncId\": {\n      \"type\": \"string\",\n      \"description\": \"The mapplet ID for mapplet-type parameters.\"\n    },\n    \"uiProperties\": {\n      \"type\": \"string\",\n      \"description\": \"Display configuration including connection type, logical connection, order, visibility, editability, and control type.\"\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-mapping-parameter-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: MappingParameter
---
