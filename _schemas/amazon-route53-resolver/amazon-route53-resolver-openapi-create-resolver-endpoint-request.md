---
description: CreateResolverEndpointRequest schema from openapi
layout: schema
name: CreateResolverEndpointRequest
properties_list:
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
- description: ''
  name: Direction
  type: object
- description: ''
  name: IpAddresses
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ResolverEndpointType
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-create-resolver-endpoint-request-schema.json
slug: amazon-route53-resolver-openapi-create-resolver-endpoint-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-resolver-endpoint-request-schema.json\",\n  \"title\": \"CreateResolverEndpointRequest\",\n  \"description\": \"CreateResolverEndpointRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that identifies the request and that allows failed requests to be retried without the risk of running the operation twice. <code>CreatorRequestId</code> can be any unique string, for example, a date/time stamp. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n\
  \          \"description\": \"A friendly name that lets you easily find a configuration in the Resolver dashboard in the Route 53 console.\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"The ID of one or more security groups that you want to use to control access to this VPC. The security group that you specify must include one or more inbound rules (for inbound Resolver endpoints) or outbound rules (for outbound Resolver endpoints). Inbound and outbound rules must allow TCP and UDP access. For inbound access, open port 53. For outbound access, open the port that you're using for DNS queries on your network.\"\n        }\n      ]\n    },\n    \"Direction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverEndpointDirection\"\n        },\n        {\n          \"description\": \"<p>Specify the applicable\
  \ value:</p> <ul> <li> <p> <code>INBOUND</code>: Resolver forwards DNS queries to the DNS service for a VPC from your network</p> </li> <li> <p> <code>OUTBOUND</code>: Resolver forwards DNS queries from the DNS service for a VPC to your network</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"IpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressesRequest\"\n        },\n        {\n          \"description\": \"The subnets and IP addresses in your VPC that DNS queries originate from (for outbound endpoints) or that you forward DNS queries to (for inbound endpoints). The subnet ID uniquely identifies a VPC. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of the tag keys and values that you want to associate with the endpoint.\"\n        }\n      ]\n    },\n    \"ResolverEndpointType\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverEndpointType\"\n        },\n        {\n          \"description\": \" For the endpoint type you can choose either IPv4, IPv6. or dual-stack. A dual-stack endpoint means that it will resolve via both IPv4 and IPv6. This endpoint type is applied to all IP addresses. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreatorRequestId\",\n    \"SecurityGroupIds\",\n    \"Direction\",\n    \"IpAddresses\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-resolver-endpoint-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: CreateResolverEndpointRequest
---
