---
description: GetQualificationScoreResponse schema from Amazon Mechanical Turk API
layout: schema
name: GetQualificationScoreResponse
properties_list:
- description: ''
  name: Qualification
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-get-qualification-score-response-schema.json
slug: amazon-mechanical-turk-get-qualification-score-response
source_filename: amazon-mechanical-turk-get-qualification-score-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-qualification-score-response-schema.json\",\n  \"title\": \"GetQualificationScoreResponse\",\n  \"description\": \"GetQualificationScoreResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Qualification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Qualification\"\n        },\n        {\n          \"description\": \" The Qualification data structure of the Qualification assigned to a user, including the Qualification type and the value (score). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-qualification-score-response-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: GetQualificationScoreResponse
---
