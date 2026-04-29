---
description: GetHITResponse schema from Amazon Mechanical Turk API
layout: schema
name: GetHITResponse
properties_list:
- description: ''
  name: HIT
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-get-hit-response-schema.json
slug: amazon-mechanical-turk-get-hit-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-hit-response-schema.json\",\n  \"title\": \"GetHITResponse\",\n  \"description\": \"GetHITResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HIT\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HIT\"\n        },\n        {\n          \"description\": \" Contains the requested HIT data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-hit-response-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: GetHITResponse
---
