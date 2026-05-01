---
description: GetFileUploadURLRequest schema from Amazon Mechanical Turk API
layout: schema
name: GetFileUploadURLRequest
properties_list:
- description: ''
  name: AssignmentId
  type: object
- description: ''
  name: QuestionIdentifier
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-get-file-upload-url-request-schema.json
slug: amazon-mechanical-turk-get-file-upload-url-request
source_filename: amazon-mechanical-turk-get-file-upload-url-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-file-upload-url-request-schema.json\",\n  \"title\": \"GetFileUploadURLRequest\",\n  \"description\": \"GetFileUploadURLRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssignmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the assignment that contains the question with a FileUploadAnswer.\"\n        }\n      ]\n    },\n    \"QuestionIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier of the question with a FileUploadAnswer, as specified in the QuestionForm of the HIT.\"\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"AssignmentId\",\n    \"QuestionIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-file-upload-url-request-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: GetFileUploadURLRequest
---
