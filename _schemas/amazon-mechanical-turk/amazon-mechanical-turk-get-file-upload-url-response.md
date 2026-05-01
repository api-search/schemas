---
description: GetFileUploadURLResponse schema from Amazon Mechanical Turk API
layout: schema
name: GetFileUploadURLResponse
properties_list:
- description: ''
  name: FileUploadURL
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-get-file-upload-url-response-schema.json
slug: amazon-mechanical-turk-get-file-upload-url-response
source_filename: amazon-mechanical-turk-get-file-upload-url-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-file-upload-url-response-schema.json\",\n  \"title\": \"GetFileUploadURLResponse\",\n  \"description\": \"GetFileUploadURLResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileUploadURL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A temporary URL for the file that the Worker uploaded for the answer. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-file-upload-url-response-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: GetFileUploadURLResponse
---
