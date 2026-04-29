---
description: Placeholder documentation for CdiInputSpecification
layout: schema
name: CdiInputSpecification
properties_list:
- description: ''
  name: Resolution
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-cdi-input-specification-schema.json
slug: medialive-api-cdi-input-specification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-cdi-input-specification-schema.json\",\n  \"title\": \"CdiInputSpecification\",\n  \"description\": \"Placeholder documentation for CdiInputSpecification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Resolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CdiInputResolution\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resolution\"\n          },\n          \"description\": \"Maximum CDI input resolution\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-cdi-input-specification-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CdiInputSpecification
---
