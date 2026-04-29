---
description: ListPrefetchSchedulesResponse schema from Amazon MediaTailor API
layout: schema
name: ListPrefetchSchedulesResponse
properties_list:
- description: ''
  name: Items
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-list-prefetch-schedules-response-schema.json
slug: mediatailor-api-list-prefetch-schedules-response
source_filename: mediatailor-api-list-prefetch-schedules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-list-prefetch-schedules-response-schema.json\",\n  \"title\": \"ListPrefetchSchedulesResponse\",\n  \"description\": \"ListPrefetchSchedulesResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfPrefetchSchedule\"\n        },\n        {\n          \"description\": \"Lists the prefetch schedules. An empty <code>Items</code> list doesn't mean there aren't more items to fetch, just that that page was empty.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Pagination token returned by the list request when results\
  \ exceed the maximum allowed. Use the token to fetch the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-list-prefetch-schedules-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListPrefetchSchedulesResponse
---
