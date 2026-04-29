---
description: Represents an Amazon Virtual Private Cloud (VPC) endpoint configuration.
layout: schema
name: VPCEConfiguration
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: vpceConfigurationName
  type: object
- description: ''
  name: vpceServiceName
  type: object
- description: ''
  name: serviceDnsName
  type: object
- description: ''
  name: vpceConfigurationDescription
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-vpce-configuration-schema.json
slug: amazon-device-farm-vpce-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-vpce-configuration-schema.json\",\n  \"title\": \"VPCEConfiguration\",\n  \"description\": \"Represents an Amazon Virtual Private Cloud (VPC) endpoint configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the VPC endpoint configuration.\"\n        }\n      ]\n    },\n    \"vpceConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCEConfigurationName\"\n        },\n        {\n          \"description\": \"The friendly name you give to your VPC endpoint configuration to manage your configurations more easily.\"\n        }\n      ]\n\
  \    },\n    \"vpceServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCEServiceName\"\n        },\n        {\n          \"description\": \"The name of the VPC endpoint service running in your AWS account that you want Device Farm to test.\"\n        }\n      ]\n    },\n    \"serviceDnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceDnsName\"\n        },\n        {\n          \"description\": \"The DNS name that maps to the private IP address of the service you want to access.\"\n        }\n      ]\n    },\n    \"vpceConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCEConfigurationDescription\"\n        },\n        {\n          \"description\": \"An optional description that provides details about your VPC endpoint configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-vpce-configuration-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: VPCEConfiguration
---
