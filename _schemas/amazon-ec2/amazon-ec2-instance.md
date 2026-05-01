---
description: Represents an Amazon EC2 virtual server instance with its associated configuration, state, and metadata.
layout: schema
name: Amazon EC2 Instance
properties_list:
- description: The unique identifier for the instance
  name: instanceId
  type: string
- description: The ID of the AMI used to launch the instance
  name: imageId
  type: string
- description: The instance type (e.g., t2.micro, m5.large, c5.xlarge)
  name: instanceType
  type: string
- description: The name of the key pair used for SSH access
  name: keyName
  type: string
- description: The time the instance was launched
  name: launchTime
  type: string
- description: ''
  name: instanceState
  type: object
- description: ''
  name: placement
  type: object
- description: The ID of the subnet the instance is running in
  name: subnetId
  type: string
- description: The ID of the VPC the instance is running in
  name: vpcId
  type: string
- description: The private IPv4 address assigned to the instance
  name: privateIpAddress
  type: string
- description: The public IPv4 address assigned to the instance
  name: publicIpAddress
  type: string
- description: The architecture of the instance
  name: architecture
  type: string
- description: The root device type used by the AMI
  name: rootDeviceType
  type: string
- description: The device name of the root device volume
  name: rootDeviceName
  type: string
- description: Block device mappings for the instance
  name: blockDeviceMappings
  type: array
- description: The security groups associated with the instance
  name: securityGroups
  type: array
- description: Tags assigned to the instance
  name: tags
  type: array
- description: The monitoring state of the instance
  name: monitoring
  type: object
- description: The platform of the instance (Windows or empty for Linux)
  name: platform
  type: string
- description: Indicates whether the instance is optimized for Amazon EBS I/O
  name: ebsOptimized
  type: boolean
- description: Specifies whether enhanced networking with ENA is enabled
  name: enaSupport
  type: boolean
provider_name: Amazon EC2
provider_slug: amazon-ec2
schema_file: json-schema/amazon-ec2-instance-schema.json
slug: amazon-ec2-instance
source_filename: amazon-ec2-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/ec2/instance.json\",\n  \"title\": \"Amazon EC2 Instance\",\n  \"description\": \"Represents an Amazon EC2 virtual server instance with its associated configuration, state, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"instanceId\", \"instanceType\", \"imageId\", \"instanceState\"],\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the instance\",\n      \"pattern\": \"^i-[a-f0-9]{8,17}$\"\n    },\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AMI used to launch the instance\",\n      \"pattern\": \"^ami-[a-f0-9]{8,17}$\"\n    },\n    \"instanceType\": {\n      \"type\": \"string\",\n      \"description\": \"The instance type (e.g., t2.micro, m5.large, c5.xlarge)\"\n    },\n    \"keyName\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The name of the key pair used for SSH access\"\n    },\n    \"launchTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the instance was launched\"\n    },\n    \"instanceState\": {\n      \"$ref\": \"#/$defs/InstanceState\"\n    },\n    \"placement\": {\n      \"$ref\": \"#/$defs/Placement\"\n    },\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the subnet the instance is running in\",\n      \"pattern\": \"^subnet-[a-f0-9]{8,17}$\"\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC the instance is running in\",\n      \"pattern\": \"^vpc-[a-f0-9]{8,17}$\"\n    },\n    \"privateIpAddress\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"The private IPv4 address assigned to the instance\"\n    },\n    \"publicIpAddress\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n\
  \      \"description\": \"The public IPv4 address assigned to the instance\"\n    },\n    \"architecture\": {\n      \"type\": \"string\",\n      \"description\": \"The architecture of the instance\",\n      \"enum\": [\"i386\", \"x86_64\", \"arm64\"]\n    },\n    \"rootDeviceType\": {\n      \"type\": \"string\",\n      \"description\": \"The root device type used by the AMI\",\n      \"enum\": [\"ebs\", \"instance-store\"]\n    },\n    \"rootDeviceName\": {\n      \"type\": \"string\",\n      \"description\": \"The device name of the root device volume\"\n    },\n    \"blockDeviceMappings\": {\n      \"type\": \"array\",\n      \"description\": \"Block device mappings for the instance\",\n      \"items\": {\n        \"$ref\": \"#/$defs/BlockDeviceMapping\"\n      }\n    },\n    \"securityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"The security groups associated with the instance\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SecurityGroupIdentifier\"\n    \
  \  }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the instance\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    },\n    \"monitoring\": {\n      \"type\": \"object\",\n      \"description\": \"The monitoring state of the instance\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether detailed monitoring is enabled\",\n          \"enum\": [\"disabled\", \"disabling\", \"enabled\", \"pending\"]\n        }\n      }\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform of the instance (Windows or empty for Linux)\"\n    },\n    \"ebsOptimized\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the instance is optimized for Amazon EBS I/O\"\n    },\n    \"enaSupport\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether enhanced networking with ENA is\
  \ enabled\"\n    }\n  },\n  \"$defs\": {\n    \"InstanceState\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the current state of the instance\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"integer\",\n          \"description\": \"The state code (0=pending, 16=running, 32=shutting-down, 48=terminated, 64=stopping, 80=stopped)\",\n          \"enum\": [0, 16, 32, 48, 64, 80]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The current state of the instance\",\n          \"enum\": [\"pending\", \"running\", \"shutting-down\", \"terminated\", \"stopping\", \"stopped\"]\n        }\n      }\n    },\n    \"Placement\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the placement of an instance\",\n      \"properties\": {\n        \"availabilityZone\": {\n          \"type\": \"string\",\n          \"description\": \"The Availability Zone of the instance\"\n        },\n        \"groupName\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The name of the placement group\"\n        },\n        \"tenancy\": {\n          \"type\": \"string\",\n          \"description\": \"The tenancy of the instance\",\n          \"enum\": [\"default\", \"dedicated\", \"host\"]\n        }\n      }\n    },\n    \"BlockDeviceMapping\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a block device mapping\",\n      \"properties\": {\n        \"deviceName\": {\n          \"type\": \"string\",\n          \"description\": \"The device name (e.g., /dev/sdh or xvdh)\"\n        },\n        \"ebs\": {\n          \"type\": \"object\",\n          \"description\": \"Parameters used to set up EBS volumes\",\n          \"properties\": {\n            \"volumeId\": {\n              \"type\": \"string\",\n              \"description\": \"The ID of the EBS volume\"\n            },\n            \"status\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"The attachment state\",\n              \"enum\": [\"attaching\", \"attached\", \"detaching\", \"detached\"]\n            },\n            \"deleteOnTermination\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the volume is deleted on instance termination\"\n            }\n          }\n        }\n      }\n    },\n    \"SecurityGroupIdentifier\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a security group\",\n      \"properties\": {\n        \"groupId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the security group\",\n          \"pattern\": \"^sg-[a-f0-9]{8,17}$\"\n        },\n        \"groupName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the security group\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a resource tag\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The key of the tag\",\n          \"maxLength\": 128\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the tag\",\n          \"maxLength\": 256\n        }\n      },\n      \"required\": [\"key\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/amazon-ec2-instance-schema.json
tags:
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
title: Amazon EC2 Instance
---
