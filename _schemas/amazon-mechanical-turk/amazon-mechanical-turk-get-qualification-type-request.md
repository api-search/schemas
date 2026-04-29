---
description: GetQualificationTypeRequest schema from Amazon Mechanical Turk API
layout: schema
name: GetQualificationTypeRequest
properties_list:
- description: ''
  name: QualificationTypeId
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-get-qualification-type-request-schema.json
slug: amazon-mechanical-turk-get-qualification-type-request
source_filename: amazon-mechanical-turk-get-qualification-type-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-qualification-type-request-schema.json\",\n  \"title\": \"GetQualificationTypeRequest\",\n  \"description\": \"GetQualificationTypeRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the QualificationType.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QualificationTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-qualification-type-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: GetQualificationTypeRequest
---
