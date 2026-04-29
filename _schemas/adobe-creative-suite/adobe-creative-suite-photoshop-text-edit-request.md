---
description: Request to edit text layer content and properties in a PSD
layout: schema
name: TextEditRequest
properties_list:
- description: ''
  name: inputs
  type: array
- description: ''
  name: outputs
  type: array
- description: ''
  name: options
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-text-edit-request-schema.json
slug: adobe-creative-suite-photoshop-text-edit-request
source_filename: adobe-creative-suite-photoshop-text-edit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-text-edit-request-schema.json\",\n  \"title\": \"TextEditRequest\",\n  \"description\": \"Request to edit text layer content and properties in a PSD\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobInput\"\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobOutput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"layers\": {\n          \"type\": \"array\",\n          \"description\": \"List of text layer edits to apply\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"\
  name\": {\n                \"type\": \"string\",\n                \"description\": \"Name of the text layer to edit\"\n              },\n              \"text\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"content\": {\n                    \"type\": \"string\",\n                    \"description\": \"New text content for the layer\"\n                  },\n                  \"characterStyles\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"fontSize\": {\n                          \"type\": \"number\"\n                        },\n                        \"fontName\": {\n                          \"type\": \"string\"\n                        },\n                        \"color\": {\n                          \"type\": \"object\",\n                          \"properties\": {\n                   \
  \         \"red\": {\n                              \"type\": \"integer\"\n                            },\n                            \"green\": {\n                              \"type\": \"integer\"\n                            },\n                            \"blue\": {\n                              \"type\": \"integer\"\n                            }\n                          }\n                        }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"outputs\",\n    \"options\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-text-edit-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: TextEditRequest
---
