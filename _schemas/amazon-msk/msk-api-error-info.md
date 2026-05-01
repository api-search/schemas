---
description: <p>Returns information about an error state of the cluster.</p>
layout: schema
name: ErrorInfo
properties_list:
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorString
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-error-info-schema.json
slug: msk-api-error-info
source_filename: msk-api-error-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-error-info-schema.json\",\n  \"title\": \"ErrorInfo\",\n  \"description\": \"\\n            <p>Returns information about an error state of the cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorCode\"\n          },\n          \"description\": \"\\n            <p>A number describing the error programmatically.</p>\"\n        }\n      ]\n    },\n    \"ErrorString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorString\"\n          },\n          \"description\": \"\\n            <p>An optional field\
  \ to provide more details about the error.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-error-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ErrorInfo
---
