---
description: Option for host instance type.
layout: schema
name: BrokerInstanceOption
properties_list:
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: EngineType
  type: object
- description: ''
  name: HostInstanceType
  type: object
- description: ''
  name: StorageType
  type: object
- description: ''
  name: SupportedDeploymentModes
  type: object
- description: ''
  name: SupportedEngineVersions
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-broker-instance-option-schema.json
slug: mq-api-broker-instance-option
source_filename: mq-api-broker-instance-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-instance-option-schema.json\",\n  \"title\": \"BrokerInstanceOption\",\n  \"description\": \"Option for host instance type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAvailabilityZone\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZones\"\n          },\n          \"description\": \"The list of available az.\"\n        }\n      ]\n    },\n    \"EngineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineType\"\n          },\n          \"description\": \"The broker's engine type.\"\n        }\n      ]\n    },\n    \"HostInstanceType\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hostInstanceType\"\n          },\n          \"description\": \"The broker's instance type.\"\n        }\n      ]\n    },\n    \"StorageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerStorageType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"storageType\"\n          },\n          \"description\": \"The broker's storage type.\"\n        }\n      ]\n    },\n    \"SupportedDeploymentModes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfDeploymentMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"supportedDeploymentModes\"\n          },\n          \"description\": \"The list of supported deployment modes.\"\n        }\n      ]\n    },\n    \"SupportedEngineVersions\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"supportedEngineVersions\"\n          },\n          \"description\": \"The list of supported engine versions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-instance-option-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BrokerInstanceOption
---
