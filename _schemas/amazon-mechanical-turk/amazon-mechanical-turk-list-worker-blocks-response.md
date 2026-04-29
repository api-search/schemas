---
description: ListWorkerBlocksResponse schema from Amazon Mechanical Turk API
layout: schema
name: ListWorkerBlocksResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: NumResults
  type: object
- description: ''
  name: WorkerBlocks
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-worker-blocks-response-schema.json
slug: amazon-mechanical-turk-list-worker-blocks-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-worker-blocks-response-schema.json\",\n  \"title\": \"ListWorkerBlocksResponse\",\n  \"description\": \"ListWorkerBlocksResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    },\n    \"NumResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of assignments on the page in the filtered results list, equivalent to the number of assignments returned by this call.\"\n        }\n      ]\n    },\n    \"WorkerBlocks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkerBlockList\"\n        },\n        {\n       \
  \   \"description\": \" The list of WorkerBlocks, containing the collection of Worker IDs and reasons for blocking.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-worker-blocks-response-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListWorkerBlocksResponse
---
