---
description: A reference to a Workday resource.
layout: schema
name: ResourceReference
properties_list:
- description: The Workday ID of the referenced resource.
  name: id
  type: string
- description: A display descriptor for the referenced resource.
  name: descriptor
  type: string
- description: A link to the referenced resource.
  name: href
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/hcm-resource-reference-schema.json
slug: hcm-resource-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceReference\",\n  \"type\": \"object\",\n  \"description\": \"A reference to a Workday resource.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the referenced resource.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the referenced resource.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"A link to the referenced resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/hcm-resource-reference-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: ResourceReference
---
