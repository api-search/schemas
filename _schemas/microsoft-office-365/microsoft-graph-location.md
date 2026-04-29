---
description: Represents location information of an event.
layout: schema
name: Location
properties_list:
- description: The name associated with the location.
  name: displayName
  type: string
- description: The type of location.
  name: locationType
  type: string
- description: Optional URI representing the location.
  name: locationUri
  type: string
- description: For internal use only.
  name: uniqueId
  type: string
- description: For internal use only.
  name: uniqueIdType
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-location-schema.json
slug: microsoft-graph-location
source_filename: microsoft-graph-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Location\",\n  \"type\": \"object\",\n  \"description\": \"Represents location information of an event.\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name associated with the location.\"\n    },\n    \"locationType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of location.\"\n    },\n    \"locationUri\": {\n      \"type\": \"string\",\n      \"description\": \"Optional URI representing the location.\"\n    },\n    \"uniqueId\": {\n      \"type\": \"string\",\n      \"description\": \"For internal use only.\"\n    },\n    \"uniqueIdType\": {\n      \"type\": \"string\",\n      \"description\": \"For internal use only.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-location-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: Location
---
