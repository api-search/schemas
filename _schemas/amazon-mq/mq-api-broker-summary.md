---
description: Returns information about all brokers.
layout: schema
name: BrokerSummary
properties_list:
- description: ''
  name: BrokerArn
  type: object
- description: ''
  name: BrokerId
  type: object
- description: ''
  name: BrokerName
  type: object
- description: ''
  name: BrokerState
  type: object
- description: ''
  name: Created
  type: object
- description: ''
  name: DeploymentMode
  type: object
- description: ''
  name: EngineType
  type: object
- description: ''
  name: HostInstanceType
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-broker-summary-schema.json
slug: mq-api-broker-summary
source_filename: mq-api-broker-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-summary-schema.json\",\n  \"title\": \"BrokerSummary\",\n  \"description\": \"Returns information about all brokers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerArn\"\n          },\n          \"description\": \"The broker's Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"BrokerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerId\"\n          },\n          \"description\": \"The unique ID that Amazon MQ generates for the broker.\"\n        }\n      ]\n    },\n    \"BrokerName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerName\"\n          },\n          \"description\": \"The broker's name. This value is unique in your AWS account, 1-50 characters long, and containing only letters, numbers, dashes, and underscores, and must not contain white spaces, brackets, wildcard characters, or special characters.\"\n        }\n      ]\n    },\n    \"BrokerState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerState\"\n          },\n          \"description\": \"The broker's status.\"\n        }\n      ]\n    },\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"created\"\n          },\n          \"description\"\
  : \"The time when the broker was created.\"\n        }\n      ]\n    },\n    \"DeploymentMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deploymentMode\"\n          },\n          \"description\": \"The broker's deployment mode.\"\n        }\n      ]\n    },\n    \"EngineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineType\"\n          },\n          \"description\": \"The type of broker engine.\"\n        }\n      ]\n    },\n    \"HostInstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hostInstanceType\"\n          },\n          \"description\": \"The broker's instance type.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"DeploymentMode\",\n    \"EngineType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-summary-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BrokerSummary
---
