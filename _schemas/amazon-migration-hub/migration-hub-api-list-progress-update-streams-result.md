---
description: ListProgressUpdateStreamsResult schema from Amazon Migration Hub API
layout: schema
name: ListProgressUpdateStreamsResult
properties_list:
- description: ''
  name: ProgressUpdateStreamSummaryList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-list-progress-update-streams-result-schema.json
slug: migration-hub-api-list-progress-update-streams-result
source_filename: migration-hub-api-list-progress-update-streams-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-progress-update-streams-result-schema.json\",\n  \"title\": \"ListProgressUpdateStreamsResult\",\n  \"description\": \"ListProgressUpdateStreamsResult schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStreamSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStreamSummaryList\"\n        },\n        {\n          \"description\": \"List of progress update streams up to the max number of results passed in the input.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"If there are more streams created than the max result, return the next\
  \ token to be passed to the next call as a bookmark of where to start from.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-progress-update-streams-result-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListProgressUpdateStreamsResult
---
