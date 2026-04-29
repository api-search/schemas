---
description: Returns information about all configurations.
layout: schema
name: Configuration
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: AuthenticationStrategy
  type: object
- description: ''
  name: Created
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: EngineType
  type: object
- description: ''
  name: EngineVersion
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: LatestRevision
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-configuration-schema.json
slug: mq-api-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-configuration-schema.json\",\n  \"title\": \"Configuration\",\n  \"description\": \"Returns information about all configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"Required. The ARN of the configuration.\"\n        }\n      ]\n    },\n    \"AuthenticationStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationStrategy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"authenticationStrategy\"\n          },\n          \"description\": \"Optional. The authentication strategy associated with the configuration.\
  \ The default is SIMPLE.\"\n        }\n      ]\n    },\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"created\"\n          },\n          \"description\": \"Required. The date and time of the configuration revision.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"Required. The description of the configuration.\"\n        }\n      ]\n    },\n    \"EngineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineType\"\n          },\n          \"description\": \"Required. The type of broker engine. Currently, Amazon MQ supports\
  \ ACTIVEMQ and RABBITMQ.\"\n        }\n      ]\n    },\n    \"EngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineVersion\"\n          },\n          \"description\": \"Required. The broker engine's version. For a list of supported engine versions, see, <a href=\\\"https://docs.aws.amazon.com//amazon-mq/latest/developer-guide/broker-engine.html\\\">Supported engines</a>.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"Required. The unique ID that Amazon MQ generates for the configuration.\"\n        }\n      ]\n    },\n    \"LatestRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRevision\"\n        },\n      \
  \  {\n          \"xml\": {\n            \"name\": \"latestRevision\"\n          },\n          \"description\": \"Required. The latest revision of the configuration.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Required. The name of the configuration. This value can contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 1-150 characters long.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The list of all tags associated with this configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Description\"\
  ,\n    \"EngineVersion\",\n    \"LatestRevision\",\n    \"AuthenticationStrategy\",\n    \"EngineType\",\n    \"Id\",\n    \"Arn\",\n    \"Name\",\n    \"Created\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Configuration
---
