---
description: DeleteWorkerBlockRequest schema from Amazon Mechanical Turk API
layout: schema
name: DeleteWorkerBlockRequest
properties_list:
- description: ''
  name: WorkerId
  type: object
- description: ''
  name: Reason
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-delete-worker-block-request-schema.json
slug: amazon-mechanical-turk-delete-worker-block-request
source_filename: amazon-mechanical-turk-delete-worker-block-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-delete-worker-block-request-schema.json\",\n  \"title\": \"DeleteWorkerBlockRequest\",\n  \"description\": \"DeleteWorkerBlockRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \"The ID of the Worker to unblock.\"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A message that explains the reason for unblocking the Worker. The Worker does not see this message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"WorkerId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-delete-worker-block-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: DeleteWorkerBlockRequest
---
