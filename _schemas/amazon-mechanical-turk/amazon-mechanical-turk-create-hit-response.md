---
description: CreateHITResponse schema from Amazon Mechanical Turk API
layout: schema
name: CreateHITResponse
properties_list:
- description: ''
  name: HIT
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-create-hit-response-schema.json
slug: amazon-mechanical-turk-create-hit-response
source_filename: amazon-mechanical-turk-create-hit-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-hit-response-schema.json\",\n  \"title\": \"CreateHITResponse\",\n  \"description\": \"CreateHITResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HIT\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HIT\"\n        },\n        {\n          \"description\": \" Contains the newly created HIT data. For a description of the HIT data structure as it appears in responses, see the HIT Data Structure documentation. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-hit-response-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: CreateHITResponse
---
