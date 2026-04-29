---
description: Represents an Amazon Virtual Private Cloud (VPC) with its associated configuration, networking, and metadata.
layout: schema
name: Amazon VPC
properties_list:
- description: The unique identifier for the VPC
  name: vpcId
  type: string
- description: The primary IPv4 CIDR block for the VPC
  name: cidrBlock
  type: string
- description: The current state of the VPC
  name: state
  type: string
- description: The ID of the set of DHCP options associated with the VPC
  name: dhcpOptionsId
  type: string
- description: The allowed tenancy of instances launched into the VPC
  name: instanceTenancy
  type: string
- description: Indicates whether the VPC is the default VPC
  name: isDefault
  type: boolean
- description: The ID of the AWS account that owns the VPC
  name: ownerId
  type: string
- description: Information about the IPv4 CIDR blocks associated with the VPC
  name: cidrBlockAssociationSet
  type: array
- description: Information about the IPv6 CIDR blocks associated with the VPC
  name: ipv6CidrBlockAssociationSet
  type: array
- description: The subnets within the VPC
  name: subnets
  type: array
- description: Internet gateways attached to the VPC
  name: internetGateways
  type: array
- description: NAT gateways in the VPC
  name: natGateways
  type: array
- description: Route tables associated with the VPC
  name: routeTables
  type: array
- description: Network ACLs associated with the VPC
  name: networkAcls
  type: array
- description: Tags assigned to the VPC
  name: tags
  type: array
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-schema.json
slug: amazon-vpc
source_filename: amazon-vpc-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/vpc/vpc.json\",\n  \"title\": \"Amazon VPC\",\n  \"description\": \"Represents an Amazon Virtual Private Cloud (VPC) with its associated configuration, networking, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"vpcId\", \"cidrBlock\", \"state\"],\n  \"properties\": {\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the VPC\",\n      \"pattern\": \"^vpc-[a-f0-9]{8,17}$\"\n    },\n    \"cidrBlock\": {\n      \"type\": \"string\",\n      \"description\": \"The primary IPv4 CIDR block for the VPC\",\n      \"pattern\": \"^([0-9]{1,3}\\\\.){3}[0-9]{1,3}/[0-9]{1,2}$\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the VPC\",\n      \"enum\": [\"pending\", \"available\"]\n    },\n    \"dhcpOptionsId\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The ID of the set of DHCP options associated with the VPC\",\n      \"pattern\": \"^dopt-[a-f0-9]{8,17}$\"\n    },\n    \"instanceTenancy\": {\n      \"type\": \"string\",\n      \"description\": \"The allowed tenancy of instances launched into the VPC\",\n      \"enum\": [\"default\", \"dedicated\", \"host\"]\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the VPC is the default VPC\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AWS account that owns the VPC\"\n    },\n    \"cidrBlockAssociationSet\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the IPv4 CIDR blocks associated with the VPC\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CidrBlockAssociation\"\n      }\n    },\n    \"ipv6CidrBlockAssociationSet\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the IPv6 CIDR blocks associated with the VPC\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/Ipv6CidrBlockAssociation\"\n      }\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"description\": \"The subnets within the VPC\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Subnet\"\n      }\n    },\n    \"internetGateways\": {\n      \"type\": \"array\",\n      \"description\": \"Internet gateways attached to the VPC\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InternetGateway\"\n      }\n    },\n    \"natGateways\": {\n      \"type\": \"array\",\n      \"description\": \"NAT gateways in the VPC\",\n      \"items\": {\n        \"$ref\": \"#/$defs/NatGateway\"\n      }\n    },\n    \"routeTables\": {\n      \"type\": \"array\",\n      \"description\": \"Route tables associated with the VPC\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RouteTable\"\n      }\n    },\n    \"networkAcls\": {\n      \"type\": \"array\",\n      \"description\": \"Network ACLs associated with the VPC\",\n      \"items\": {\n\
  \        \"$ref\": \"#/$defs/NetworkAcl\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the VPC\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"CidrBlockAssociation\": {\n      \"type\": \"object\",\n      \"description\": \"Describes an IPv4 CIDR block associated with a VPC\",\n      \"properties\": {\n        \"associationId\": {\n          \"type\": \"string\",\n          \"description\": \"The association ID for the IPv4 CIDR block\"\n        },\n        \"cidrBlock\": {\n          \"type\": \"string\",\n          \"description\": \"The IPv4 CIDR block\"\n        },\n        \"cidrBlockState\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"state\": {\n              \"type\": \"string\",\n              \"enum\": [\"associating\", \"associated\", \"disassociating\", \"disassociated\", \"failing\", \"failed\"]\n            }\n          }\n\
  \        }\n      }\n    },\n    \"Ipv6CidrBlockAssociation\": {\n      \"type\": \"object\",\n      \"description\": \"Describes an IPv6 CIDR block associated with a VPC\",\n      \"properties\": {\n        \"associationId\": {\n          \"type\": \"string\",\n          \"description\": \"The association ID for the IPv6 CIDR block\"\n        },\n        \"ipv6CidrBlock\": {\n          \"type\": \"string\",\n          \"description\": \"The IPv6 CIDR block\"\n        },\n        \"ipv6CidrBlockState\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"state\": {\n              \"type\": \"string\",\n              \"enum\": [\"associating\", \"associated\", \"disassociating\", \"disassociated\", \"failing\", \"failed\"]\n            }\n          }\n        }\n      }\n    },\n    \"Subnet\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a subnet within a VPC\",\n      \"properties\": {\n        \"subnetId\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The ID of the subnet\",\n          \"pattern\": \"^subnet-[a-f0-9]{8,17}$\"\n        },\n        \"subnetArn\": {\n          \"type\": \"string\",\n          \"description\": \"The Amazon Resource Name (ARN) of the subnet\"\n        },\n        \"vpcId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the VPC the subnet is in\"\n        },\n        \"cidrBlock\": {\n          \"type\": \"string\",\n          \"description\": \"The IPv4 CIDR block assigned to the subnet\"\n        },\n        \"availabilityZone\": {\n          \"type\": \"string\",\n          \"description\": \"The Availability Zone of the subnet\"\n        },\n        \"availabilityZoneId\": {\n          \"type\": \"string\",\n          \"description\": \"The AZ ID of the subnet\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The current state of the subnet\",\n          \"enum\": [\"pending\", \"available\"]\n\
  \        },\n        \"availableIpAddressCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of unused private IPv4 addresses in the subnet\"\n        },\n        \"defaultForAz\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether this is the default subnet for the AZ\"\n        },\n        \"mapPublicIpOnLaunch\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether instances get a public IPv4 address on launch\"\n        }\n      },\n      \"required\": [\"subnetId\", \"vpcId\", \"cidrBlock\"]\n    },\n    \"InternetGateway\": {\n      \"type\": \"object\",\n      \"description\": \"Describes an internet gateway\",\n      \"properties\": {\n        \"internetGatewayId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the internet gateway\",\n          \"pattern\": \"^igw-[a-f0-9]{8,17}$\"\n        },\n        \"attachments\": {\n          \"type\": \"array\"\
  ,\n          \"description\": \"Any VPCs attached to the internet gateway\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"state\": {\n                \"type\": \"string\",\n                \"enum\": [\"attaching\", \"attached\", \"detaching\", \"detached\"]\n              },\n              \"vpcId\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"ownerId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the AWS account that owns the internet gateway\"\n        }\n      },\n      \"required\": [\"internetGatewayId\"]\n    },\n    \"NatGateway\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a NAT gateway\",\n      \"properties\": {\n        \"natGatewayId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the NAT gateway\",\n          \"pattern\": \"^nat-[a-f0-9]{8,17}$\"\n        },\n     \
  \   \"subnetId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the subnet in which the NAT gateway is located\"\n        },\n        \"vpcId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the VPC in which the NAT gateway is located\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The state of the NAT gateway\",\n          \"enum\": [\"pending\", \"failed\", \"available\", \"deleting\", \"deleted\"]\n        },\n        \"connectivityType\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether the NAT gateway supports public or private connectivity\",\n          \"enum\": [\"public\", \"private\"]\n        },\n        \"createTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the NAT gateway was created\"\n        }\n      },\n      \"required\": [\"natGatewayId\", \"subnetId\"\
  ]\n    },\n    \"RouteTable\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a route table\",\n      \"properties\": {\n        \"routeTableId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the route table\",\n          \"pattern\": \"^rtb-[a-f0-9]{8,17}$\"\n        },\n        \"vpcId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the VPC\"\n        },\n        \"routes\": {\n          \"type\": \"array\",\n          \"description\": \"The routes in the route table\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"destinationCidrBlock\": {\n                \"type\": \"string\"\n              },\n              \"gatewayId\": {\n                \"type\": \"string\"\n              },\n              \"natGatewayId\": {\n                \"type\": \"string\"\n              },\n              \"state\": {\n                \"type\": \"string\",\n      \
  \          \"enum\": [\"active\", \"blackhole\"]\n              },\n              \"origin\": {\n                \"type\": \"string\",\n                \"enum\": [\"CreateRouteTable\", \"CreateRoute\", \"EnableVgwRoutePropagation\"]\n              }\n            }\n          }\n        },\n        \"associations\": {\n          \"type\": \"array\",\n          \"description\": \"The associations between the route table and subnets\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"routeTableAssociationId\": {\n                \"type\": \"string\"\n              },\n              \"subnetId\": {\n                \"type\": \"string\"\n              },\n              \"main\": {\n                \"type\": \"boolean\"\n              }\n            }\n          }\n        }\n      },\n      \"required\": [\"routeTableId\", \"vpcId\"]\n    },\n    \"NetworkAcl\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a network\
  \ ACL\",\n      \"properties\": {\n        \"networkAclId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the network ACL\",\n          \"pattern\": \"^acl-[a-f0-9]{8,17}$\"\n        },\n        \"vpcId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the VPC for the network ACL\"\n        },\n        \"isDefault\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether this is the default network ACL for the VPC\"\n        },\n        \"entries\": {\n          \"type\": \"array\",\n          \"description\": \"The entries (rules) in the network ACL\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"ruleNumber\": {\n                \"type\": \"integer\",\n                \"description\": \"The rule number for the entry\"\n              },\n              \"protocol\": {\n                \"type\": \"string\",\n                \"description\":\
  \ \"The protocol number (-1 means all)\"\n              },\n              \"ruleAction\": {\n                \"type\": \"string\",\n                \"enum\": [\"allow\", \"deny\"]\n              },\n              \"egress\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether this is an egress rule\"\n              },\n              \"cidrBlock\": {\n                \"type\": \"string\",\n                \"description\": \"The IPv4 CIDR range\"\n              }\n            }\n          }\n        }\n      },\n      \"required\": [\"networkAclId\", \"vpcId\"]\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a resource tag\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the tag\",\n          \"maxLength\": 128\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the tag\",\n\
  \          \"maxLength\": 256\n        }\n      },\n      \"required\": [\"key\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-schema.json
tags:
- AWS
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: Amazon VPC
---
