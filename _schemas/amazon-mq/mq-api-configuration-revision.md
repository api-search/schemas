---
description: Returns information about the specified configuration revision.
layout: schema
name: ConfigurationRevision
properties_list:
- description: ''
  name: Created
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Revision
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-configuration-revision-schema.json
slug: mq-api-configuration-revision
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-configuration-revision-schema.json\",\n  \"title\": \"ConfigurationRevision\",\n  \"description\": \"Returns information about the specified configuration revision.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"created\"\n          },\n          \"description\": \"Required. The date and time of the configuration revision.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The description of the configuration\
  \ revision.\"\n        }\n      ]\n    },\n    \"Revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"revision\"\n          },\n          \"description\": \"Required. The revision number of the configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Revision\",\n    \"Created\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-configuration-revision-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ConfigurationRevision
---
