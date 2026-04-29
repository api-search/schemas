---
description: <p>Describes the setup to be used for Apache Kafka broker nodes in the cluster.</p>
layout: schema
name: BrokerNodeGroupInfo
properties_list:
- description: ''
  name: BrokerAZDistribution
  type: object
- description: ''
  name: ClientSubnets
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: SecurityGroups
  type: object
- description: ''
  name: StorageInfo
  type: object
- description: ''
  name: ConnectivityInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-broker-node-group-info-schema.json
slug: msk-api-broker-node-group-info
source_filename: msk-api-broker-node-group-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-node-group-info-schema.json\",\n  \"title\": \"BrokerNodeGroupInfo\",\n  \"description\": \"\\n            <p>Describes the setup to be used for Apache Kafka broker nodes in the cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerAZDistribution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerAZDistribution\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerAZDistribution\"\n          },\n          \"description\": \"\\n            <p>The distribution of broker nodes across Availability Zones. This is an optional parameter. If you don't specify it, Amazon MSK gives it the value DEFAULT. You can also explicitly set this parameter to the value DEFAULT. No other values are currently allowed.</p>\\n         <p>Amazon\
  \ MSK distributes the broker nodes evenly across the Availability Zones that correspond to the subnets you provide when you create the cluster.</p>\"\n        }\n      ]\n    },\n    \"ClientSubnets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientSubnets\"\n          },\n          \"description\": \"\\n            <p>The list of subnets to connect to in the client virtual private cloud (VPC). AWS creates elastic network interfaces inside these subnets. Client applications use elastic network interfaces to produce and consume data. Client subnets can't occupy the Availability Zone with ID use use1-az3.</p>\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin5Max32\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceType\"\n          },\n         \
  \ \"description\": \"\\n            <p>The type of Amazon EC2 instances to use for Apache Kafka brokers. The following instance types are allowed: kafka.m5.large, kafka.m5.xlarge, kafka.m5.2xlarge,\\nkafka.m5.4xlarge, kafka.m5.12xlarge, and kafka.m5.24xlarge.</p>\"\n        }\n      ]\n    },\n    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroups\"\n          },\n          \"description\": \"\\n            <p>The AWS security groups to associate with the elastic network interfaces in order to specify who can connect to and communicate with the Amazon MSK cluster. If you don't specify a security group, Amazon MSK uses the default security group associated with the VPC.</p>\"\n        }\n      ]\n    },\n    \"StorageInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageInfo\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"storageInfo\"\n          },\n          \"description\": \"\\n            <p>Contains information about storage volumes attached to MSK broker nodes.</p>\"\n        }\n      ]\n    },\n    \"ConnectivityInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectivityInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"connectivityInfo\"\n          },\n          \"description\": \"\\n            <p>Information about the broker access configuration.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientSubnets\",\n    \"InstanceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-node-group-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BrokerNodeGroupInfo
---
