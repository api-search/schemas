---
description: Details about the error.
layout: schema
name: ErrorDetail
properties_list:
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-error-detail-schema.json
slug: amazon-marketplace-error-detail
source_filename: amazon-marketplace-error-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-error-detail-schema.json\",\n  \"title\": \"ErrorDetail\",\n  \"description\": \"Details about the error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCodeString\"\n        },\n        {\n          \"description\": \"The error code that identifies the type of error.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExceptionMessageContent\"\n        },\n        {\n          \"description\": \"The message for the error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-error-detail-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: ErrorDetail
---
