---
description: Settings for for a PULL type input.
layout: schema
name: InputSourceRequest
properties_list:
- description: ''
  name: PasswordParam
  type: object
- description: ''
  name: Url
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-source-request-schema.json
slug: medialive-api-input-source-request
source_filename: medialive-api-input-source-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-source-request-schema.json\",\n  \"title\": \"InputSourceRequest\",\n  \"description\": \"Settings for for a PULL type input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PasswordParam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"passwordParam\"\n          },\n          \"description\": \"The key used to extract the password from EC2 Parameter store.\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"This represents the customer's source URL where stream is\\\
  npulled from.\\n\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"The username for the input source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-source-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputSourceRequest
---
