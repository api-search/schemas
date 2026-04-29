---
description: RejectQualificationRequestRequest schema from Amazon Mechanical Turk API
layout: schema
name: RejectQualificationRequestRequest
properties_list:
- description: ''
  name: QualificationRequestId
  type: object
- description: ''
  name: Reason
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-reject-qualification-request-request-schema.json
slug: amazon-mechanical-turk-reject-qualification-request-request
source_filename: amazon-mechanical-turk-reject-qualification-request-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-reject-qualification-request-request-schema.json\",\n  \"title\": \"RejectQualificationRequestRequest\",\n  \"description\": \"RejectQualificationRequestRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The ID of the Qualification request, as returned by the <code>ListQualificationRequests</code> operation. \"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A text message explaining why the request was rejected, to be shown\
  \ to the Worker who made the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QualificationRequestId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-reject-qualification-request-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: RejectQualificationRequestRequest
---
