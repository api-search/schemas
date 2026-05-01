---
description: The log configuration for the channel.
layout: schema
name: LogConfigurationForChannel
properties_list:
- description: ''
  name: LogTypes
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-log-configuration-for-channel-schema.json
slug: mediatailor-api-log-configuration-for-channel
source_filename: mediatailor-api-log-configuration-for-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-log-configuration-for-channel-schema.json\",\n  \"title\": \"LogConfigurationForChannel\",\n  \"description\": \"The log configuration for the channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogTypes\"\n        },\n        {\n          \"description\": \"The log types.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-log-configuration-for-channel-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: LogConfigurationForChannel
---
