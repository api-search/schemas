---
description: ListWorkerBlocksRequest schema from Amazon Mechanical Turk API
layout: schema
name: ListWorkerBlocksRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-worker-blocks-request-schema.json
slug: amazon-mechanical-turk-list-worker-blocks-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-worker-blocks-request-schema.json\",\n  \"title\": \"ListWorkerBlocksRequest\",\n  \"description\": \"ListWorkerBlocksRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination token\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"$ref\": \"#/components/schemas/ResultSize\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-worker-blocks-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListWorkerBlocksRequest
---
