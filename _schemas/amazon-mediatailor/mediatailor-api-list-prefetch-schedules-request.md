---
description: ListPrefetchSchedulesRequest schema from Amazon MediaTailor API
layout: schema
name: ListPrefetchSchedulesRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: StreamId
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-list-prefetch-schedules-request-schema.json
slug: mediatailor-api-list-prefetch-schedules-request
source_filename: mediatailor-api-list-prefetch-schedules-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-list-prefetch-schedules-request-schema.json\",\n  \"title\": \"ListPrefetchSchedulesRequest\",\n  \"description\": \"ListPrefetchSchedulesRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max100\"\n        },\n        {\n          \"description\": \"The maximum number of prefetch schedules that you want MediaTailor to return in response to the current request. If there are more than <code>MaxResults</code> prefetch schedules, use the value of <code>NextToken</code> in the response to get the next page of results.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"<p>(Optional) If the playback configuration has more than <code>MaxResults</code> prefetch schedules, use <code>NextToken</code> to get the second and subsequent pages of results.</p> <p> For the first <code>ListPrefetchSchedulesRequest</code> request, omit this value.</p> <p> For the second and subsequent requests, get the value of <code>NextToken</code> from the previous response and specify that value for <code>NextToken</code> in the request.</p> <p> If the previous response didn't include a <code>NextToken</code> element, there are no more prefetch schedules to get.</p>\"\n        }\n      ]\n    },\n    \"StreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"An optional filtering parameter whereby MediaTailor filters the prefetch schedules to include only specific streams.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-list-prefetch-schedules-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListPrefetchSchedulesRequest
---
