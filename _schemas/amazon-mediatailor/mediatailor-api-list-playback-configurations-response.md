---
description: ListPlaybackConfigurationsResponse schema from Amazon MediaTailor API
layout: schema
name: ListPlaybackConfigurationsResponse
properties_list:
- description: ''
  name: Items
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-list-playback-configurations-response-schema.json
slug: mediatailor-api-list-playback-configurations-response
source_filename: mediatailor-api-list-playback-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-list-playback-configurations-response-schema.json\",\n  \"title\": \"ListPlaybackConfigurationsResponse\",\n  \"description\": \"ListPlaybackConfigurationsResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfPlaybackConfiguration\"\n        },\n        {\n          \"description\": \"Array of playback configurations. This might be all the available configurations or a subset, depending on the settings that you provide and the total number of configurations stored.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\"\
  : \"Pagination token returned by the GET list request when results exceed the maximum allowed. Use the token to fetch the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-list-playback-configurations-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListPlaybackConfigurationsResponse
---
