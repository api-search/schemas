---
description: A summary of configuration properties for a node.
layout: schema
name: NodeSummary
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: Arn
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-node-summary-schema.json
slug: amazon-managed-blockchain-node-summary
source_filename: amazon-managed-blockchain-node-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-summary-schema.json\",\n  \"title\": \"NodeSummary\",\n  \"description\": \"A summary of configuration properties for a node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the node.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeStatus\"\n        },\n        {\n          \"description\": \"The status of the node.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\"\
  : \"The date and time that the node was created.\"\n        }\n      ]\n    },\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityZoneString\"\n        },\n        {\n          \"description\": \"The Availability Zone in which the node exists.\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceTypeString\"\n        },\n        {\n          \"description\": \"The EC2 instance type for the node.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the node. For more information about ARNs and their format, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-node-summary-schema.json
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: NodeSummary
---
