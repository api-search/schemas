---
description: Broker configuration information
layout: schema
name: Configurations
properties_list:
- description: ''
  name: Current
  type: object
- description: ''
  name: History
  type: object
- description: ''
  name: Pending
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-configurations-schema.json
slug: mq-api-configurations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-configurations-schema.json\",\n  \"title\": \"Configurations\",\n  \"description\": \"Broker configuration information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Current\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"current\"\n          },\n          \"description\": \"The broker's current configuration.\"\n        }\n      ]\n    },\n    \"History\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfConfigurationId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"history\"\n          },\n          \"description\": \"The history of configurations applied to the broker.\"\n        }\n      ]\n    },\n    \"Pending\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pending\"\n          },\n          \"description\": \"The broker's pending configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-configurations-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Configurations
---
