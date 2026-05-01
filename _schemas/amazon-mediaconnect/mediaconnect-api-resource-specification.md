---
description: A definition of what is being billed for, including the type and amount.
layout: schema
name: ResourceSpecification
properties_list:
- description: ''
  name: ReservedBitrate
  type: object
- description: ''
  name: ResourceType
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-resource-specification-schema.json
slug: mediaconnect-api-resource-specification
source_filename: mediaconnect-api-resource-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-resource-specification-schema.json\",\n  \"title\": \"ResourceSpecification\",\n  \"description\": \"A definition of what is being billed for, including the type and amount.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservedBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservedBitrate\"\n          },\n          \"description\": \"The amount of outbound bandwidth that is discounted in the offering.\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceType\"\n          },\n       \
  \   \"description\": \"The type of resource and the unit that is being billed for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-resource-specification-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: ResourceSpecification
---
