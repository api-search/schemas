---
description: An in-out parameter defined within a mapping.
layout: schema
name: MappingInOutParameter
properties_list:
- description: The parameter ID.
  name: id
  type: integer
- description: The parameter name.
  name: name
  type: string
- description: A description of the parameter.
  name: description
  type: string
- description: The starting value for the parameter.
  name: initialValue
  type: string
- description: The data type of the parameter.
  name: datatype
  type: string
- description: The numeric precision.
  name: precision
  type: string
- description: The decimal scale.
  name: scale
  type: string
- description: The value retention policy.
  name: retentionPolicy
  type: string
- description: The method for determining the final value.
  name: aggregationType
  type: string
- description: The current parameter value.
  name: currentValue
  type: string
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-mapping-in-out-parameter-schema.json
slug: informatica-platform-rest-mapping-in-out-parameter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingInOutParameter\",\n  \"type\": \"object\",\n  \"description\": \"An in-out parameter defined within a mapping.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The parameter ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The parameter name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the parameter.\"\n    },\n    \"initialValue\": {\n      \"type\": \"string\",\n      \"description\": \"The starting value for the parameter.\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the parameter.\"\n    },\n    \"precision\": {\n      \"type\": \"string\",\n      \"description\": \"The numeric precision.\"\n    },\n    \"scale\": {\n      \"type\": \"string\",\n      \"description\": \"The decimal\
  \ scale.\"\n    },\n    \"retentionPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"The value retention policy.\"\n    },\n    \"aggregationType\": {\n      \"type\": \"string\",\n      \"description\": \"The method for determining the final value.\"\n    },\n    \"currentValue\": {\n      \"type\": \"string\",\n      \"description\": \"The current parameter value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-mapping-in-out-parameter-schema.json
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
title: MappingInOutParameter
---
