---
description: CreateOutpostInput schema from Amazon Outposts
layout: schema
name: CreateOutpostInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: SiteId
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: AvailabilityZoneId
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: SupportedHardwareType
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-create-outpost-input-schema.json
slug: openapi-create-outpost-input
source_filename: openapi-create-outpost-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-create-outpost-input-schema.json\",\n  \"title\": \"CreateOutpostInput\",\n  \"description\": \"CreateOutpostInput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"$ref\": \"#/components/schemas/OutpostName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/OutpostDescription\"\n    },\n    \"SiteId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SiteId\"\n        },\n        {\n          \"description\": \" The ID or the Amazon Resource Name (ARN) of the site. \"\n        }\n      ]\n    },\n    \"AvailabilityZone\": {\n      \"$ref\": \"#/components/schemas/AvailabilityZone\"\n    },\n    \"AvailabilityZoneId\": {\n      \"$ref\": \"#/components/schemas/AvailabilityZoneId\"\n    },\n \
  \   \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags to apply to the Outpost.\"\n        }\n      ]\n    },\n    \"SupportedHardwareType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SupportedHardwareType\"\n        },\n        {\n          \"description\": \" The type of hardware for this Outpost. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"SiteId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-create-outpost-input-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: CreateOutpostInput
---
