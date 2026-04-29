---
description: Describes a gateway object.
layout: schema
name: GatewayInfo
properties_list:
- description: ''
  name: GatewayId
  type: object
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: GatewayType
  type: object
- description: ''
  name: GatewayOperationalState
  type: object
- description: ''
  name: GatewayName
  type: object
- description: ''
  name: Ec2InstanceId
  type: object
- description: ''
  name: Ec2InstanceRegion
  type: object
- description: ''
  name: HostEnvironment
  type: object
- description: ''
  name: HostEnvironmentId
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-gateway-info-schema.json
slug: amazon-storage-gateway-gateway-info
source_filename: amazon-storage-gateway-gateway-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-gateway-info-schema.json\",\n  \"title\": \"GatewayInfo\",\n  \"description\": \"Describes a gateway object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayId\"\n        },\n        {\n          \"description\": \"The unique identifier assigned to your gateway during activation. This ID becomes part of the gateway Amazon Resource Name (ARN), which you use as input for other operations.\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the gateway. Use the <a>ListGateways</a> operation to return\
  \ a list of gateways for your account and Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"GatewayType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayType\"\n        },\n        {\n          \"description\": \"The type of the gateway.\"\n        }\n      ]\n    },\n    \"GatewayOperationalState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayOperationalState\"\n        },\n        {\n          \"description\": \"<p>The state of the gateway.</p> <p>Valid Values: <code>DISABLED</code> | <code>ACTIVE</code> </p>\"\n        }\n      ]\n    },\n    \"GatewayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The name of the gateway.\"\n        }\n      ]\n    },\n    \"Ec2InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2InstanceId\"\n        },\n        {\n  \
  \        \"description\": \"The ID of the Amazon EC2 instance that was used to launch the gateway.\"\n        }\n      ]\n    },\n    \"Ec2InstanceRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2InstanceRegion\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the Amazon EC2 instance is located.\"\n        }\n      ]\n    },\n    \"HostEnvironment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HostEnvironment\"\n        },\n        {\n          \"description\": \"The type of hardware or software platform on which the gateway is running.\"\n        }\n      ]\n    },\n    \"HostEnvironmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HostEnvironmentId\"\n        },\n        {\n          \"description\": \"A unique identifier for the specific instance of the host platform running the gateway. This value is only available for certain host\
  \ environments, and its format depends on the host environment type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-gateway-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: GatewayInfo
---
