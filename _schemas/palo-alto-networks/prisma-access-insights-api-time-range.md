---
description: Time range specification for the query
layout: schema
name: TimeRange
properties_list:
- description: Type of time range (absolute or relative)
  name: type
  type: string
- description: Time range value (required for ABSOLUTE type)
  name: value
  type: object
- description: Relative time range (required for RELATIVE type)
  name: last
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-insights-api-time-range-schema.json
slug: prisma-access-insights-api-time-range
source_filename: prisma-access-insights-api-time-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeRange\",\n  \"description\": \"Time range specification for the query\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-time-range-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of time range (absolute or relative)\",\n      \"enum\": [\n        \"ABSOLUTE\",\n        \"RELATIVE\"\n      ]\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\": \"Time range value (required for ABSOLUTE type)\",\n      \"properties\": {\n        \"from\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Start of the time range (ISO 8601)\"\n        },\n        \"to\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"\
  description\": \"End of the time range (ISO 8601)\"\n        }\n      }\n    },\n    \"last\": {\n      \"type\": \"object\",\n      \"description\": \"Relative time range (required for RELATIVE type)\",\n      \"properties\": {\n        \"units\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"HOURS\",\n            \"DAYS\",\n            \"WEEKS\"\n          ],\n          \"description\": \"Unit of time for relative range\"\n        },\n        \"value\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of units for relative range\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-time-range-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TimeRange
---
