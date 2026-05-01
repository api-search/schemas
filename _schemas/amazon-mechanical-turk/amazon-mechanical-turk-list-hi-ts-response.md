---
description: ListHITsResponse schema from Amazon Mechanical Turk API
layout: schema
name: ListHITsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: NumResults
  type: object
- description: ''
  name: HITs
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-hi-ts-response-schema.json
slug: amazon-mechanical-turk-list-hi-ts-response
source_filename: amazon-mechanical-turk-list-hi-ts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-hi-ts-response-schema.json\",\n  \"title\": \"ListHITsResponse\",\n  \"description\": \"ListHITsResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    },\n    \"NumResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of HITs on this page in the filtered results list, equivalent to the number of HITs being returned by this call.\"\n        }\n      ]\n    },\n    \"HITs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HITList\"\n        },\n        {\n          \"description\": \" The list of HIT elements returned\
  \ by the query.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-hi-ts-response-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListHITsResponse
---
