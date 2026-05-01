---
description: GetQualificationTypeResponse schema from Amazon Mechanical Turk API
layout: schema
name: GetQualificationTypeResponse
properties_list:
- description: ''
  name: QualificationType
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-get-qualification-type-response-schema.json
slug: amazon-mechanical-turk-get-qualification-type-response
source_filename: amazon-mechanical-turk-get-qualification-type-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-qualification-type-response-schema.json\",\n  \"title\": \"GetQualificationTypeResponse\",\n  \"description\": \"GetQualificationTypeResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QualificationType\"\n        },\n        {\n          \"description\": \" The returned Qualification Type\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-qualification-type-response-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: GetQualificationTypeResponse
---
