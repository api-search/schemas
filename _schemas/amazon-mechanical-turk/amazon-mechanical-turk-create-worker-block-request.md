---
description: CreateWorkerBlockRequest schema from Amazon Mechanical Turk API
layout: schema
name: CreateWorkerBlockRequest
properties_list:
- description: ''
  name: WorkerId
  type: object
- description: ''
  name: Reason
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-create-worker-block-request-schema.json
slug: amazon-mechanical-turk-create-worker-block-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-worker-block-request-schema.json\",\n  \"title\": \"CreateWorkerBlockRequest\",\n  \"description\": \"CreateWorkerBlockRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \"The ID of the Worker to block.\"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A message explaining the reason for blocking the Worker. This parameter enables you to keep track of your Workers. The Worker does not see this message.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"WorkerId\",\n    \"Reason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-worker-block-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: CreateWorkerBlockRequest
---
