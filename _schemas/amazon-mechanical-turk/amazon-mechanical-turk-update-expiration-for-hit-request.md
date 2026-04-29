---
description: UpdateExpirationForHITRequest schema from Amazon Mechanical Turk API
layout: schema
name: UpdateExpirationForHITRequest
properties_list:
- description: ''
  name: HITId
  type: object
- description: ''
  name: ExpireAt
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-update-expiration-for-hit-request-schema.json
slug: amazon-mechanical-turk-update-expiration-for-hit-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-expiration-for-hit-request-schema.json\",\n  \"title\": \"UpdateExpirationForHITRequest\",\n  \"description\": \"UpdateExpirationForHITRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The HIT to update. \"\n        }\n      ]\n    },\n    \"ExpireAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time at which you want the HIT to expire \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HITId\",\n    \"ExpireAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-expiration-for-hit-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: UpdateExpirationForHITRequest
---
