---
description: Describes an EC2 instance
layout: schema
name: Instance
properties_list:
- description: The ID of the instance
  name: instanceId
  type: string
- description: The ID of the AMI used to launch the instance
  name: imageId
  type: string
- description: The instance type
  name: instanceType
  type: string
- description: The name of the key pair
  name: keyName
  type: string
- description: The time the instance was launched
  name: launchTime
  type: string
- description: The location where the instance launched
  name: placement
  type: object
- description: The monitoring for the instance
  name: monitoring
  type: object
- description: The current state of the instance
  name: instanceState
  type: object
- description: The ID of the subnet in which the instance is running
  name: subnetId
  type: string
- description: The ID of the VPC in which the instance is running
  name: vpcId
  type: string
- description: The private IPv4 address assigned to the instance
  name: privateIpAddress
  type: string
- description: The public IPv4 address assigned to the instance
  name: publicIpAddress
  type: string
- description: The architecture of the image
  name: architecture
  type: string
- description: The root device type used by the AMI
  name: rootDeviceType
  type: string
- description: Any tags assigned to the instance
  name: tags
  type: array
- description: The security groups for the instance
  name: securityGroups
  type: array
provider_name: Amazon EC2
provider_slug: amazon-ec2
schema_file: json-schema/ec2-openapi-instance-schema.json
slug: ec2-openapi-instance
source_filename: ec2-openapi-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-instance-schema.json\",\n  \"title\": \"Instance\",\n  \"description\": \"Describes an EC2 instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the instance\"\n    },\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AMI used to launch the instance\"\n    },\n    \"instanceType\": {\n      \"type\": \"string\",\n      \"description\": \"The instance type\"\n    },\n    \"keyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the key pair\"\n    },\n    \"launchTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the instance was launched\"\n    },\n    \"placement\": {\n      \"type\": \"\
  object\",\n      \"description\": \"The location where the instance launched\",\n      \"properties\": {\n        \"availabilityZone\": {\n          \"type\": \"string\",\n          \"description\": \"The Availability Zone of the instance\"\n        }\n      }\n    },\n    \"monitoring\": {\n      \"type\": \"object\",\n      \"description\": \"The monitoring for the instance\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The monitoring state\",\n          \"enum\": [\n            \"disabled\",\n            \"disabling\",\n            \"enabled\",\n            \"pending\"\n          ]\n        }\n      }\n    },\n    \"instanceState\": {\n      \"type\": \"object\",\n      \"description\": \"The current state of the instance\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"integer\",\n          \"description\": \"The state code (0=pending, 16=running, 32=shutting-down, 48=terminated, 64=stopping, 80=stopped)\"\
  \n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The current state of the instance\",\n          \"enum\": [\n            \"pending\",\n            \"running\",\n            \"shutting-down\",\n            \"terminated\",\n            \"stopping\",\n            \"stopped\"\n          ]\n        }\n      }\n    },\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the subnet in which the instance is running\"\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC in which the instance is running\"\n    },\n    \"privateIpAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The private IPv4 address assigned to the instance\"\n    },\n    \"publicIpAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The public IPv4 address assigned to the instance\"\n    },\n    \"architecture\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The architecture of the image\",\n      \"enum\": [\n        \"i386\",\n        \"x86_64\",\n        \"arm64\"\n      ]\n    },\n    \"rootDeviceType\": {\n      \"type\": \"string\",\n      \"description\": \"The root device type used by the AMI\",\n      \"enum\": [\n        \"ebs\",\n        \"instance-store\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Any tags assigned to the instance\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    },\n    \"securityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"The security groups for the instance\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"groupId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the security group\"\n          },\n          \"groupName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the security group\"\n    \
  \      }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-instance-schema.json
tags:
- AWS
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
title: Instance
---
