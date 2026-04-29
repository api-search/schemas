---
description: Returns information about the XML element or attribute that was sanitized in the configuration.
layout: schema
name: SanitizationWarning
properties_list:
- description: ''
  name: AttributeName
  type: object
- description: ''
  name: ElementName
  type: object
- description: ''
  name: Reason
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-sanitization-warning-schema.json
slug: mq-api-sanitization-warning
source_filename: mq-api-sanitization-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-sanitization-warning-schema.json\",\n  \"title\": \"SanitizationWarning\",\n  \"description\": \"Returns information about the XML element or attribute that was sanitized in the configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attributeName\"\n          },\n          \"description\": \"The name of the XML attribute that has been sanitized.\"\n        }\n      ]\n    },\n    \"ElementName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"elementName\"\n          },\n          \"description\": \"The name\
  \ of the XML element that has been sanitized.\"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SanitizationWarningReason\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reason\"\n          },\n          \"description\": \"Required. The reason for which the XML elements or attributes were sanitized.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Reason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-sanitization-warning-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: SanitizationWarning
---
