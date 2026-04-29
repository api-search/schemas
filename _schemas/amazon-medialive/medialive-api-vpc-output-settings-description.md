---
description: The properties for a private VPC Output
layout: schema
name: VpcOutputSettingsDescription
properties_list:
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: NetworkInterfaceIds
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
- description: ''
  name: SubnetIds
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-vpc-output-settings-description-schema.json
slug: medialive-api-vpc-output-settings-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-vpc-output-settings-description-schema.json\",\n  \"title\": \"VpcOutputSettingsDescription\",\n  \"description\": \"The properties for a private VPC Output\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZones\"\n          },\n          \"description\": \"The Availability Zones where the vpc subnets are located.\\nThe first Availability Zone applies to the first subnet in the list of subnets.\\nThe second Availability Zone applies to the second subnet.\\n\"\n        }\n      ]\n    },\n    \"NetworkInterfaceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"networkInterfaceIds\"\n          },\n          \"description\": \"A list of Elastic Network Interfaces created by MediaLive in the customer's VPC\\n\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroupIds\"\n          },\n          \"description\": \"A list of up EC2 VPC security group IDs attached to the Output VPC network interfaces.\\n\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetIds\"\n          },\n          \"description\": \"A list of VPC subnet IDs from the same VPC.\\nIf STANDARD channel, subnet IDs must be mapped to two unique availability zones (AZ).\\\
  n\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-vpc-output-settings-description-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VpcOutputSettingsDescription
---
