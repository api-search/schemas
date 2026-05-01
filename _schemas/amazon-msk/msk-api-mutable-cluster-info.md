---
description: <p>Information about cluster attributes that can be updated via update APIs.</p>
layout: schema
name: MutableClusterInfo
properties_list:
- description: ''
  name: BrokerEBSVolumeInfo
  type: object
- description: ''
  name: ConfigurationInfo
  type: object
- description: ''
  name: NumberOfBrokerNodes
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
  name: InstanceType
  type: object
- description: ''
  name: ClientAuthentication
  type: object
- description: ''
  name: EncryptionInfo
  type: object
- description: ''
  name: ConnectivityInfo
  type: object
- description: ''
  name: StorageMode
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-mutable-cluster-info-schema.json
slug: msk-api-mutable-cluster-info
source_filename: msk-api-mutable-cluster-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-mutable-cluster-info-schema.json\",\n  \"title\": \"MutableClusterInfo\",\n  \"description\": \"\\n            <p>Information about cluster attributes that can be updated via update APIs.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerEBSVolumeInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBrokerEBSVolumeInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerEBSVolumeInfo\"\n          },\n          \"description\": \"\\n            <p>Specifies the size of the EBS volume and the ID of the associated broker.</p>\"\n        }\n      ]\n    },\n    \"ConfigurationInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationInfo\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"configurationInfo\"\n          },\n          \"description\": \"\\n            <p>Information about the changes in the configuration of the brokers.</p>\"\n        }\n      ]\n    },\n    \"NumberOfBrokerNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"numberOfBrokerNodes\"\n          },\n          \"description\": \"\\n            <p>The number of broker nodes in the cluster.</p>\"\n        }\n      ]\n    },\n    \"EnhancedMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnhancedMonitoring\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enhancedMonitoring\"\n          },\n          \"description\": \"\\n            <p>Specifies which Apache Kafka metrics Amazon MSK gathers and sends to Amazon CloudWatch for this cluster.</p>\"\n        }\n      ]\n    },\n    \"OpenMonitoring\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenMonitoring\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"openMonitoring\"\n          },\n          \"description\": \"\\n            <p>The settings for open monitoring.</p>\"\n        }\n      ]\n    },\n    \"KafkaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kafkaVersion\"\n          },\n          \"description\": \"\\n            <p>The Apache Kafka version.</p>\"\n        }\n      ]\n    },\n    \"LoggingInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loggingInfo\"\n          },\n          \"description\": \"\\n            <p>You can configure your MSK cluster to send broker logs to different destination types. This is a container for\
  \ the configuration details related to broker logs.</p>\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin5Max32\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceType\"\n          },\n          \"description\": \"\\n            <p>Information about the Amazon MSK broker type.</p>\"\n        }\n      ]\n    },\n    \"ClientAuthentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientAuthentication\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientAuthentication\"\n          },\n          \"description\": \"\\n            <p>Includes all client authentication information.</p>\"\n        }\n      ]\n    },\n    \"EncryptionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionInfo\"\
  \n          },\n          \"description\": \"\\n            <p>Includes all encryption-related information.</p>\"\n        }\n      ]\n    },\n    \"ConnectivityInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectivityInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"connectivityInfo\"\n          },\n          \"description\": \"\\n            <p>Information about the broker access configuration.</p>\"\n        }\n      ]\n    },\n    \"StorageMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"storageMode\"\n          },\n          \"description\": \"\\n            <p>This controls storage mode for supported storage tiers.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-mutable-cluster-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MutableClusterInfo
---
