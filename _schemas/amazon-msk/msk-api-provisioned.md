---
description: <p>Provisioned cluster.</p>
layout: schema
name: Provisioned
properties_list:
- description: ''
  name: BrokerNodeGroupInfo
  type: object
- description: ''
  name: CurrentBrokerSoftwareInfo
  type: object
- description: ''
  name: ClientAuthentication
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
  name: LoggingInfo
  type: object
- description: ''
  name: NumberOfBrokerNodes
  type: object
- description: ''
  name: ZookeeperConnectString
  type: object
- description: ''
  name: ZookeeperConnectStringTls
  type: object
- description: ''
  name: StorageMode
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-provisioned-schema.json
slug: msk-api-provisioned
source_filename: msk-api-provisioned-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-provisioned-schema.json\",\n  \"title\": \"Provisioned\",\n  \"description\": \"\\n            <p>Provisioned cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerNodeGroupInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerNodeGroupInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerNodeGroupInfo\"\n          },\n          \"description\": \"\\n            <p>Information about the brokers.</p>\"\n        }\n      ]\n    },\n    \"CurrentBrokerSoftwareInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerSoftwareInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentBrokerSoftwareInfo\"\n          },\n          \"description\": \"\\n          \
  \  <p>Information about the Apache Kafka version deployed on the brokers.</p>\"\n        }\n      ]\n    },\n    \"ClientAuthentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientAuthentication\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientAuthentication\"\n          },\n          \"description\": \"\\n            <p>Includes all client authentication information.</p>\"\n        }\n      ]\n    },\n    \"EncryptionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionInfo\"\n          },\n          \"description\": \"\\n            <p>Includes all encryption-related information.</p>\"\n        }\n      ]\n    },\n    \"EnhancedMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnhancedMonitoring\"\n        },\n        {\n          \"xml\": {\n   \
  \         \"name\": \"enhancedMonitoring\"\n          },\n          \"description\": \"\\n            <p>Specifies the level of monitoring for the MSK cluster. The possible values are DEFAULT, PER_BROKER, PER_TOPIC_PER_BROKER, and PER_TOPIC_PER_PARTITION.</p>\"\n        }\n      ]\n    },\n    \"OpenMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenMonitoringInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"openMonitoring\"\n          },\n          \"description\": \"\\n            <p>The settings for open monitoring.</p>\"\n        }\n      ]\n    },\n    \"LoggingInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loggingInfo\"\n          },\n          \"description\": \"\\n            <p>Log delivery information for the cluster.</p>\"\n        }\n      ]\n    },\n    \"NumberOfBrokerNodes\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max15\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"numberOfBrokerNodes\"\n          },\n          \"description\": \"\\n            <p>The number of broker nodes in the cluster.</p>\"\n        }\n      ]\n    },\n    \"ZookeeperConnectString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"zookeeperConnectString\"\n          },\n          \"description\": \"\\n            <p>The connection string to use to connect to the Apache ZooKeeper cluster.</p>\"\n        }\n      ]\n    },\n    \"ZookeeperConnectStringTls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"zookeeperConnectStringTls\"\n          },\n          \"description\": \"\\n            <p>The connection\
  \ string to use to connect to the Apache ZooKeeper cluster on a TLS port.</p>\"\n        }\n      ]\n    },\n    \"StorageMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"storageMode\"\n          },\n          \"description\": \"\\n            <p>This controls storage mode for supported storage tiers.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BrokerNodeGroupInfo\",\n    \"NumberOfBrokerNodes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-provisioned-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Provisioned
---
