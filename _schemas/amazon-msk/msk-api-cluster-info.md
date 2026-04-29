---
description: <p>Returns information about a cluster.</p>
layout: schema
name: ClusterInfo
properties_list:
- description: ''
  name: ActiveOperationArn
  type: object
- description: ''
  name: BrokerNodeGroupInfo
  type: object
- description: ''
  name: ClientAuthentication
  type: object
- description: ''
  name: ClusterArn
  type: object
- description: ''
  name: ClusterName
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: CurrentBrokerSoftwareInfo
  type: object
- description: ''
  name: CurrentVersion
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
  name: State
  type: object
- description: ''
  name: StateInfo
  type: object
- description: ''
  name: Tags
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
schema_file: json-schema/msk-api-cluster-info-schema.json
slug: msk-api-cluster-info
source_filename: msk-api-cluster-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-info-schema.json\",\n  \"title\": \"ClusterInfo\",\n  \"description\": \"\\n            <p>Returns information about a cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveOperationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeOperationArn\"\n          },\n          \"description\": \"\\n            <p>Arn of active cluster operation.</p>\"\n        }\n      ]\n    },\n    \"BrokerNodeGroupInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerNodeGroupInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerNodeGroupInfo\"\n          },\n          \"description\": \"\\n            <p>Information\
  \ about the broker nodes.</p>\"\n        }\n      ]\n    },\n    \"ClientAuthentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientAuthentication\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientAuthentication\"\n          },\n          \"description\": \"\\n            <p>Includes all client authentication information.</p>\"\n        }\n      ]\n    },\n    \"ClusterArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterArn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) that uniquely identifies the cluster.</p>\"\n        }\n      ]\n    },\n    \"ClusterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterName\"\n          },\n     \
  \     \"description\": \"\\n            <p>The name of the cluster.</p>\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creationTime\"\n          },\n          \"description\": \"\\n            <p>The time when the cluster was created.</p>\"\n        }\n      ]\n    },\n    \"CurrentBrokerSoftwareInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerSoftwareInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentBrokerSoftwareInfo\"\n          },\n          \"description\": \"\\n            <p>Information about the version of software currently deployed on the Apache Kafka brokers in the cluster.</p>\"\n        }\n      ]\n    },\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\": \"\\n            <p>The current version of the MSK cluster.</p>\"\n        }\n      ]\n    },\n    \"EncryptionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionInfo\"\n          },\n          \"description\": \"\\n            <p>Includes all encryption-related information.</p>\"\n        }\n      ]\n    },\n    \"EnhancedMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnhancedMonitoring\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enhancedMonitoring\"\n          },\n          \"description\": \"\\n            <p>Specifies which metrics are gathered for the MSK cluster. This property has the following possible values: DEFAULT, PER_BROKER, PER_TOPIC_PER_BROKER, and PER_TOPIC_PER_PARTITION.\
  \ For a list of the metrics associated with each of these levels of monitoring, see <a href=\\\"https://docs.aws.amazon.com/msk/latest/developerguide/monitoring.html\\\">Monitoring</a>.</p>\"\n        }\n      ]\n    },\n    \"OpenMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenMonitoring\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"openMonitoring\"\n          },\n          \"description\": \"\\n            <p>Settings for open monitoring using Prometheus.</p>\"\n        }\n      ]\n    },\n    \"LoggingInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loggingInfo\"\n          }\n        }\n      ]\n    },\n    \"NumberOfBrokerNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"numberOfBrokerNodes\"\
  \n          },\n          \"description\": \"\\n            <p>The number of broker nodes in the cluster.</p>\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"\\n            <p>The state of the cluster. The possible states are ACTIVE, CREATING, DELETING, FAILED, HEALING, MAINTENANCE, REBOOTING_BROKER, and UPDATING.</p>\"\n        }\n      ]\n    },\n    \"StateInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stateInfo\"\n          }\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n   \
  \       \"description\": \"\\n            <p>Tags attached to the cluster.</p>\"\n        }\n      ]\n    },\n    \"ZookeeperConnectString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"zookeeperConnectString\"\n          },\n          \"description\": \"\\n            <p>The connection string to use to connect to the Apache ZooKeeper cluster.</p>\"\n        }\n      ]\n    },\n    \"ZookeeperConnectStringTls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"zookeeperConnectStringTls\"\n          },\n          \"description\": \"\\n            <p>The connection string to use to connect to zookeeper cluster on Tls port.</p>\"\n        }\n      ]\n    },\n    \"StorageMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageMode\"\n\
  \        },\n        {\n          \"xml\": {\n            \"name\": \"storageMode\"\n          },\n          \"description\": \"\\n            <p>This controls storage mode for supported storage tiers.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ClusterInfo
---
