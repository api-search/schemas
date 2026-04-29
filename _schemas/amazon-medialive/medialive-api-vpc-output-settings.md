---
description: The properties for a private VPC Output When this property is specified, the output egress addresses will be created in a user specified VPC
layout: schema
name: VpcOutputSettings
properties_list:
- description: ''
  name: PublicAddressAllocationIds
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
- description: ''
  name: SubnetIds
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-vpc-output-settings-schema.json
slug: medialive-api-vpc-output-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-vpc-output-settings-schema.json\",\n  \"title\": \"VpcOutputSettings\",\n  \"description\": \"The properties for a private VPC Output\\nWhen this property is specified, the output egress addresses will be created in a user specified VPC\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PublicAddressAllocationIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"publicAddressAllocationIds\"\n          },\n          \"description\": \"List of public address allocation ids to associate with ENIs that will be created in Output VPC.\\nMust specify one for SINGLE_PIPELINE, two for STANDARD channels\\n\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroupIds\"\n          },\n          \"description\": \"A list of up to 5 EC2 VPC security group IDs to attach to the Output VPC network interfaces.\\nIf none are specified then the VPC default security group will be used\\n\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetIds\"\n          },\n          \"description\": \"A list of VPC subnet IDs from the same VPC.\\nIf STANDARD channel, subnet IDs must be mapped to two unique availability zones (AZ).\\n\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SubnetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-vpc-output-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VpcOutputSettings
---
