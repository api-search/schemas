---
description: The configuration information for a virtual private cloud (VPC) destination.
layout: schema
name: VpcDestinationConfiguration
properties_list:
- description: ''
  name: subnetIds
  type: object
- description: ''
  name: securityGroups
  type: object
- description: ''
  name: vpcId
  type: object
- description: ''
  name: roleArn
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-vpc-destination-configuration-schema.json
slug: iot-device-management-vpc-destination-configuration
source_filename: iot-device-management-vpc-destination-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-vpc-destination-configuration-schema.json\",\n  \"title\": \"VpcDestinationConfiguration\",\n  \"description\": \"The configuration information for a virtual private cloud (VPC) destination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIdList\"\n        },\n        {\n          \"description\": \"The subnet IDs of the VPC destination.\"\n        }\n      ]\n    },\n    \"securityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupList\"\n        },\n        {\n          \"description\": \"The security groups of the VPC destination.\"\n        }\n      ]\n    },\n    \"vpcId\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The ID of the VPC.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsArn\"\n        },\n        {\n          \"description\": \"The ARN of a role that has permission to create and attach to elastic network interfaces (ENIs).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"subnetIds\",\n    \"vpcId\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-vpc-destination-configuration-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: VpcDestinationConfiguration
---
