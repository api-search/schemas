---
description: Schema representing an Amazon Transit Gateway resource.
layout: schema
name: Amazon Transit Gateway
properties_list:
- description: The ID of the transit gateway.
  name: TransitGatewayId
  type: string
- description: The Amazon Resource Name (ARN) of the transit gateway.
  name: TransitGatewayArn
  type: string
- description: The state of the transit gateway.
  name: State
  type: string
- description: The ID of the AWS account that owns the transit gateway.
  name: OwnerId
  type: string
- description: The description of the transit gateway.
  name: Description
  type: string
- description: The transit gateway options.
  name: Options
  type: object
- description: The creation date and time of the transit gateway.
  name: CreationTime
  type: string
- description: The tags assigned to the transit gateway.
  name: Tags
  type: array
provider_name: Amazon Transit Gateway
provider_slug: amazon-transit-gateway
schema_file: json-schema/amazon-transit-gateway-schema.json
slug: amazon-transit-gateway
source_filename: amazon-transit-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://ec2.amazonaws.com/schemas/transit-gateway\",\n  \"title\": \"Amazon Transit Gateway\",\n  \"description\": \"Schema representing an Amazon Transit Gateway resource.\",\n  \"type\": \"object\",\n  \"required\": [],\n  \"properties\": {\n    \"TransitGatewayId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the transit gateway.\",\n      \"pattern\": \"^tgw-[a-f0-9]+$\"\n    },\n    \"TransitGatewayArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the transit gateway.\",\n      \"pattern\": \"^arn:aws:ec2:.+:.+:transit-gateway/.+\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the transit gateway.\",\n      \"enum\": [\n        \"pending\",\n        \"available\",\n        \"modifying\",\n        \"deleting\",\n        \"deleted\"\n      ]\n    },\n    \"OwnerId\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"The ID of the AWS account that owns the transit gateway.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the transit gateway.\"\n    },\n    \"Options\": {\n      \"type\": \"object\",\n      \"description\": \"The transit gateway options.\",\n      \"properties\": {\n        \"AmazonSideAsn\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"A private Autonomous System Number (ASN) for the Amazon side of a BGP session.\"\n        },\n        \"AutoAcceptSharedAttachments\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether attachment requests are automatically accepted.\",\n          \"enum\": [\n            \"enable\",\n            \"disable\"\n          ]\n        },\n        \"DefaultRouteTableAssociation\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether\
  \ resource attachments are automatically associated with the default route table.\",\n          \"enum\": [\n            \"enable\",\n            \"disable\"\n          ]\n        },\n        \"DefaultRouteTablePropagation\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether resource attachments automatically propagate routes to the default route table.\",\n          \"enum\": [\n            \"enable\",\n            \"disable\"\n          ]\n        },\n        \"DnsSupport\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether DNS support is enabled.\",\n          \"enum\": [\n            \"enable\",\n            \"disable\"\n          ]\n        },\n        \"VpnEcmpSupport\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether Equal Cost Multipath Protocol support is enabled.\",\n          \"enum\": [\n            \"enable\",\n            \"disable\"\n          ]\n        },\n        \"AssociationDefaultRouteTableId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The ID of the default association route table.\"\n        },\n        \"PropagationDefaultRouteTableId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the default propagation route table.\"\n        }\n      }\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation date and time of the transit gateway.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"The tags assigned to the transit gateway.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair for tagging resources.\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n        \
  \  \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-transit-gateway/refs/heads/main/json-schema/amazon-transit-gateway-schema.json
tags:
- AWS
- Cloud Networking
- Network Hub
- Networking
- Transit Gateway
- VPC
title: Amazon Transit Gateway
---
