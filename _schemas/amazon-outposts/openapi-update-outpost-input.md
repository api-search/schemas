---
description: UpdateOutpostInput schema from Amazon Outposts
layout: schema
name: UpdateOutpostInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: SupportedHardwareType
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-update-outpost-input-schema.json
slug: openapi-update-outpost-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-update-outpost-input-schema.json\",\n  \"title\": \"UpdateOutpostInput\",\n  \"description\": \"UpdateOutpostInput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"$ref\": \"#/components/schemas/OutpostName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/OutpostDescription\"\n    },\n    \"SupportedHardwareType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SupportedHardwareType\"\n        },\n        {\n          \"description\": \" The type of hardware for this Outpost. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-update-outpost-input-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: UpdateOutpostInput
---
