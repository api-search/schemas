---
description: The HTTP configuration for the source location.
layout: schema
name: HttpConfiguration
properties_list:
- description: ''
  name: BaseUrl
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-http-configuration-schema.json
slug: mediatailor-api-http-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-http-configuration-schema.json\",\n  \"title\": \"HttpConfiguration\",\n  \"description\": \"The HTTP configuration for the source location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BaseUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The base URL for the source location host server. This string must include the protocol, such as <b>https://</b>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BaseUrl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-http-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HttpConfiguration
---
