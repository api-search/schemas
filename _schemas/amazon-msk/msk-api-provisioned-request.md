---
description: <p>Provisioned cluster request.</p>
layout: schema
name: ProvisionedRequest
properties_list:
- description: ''
  name: BrokerNodeGroupInfo
  type: object
- description: ''
  name: ClientAuthentication
  type: object
- description: ''
  name: ConfigurationInfo
  type: object
- description: ''
  name: EncryptionInfo
  type: object
- description: ''
  name: EnhancedMonitoring
  type: object
- description: ''
  name: OpenMonitoring
  type: object
- description: ''
  name: KafkaVersion
  type: object
- description: ''
  name: LoggingInfo
  type: object
- description: ''
  name: NumberOfBrokerNodes
  type: object
- description: ''
  name: StorageMode
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-provisioned-request-schema.json
slug: msk-api-provisioned-request
source_filename: msk-api-provisioned-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-provisioned-request-schema.json\",\n  \"title\": \"ProvisionedRequest\",\n  \"description\": \"\\n            <p>Provisioned cluster request.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerNodeGroupInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerNodeGroupInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerNodeGroupInfo\"\n          },\n          \"description\": \"\\n            <p>Information about the brokers.</p>\"\n        }\n      ]\n    },\n    \"ClientAuthentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientAuthentication\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientAuthentication\"\n          },\n          \"description\": \"\
  \\n            <p>Includes all client authentication information.</p>\"\n        }\n      ]\n    },\n    \"ConfigurationInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurationInfo\"\n          },\n          \"description\": \"\\n            <p>Represents the configuration that you want Amazon MSK to use for the brokers in a cluster.</p>\"\n        }\n      ]\n    },\n    \"EncryptionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionInfo\"\n          },\n          \"description\": \"\\n            <p>Includes all encryption-related information.</p>\"\n        }\n      ]\n    },\n    \"EnhancedMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnhancedMonitoring\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"enhancedMonitoring\"\n          },\n          \"description\": \"\\n            <p>Specifies the level of monitoring for the MSK cluster. The possible values are DEFAULT, PER_BROKER, PER_TOPIC_PER_BROKER, and PER_TOPIC_PER_PARTITION.</p>\"\n        }\n      ]\n    },\n    \"OpenMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenMonitoringInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"openMonitoring\"\n          },\n          \"description\": \"\\n            <p>The settings for open monitoring.</p>\"\n        }\n      ]\n    },\n    \"KafkaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max128\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kafkaVersion\"\n          },\n          \"description\": \"\\n            <p>The Apache Kafka version that you want for the cluster.</p>\"\n        }\n  \
  \    ]\n    },\n    \"LoggingInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loggingInfo\"\n          },\n          \"description\": \"\\n            <p>Log delivery information for the cluster.</p>\"\n        }\n      ]\n    },\n    \"NumberOfBrokerNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max15\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"numberOfBrokerNodes\"\n          },\n          \"description\": \"\\n            <p>The number of broker nodes in the cluster.</p>\"\n        }\n      ]\n    },\n    \"StorageMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"storageMode\"\n          },\n          \"description\": \"\\n            <p>This controls storage mode for supported\
  \ storage tiers.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BrokerNodeGroupInfo\",\n    \"KafkaVersion\",\n    \"NumberOfBrokerNodes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-provisioned-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ProvisionedRequest
---
