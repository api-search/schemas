---
description: DeleteHITRequest schema from Amazon Mechanical Turk API
layout: schema
name: DeleteHITRequest
properties_list:
- description: ''
  name: HITId
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-delete-hit-request-schema.json
slug: amazon-mechanical-turk-delete-hit-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-delete-hit-request-schema.json\",\n  \"title\": \"DeleteHITRequest\",\n  \"description\": \"DeleteHITRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the HIT to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HITId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-delete-hit-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: DeleteHITRequest
---
