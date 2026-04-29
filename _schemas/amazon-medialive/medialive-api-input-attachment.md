---
description: Placeholder documentation for InputAttachment
layout: schema
name: InputAttachment
properties_list:
- description: ''
  name: AutomaticInputFailoverSettings
  type: object
- description: ''
  name: InputAttachmentName
  type: object
- description: ''
  name: InputId
  type: object
- description: ''
  name: InputSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-attachment-schema.json
slug: medialive-api-input-attachment
source_filename: medialive-api-input-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-attachment-schema.json\",\n  \"title\": \"InputAttachment\",\n  \"description\": \"Placeholder documentation for InputAttachment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutomaticInputFailoverSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomaticInputFailoverSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"automaticInputFailoverSettings\"\n          },\n          \"description\": \"User-specified settings for defining what the conditions are for declaring the input unhealthy and failing over to a different input.\"\n        }\n      ]\n    },\n    \"InputAttachmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n         \
  \ \"xml\": {\n            \"name\": \"inputAttachmentName\"\n          },\n          \"description\": \"User-specified name for the attachment. This is required if the user wants to use this input in an input switch action.\"\n        }\n      ]\n    },\n    \"InputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputId\"\n          },\n          \"description\": \"The ID of the input\"\n        }\n      ]\n    },\n    \"InputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSettings\"\n          },\n          \"description\": \"Settings of an input (caption selector, etc.)\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-attachment-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputAttachment
---
