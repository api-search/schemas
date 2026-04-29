---
description: UpdateHITTypeOfHITRequest schema from Amazon Mechanical Turk API
layout: schema
name: UpdateHITTypeOfHITRequest
properties_list:
- description: ''
  name: HITId
  type: object
- description: ''
  name: HITTypeId
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-update-hit-type-of-hit-request-schema.json
slug: amazon-mechanical-turk-update-hit-type-of-hit-request
source_filename: amazon-mechanical-turk-update-hit-type-of-hit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-hit-type-of-hit-request-schema.json\",\n  \"title\": \"UpdateHITTypeOfHITRequest\",\n  \"description\": \"UpdateHITTypeOfHITRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The HIT to update.\"\n        }\n      ]\n    },\n    \"HITTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the new HIT type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HITId\",\n    \"HITTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-hit-type-of-hit-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: UpdateHITTypeOfHITRequest
---
