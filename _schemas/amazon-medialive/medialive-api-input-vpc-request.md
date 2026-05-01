---
description: Settings for a private VPC Input. When this property is specified, the input destination addresses will be created in a VPC rather than with public Internet addresses. This property requires setting the roleArn property on Input creation. Not compatible with the inputSecurityGroups property.
layout: schema
name: InputVpcRequest
properties_list:
- description: ''
  name: SecurityGroupIds
  type: object
- description: ''
  name: SubnetIds
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-vpc-request-schema.json
slug: medialive-api-input-vpc-request
source_filename: medialive-api-input-vpc-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-vpc-request-schema.json\",\n  \"title\": \"InputVpcRequest\",\n  \"description\": \"Settings for a private VPC Input.\\nWhen this property is specified, the input destination addresses will be created in a VPC rather than with public Internet addresses.\\nThis property requires setting the roleArn property on Input creation.\\nNot compatible with the inputSecurityGroups property.\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroupIds\"\n          },\n          \"description\": \"A list of up to 5 EC2 VPC security group IDs to attach to the Input VPC network interfaces.\\nRequires\
  \ subnetIds. If none are specified then the VPC default security group will be used.\\n\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetIds\"\n          },\n          \"description\": \"A list of 2 VPC subnet IDs from the same VPC.\\nSubnet IDs must be mapped to two unique availability zones (AZ).\\n\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SubnetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-vpc-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputVpcRequest
---
