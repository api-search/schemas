---
description: CreateConfigurationRequest schema from Amazon MSK API
layout: schema
name: CreateConfigurationRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: KafkaVersions
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: ServerProperties
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-create-configuration-request-schema.json
slug: msk-api-create-configuration-request
source_filename: msk-api-create-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-create-configuration-request-schema.json\",\n  \"title\": \"CreateConfigurationRequest\",\n  \"description\": \"CreateConfigurationRequest schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"\\n            <p>The description of the configuration.</p>\"\n        }\n      ]\n    },\n    \"KafkaVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kafkaVersions\"\n          },\n          \"description\": \"\\n            <p>The\
  \ versions of Apache Kafka with which you can use this MSK configuration.</p>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"\\n            <p>The name of the configuration.</p>\"\n        }\n      ]\n    },\n    \"ServerProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__blob\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serverProperties\"\n          },\n          \"description\": \"\\n            <p>Contents of the <filename>server.properties</filename> file. When using the API, you must ensure that the contents of the file are base64 encoded. \\n               When using the AWS Management Console, the SDK, or the AWS CLI, the contents of <filename>server.properties</filename> can be in plaintext.</p>\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"ServerProperties\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-create-configuration-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateConfigurationRequest
---
