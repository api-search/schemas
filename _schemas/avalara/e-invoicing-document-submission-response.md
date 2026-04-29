---
description: DocumentSubmissionResponse schema from Avalara API
layout: schema
name: DocumentSubmissionResponse
properties_list:
- description: Document submission ID
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: statusDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-document-submission-response-schema.json
slug: e-invoicing-document-submission-response
source_filename: e-invoicing-document-submission-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-submission-response-schema.json\",\n  \"title\": \"DocumentSubmissionResponse\",\n  \"description\": \"DocumentSubmissionResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Document submission ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Accepted\",\n        \"Rejected\",\n        \"Error\"\n      ]\n    },\n    \"statusDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-submission-response-schema.json
tags:
- Taxes
title: DocumentSubmissionResponse
---
