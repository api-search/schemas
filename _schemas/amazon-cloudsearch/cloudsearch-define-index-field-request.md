---
description: DefineIndexFieldRequest schema
layout: schema
name: DefineIndexFieldRequest
properties_list:
- description: ''
  name: IndexField
  type: object
provider_name: Amazon CloudSearch
provider_slug: amazon-cloudsearch
schema_file: json-schema/cloudsearch-define-index-field-request-schema.json
slug: cloudsearch-define-index-field-request
source_filename: cloudsearch-define-index-field-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-define-index-field-request-schema.json\",\n  \"title\": \"DefineIndexFieldRequest\",\n  \"description\": \"DefineIndexFieldRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IndexField\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"IndexFieldName\",\n        \"IndexFieldType\"\n      ],\n      \"properties\": {\n        \"IndexFieldName\": {\n          \"type\": \"string\"\n        },\n        \"IndexFieldType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"int\",\n            \"double\",\n            \"literal\",\n            \"text\",\n            \"date\",\n            \"latlon\",\n            \"int-array\",\n            \"double-array\",\n            \"literal-array\",\n            \"text-array\",\n            \"date-array\"\
  \n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"IndexField\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-define-index-field-request-schema.json
tags:
- CloudSearch
- Search
- Full-Text Search
- Managed
title: DefineIndexFieldRequest
---
