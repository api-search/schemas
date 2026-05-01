---
description: <p>BrokerNodeInfo</p>
layout: schema
name: BrokerNodeInfo
properties_list:
- description: ''
  name: AttachedENIId
  type: object
- description: ''
  name: BrokerId
  type: object
- description: ''
  name: ClientSubnet
  type: object
- description: ''
  name: ClientVpcIpAddress
  type: object
- description: ''
  name: CurrentBrokerSoftwareInfo
  type: object
- description: ''
  name: Endpoints
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-broker-node-info-schema.json
slug: msk-api-broker-node-info
source_filename: msk-api-broker-node-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-node-info-schema.json\",\n  \"title\": \"BrokerNodeInfo\",\n  \"description\": \"\\n            <p>BrokerNodeInfo</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttachedENIId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attachedENIId\"\n          },\n          \"description\": \"\\n            <p>The attached elastic network interface of the broker.</p>\"\n        }\n      ]\n    },\n    \"BrokerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerId\"\n          },\n          \"description\": \"\\n            <p>The ID of the broker.</p>\"\n        }\n\
  \      ]\n    },\n    \"ClientSubnet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientSubnet\"\n          },\n          \"description\": \"\\n            <p>The client subnet to which this broker node belongs.</p>\"\n        }\n      ]\n    },\n    \"ClientVpcIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientVpcIpAddress\"\n          },\n          \"description\": \"\\n            <p>The virtual private cloud (VPC) of the client.</p>\"\n        }\n      ]\n    },\n    \"CurrentBrokerSoftwareInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerSoftwareInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentBrokerSoftwareInfo\"\n          },\n          \"description\": \"\\n       \
  \     <p>Information about the version of software currently deployed on the Apache Kafka brokers in the cluster.</p>\"\n        }\n      ]\n    },\n    \"Endpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"endpoints\"\n          },\n          \"description\": \"\\n            <p>Endpoints for accessing the broker.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-node-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BrokerNodeInfo
---
