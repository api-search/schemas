---
description: Details of the Amazon EC2 instance involved in a finding.
layout: schema
name: AwsEc2InstanceDetails
properties_list:
- description: ''
  name: iamInstanceProfileArn
  type: object
- description: ''
  name: imageId
  type: object
- description: ''
  name: ipV4Addresses
  type: object
- description: ''
  name: ipV6Addresses
  type: object
- description: ''
  name: keyName
  type: object
- description: ''
  name: launchedAt
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: subnetId
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: vpcId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-aws-ec2-instance-details-schema.json
slug: inspector-aws-ec2-instance-details
source_filename: inspector-aws-ec2-instance-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-ec2-instance-details-schema.json\",\n  \"title\": \"AwsEc2InstanceDetails\",\n  \"description\": \"Details of the Amazon EC2 instance involved in a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iamInstanceProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The IAM instance profile ARN of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"imageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The image ID of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"ipV4Addresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpV4AddressList\"\
  \n        },\n        {\n          \"description\": \"The IPv4 addresses of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"ipV6Addresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpV6AddressList\"\n        },\n        {\n          \"description\": \"The IPv6 addresses of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"keyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the key pair used to launch the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"launchedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeTimestamp\"\n        },\n        {\n          \"description\": \"The date and time the Amazon EC2 instance was launched at.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\
  \n        },\n        {\n          \"description\": \"The platform of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"subnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The subnet ID of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The type of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"vpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The VPC ID of the Amazon EC2 instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-ec2-instance-details-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AwsEc2InstanceDetails
---
