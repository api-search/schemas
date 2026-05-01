---
description: Creates a new configuration for the specified configuration name. Amazon MQ uses the default configuration (the engine type and version).
layout: schema
name: CreateConfigurationRequest
properties_list:
- description: ''
  name: AuthenticationStrategy
  type: object
- description: ''
  name: EngineType
  type: object
- description: ''
  name: EngineVersion
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-create-configuration-request-schema.json
slug: mq-api-create-configuration-request
source_filename: mq-api-create-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-create-configuration-request-schema.json\",\n  \"title\": \"CreateConfigurationRequest\",\n  \"description\": \"Creates a new configuration for the specified configuration name. Amazon MQ uses the default configuration (the engine type and version).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthenticationStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationStrategy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"authenticationStrategy\"\n          },\n          \"description\": \"Optional. The authentication strategy associated with the configuration. The default is SIMPLE.\"\n        }\n      ]\n    },\n    \"EngineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n\
  \        },\n        {\n          \"xml\": {\n            \"name\": \"engineType\"\n          },\n          \"description\": \"Required. The type of broker engine. Currently, Amazon MQ supports ACTIVEMQ and RABBITMQ.\"\n        }\n      ]\n    },\n    \"EngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineVersion\"\n          },\n          \"description\": \"Required. The broker engine's version. For a list of supported engine versions, see <a href=\\\"https://docs.aws.amazon.com//amazon-mq/latest/developer-guide/broker-engine.html\\\">Supported engines</a>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Required. The name of the configuration. This value can\
  \ contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 1-150 characters long.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"Create tags when creating the configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EngineVersion\",\n    \"EngineType\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-create-configuration-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateConfigurationRequest
---
