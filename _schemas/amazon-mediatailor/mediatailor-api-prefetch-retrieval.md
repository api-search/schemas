---
description: A complex type that contains settings governing when MediaTailor prefetches ads, and which dynamic variables that MediaTailor includes in the request to the ad decision server.
layout: schema
name: PrefetchRetrieval
properties_list:
- description: ''
  name: DynamicVariables
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: StartTime
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-prefetch-retrieval-schema.json
slug: mediatailor-api-prefetch-retrieval
source_filename: mediatailor-api-prefetch-retrieval-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-prefetch-retrieval-schema.json\",\n  \"title\": \"PrefetchRetrieval\",\n  \"description\": \"A complex type that contains settings governing when MediaTailor prefetches ads, and which dynamic variables that MediaTailor includes in the request to the ad decision server.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DynamicVariables\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"description\": \"<p>The dynamic variables to use for substitution during prefetch requests to the ad decision server (ADS).</p> <p>You initially configure <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/variables.html\\\">dynamic variables</a> for the ADS URL when you set up your playback configuration.\
  \ When you specify <code>DynamicVariables</code> for prefetch retrieval, MediaTailor includes the dynamic variables in the request to the ADS.</p>\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The time when prefetch retrieval ends for the ad break. Prefetching will be attempted for manifest requests that occur at or before this time.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The time when prefetch retrievals can start for this break. Ad prefetching will be attempted for manifest requests that occur at or after this time. Defaults to the current time. If not specified, the prefetch retrieval starts as soon as possible.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndTime\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-prefetch-retrieval-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PrefetchRetrieval
---
