---
description: ''
layout: schema
name: Location
properties_list:
- description: The Workday ID of the location.
  name: id
  type: string
- description: A display descriptor for the location.
  name: descriptor
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: latitude
  type: number
- description: ''
  name: longitude
  type: number
- description: ''
  name: usages
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/hcm-location-schema.json
slug: hcm-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Location\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the location.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the location.\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"latitude\": {\n      \"type\": \"number\"\n    },\n    \"longitude\": {\n      \"type\": \"number\"\n    },\n    \"usages\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/hcm-location-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Location
---
