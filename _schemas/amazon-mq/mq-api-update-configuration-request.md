---
description: Updates the specified configuration.
layout: schema
name: UpdateConfigurationRequest
properties_list:
- description: ''
  name: Data
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-update-configuration-request-schema.json
slug: mq-api-update-configuration-request
source_filename: mq-api-update-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-update-configuration-request-schema.json\",\n  \"title\": \"UpdateConfigurationRequest\",\n  \"description\": \"Updates the specified configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"data\"\n          },\n          \"description\": \"Required. The base64-encoded XML configuration.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The description of the configuration.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"Data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-update-configuration-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateConfigurationRequest
---
