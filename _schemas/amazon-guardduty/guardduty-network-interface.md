---
description: Contains information about the elastic network interface of the EC2 instance.
layout: schema
name: NetworkInterface
properties_list:
- description: ''
  name: Ipv6Addresses
  type: object
- description: ''
  name: NetworkInterfaceId
  type: object
- description: ''
  name: PrivateDnsName
  type: object
- description: ''
  name: PrivateIpAddress
  type: object
- description: ''
  name: PrivateIpAddresses
  type: object
- description: ''
  name: PublicDnsName
  type: object
- description: ''
  name: PublicIp
  type: object
- description: ''
  name: SecurityGroups
  type: object
- description: ''
  name: SubnetId
  type: object
- description: ''
  name: VpcId
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-network-interface-schema.json
slug: guardduty-network-interface
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-network-interface-schema.json\",\n  \"title\": \"NetworkInterface\",\n  \"description\": \"Contains information about the elastic network interface of the EC2 instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Ipv6Addresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ipv6Addresses\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipv6Addresses\"\n          },\n          \"description\": \"A list of IPv6 addresses for the EC2 instance.\"\n        }\n      ]\n    },\n    \"NetworkInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkInterfaceId\"\n          },\n          \"description\": \"The ID of\
  \ the network interface.\"\n        }\n      ]\n    },\n    \"PrivateDnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privateDnsName\"\n          },\n          \"description\": \"The private DNS name of the EC2 instance.\"\n        }\n      ]\n    },\n    \"PrivateIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privateIpAddress\"\n          },\n          \"description\": \"The private IP address of the EC2 instance.\"\n        }\n      ]\n    },\n    \"PrivateIpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrivateIpAddresses\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privateIpAddresses\"\n          },\n          \"description\": \"Other private IP address information of the EC2 instance.\"\
  \n        }\n      ]\n    },\n    \"PublicDnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"publicDnsName\"\n          },\n          \"description\": \"The public DNS name of the EC2 instance.\"\n        }\n      ]\n    },\n    \"PublicIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"publicIp\"\n          },\n          \"description\": \"The public IP address of the EC2 instance.\"\n        }\n      ]\n    },\n    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroups\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroups\"\n          },\n          \"description\": \"The security groups associated with the EC2 instance.\"\n        }\n      ]\n    },\n    \"SubnetId\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetId\"\n          },\n          \"description\": \"The subnet ID of the EC2 instance.\"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcId\"\n          },\n          \"description\": \"The VPC ID of the EC2 instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-network-interface-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: NetworkInterface
---
