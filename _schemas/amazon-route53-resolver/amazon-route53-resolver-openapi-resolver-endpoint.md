---
description: In the response to a <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverEndpoint.html">CreateResolverEndpoint</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DeleteResolverEndpoint.html">DeleteResolverEndpoint</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverEndpoint.html">GetResolverEndpoint</a>, Updates the name, or ResolverEndpointType for an endpoint, or <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverEndpoint.html">UpdateResolverEndpoint</a> request, a complex type that contains settings for an existing inbound or outbound Resolver endpoint.
layout: schema
name: ResolverEndpoint
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: Arn
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
  name: IpAddressCount
  type: object
- description: ''
  name: HostVPCId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: ModificationTime
  type: object
- description: ''
  name: ResolverEndpointType
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-resolver-endpoint-schema.json
slug: amazon-route53-resolver-openapi-resolver-endpoint
source_filename: amazon-route53-resolver-openapi-resolver-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-endpoint-schema.json\",\n  \"title\": \"ResolverEndpoint\",\n  \"description\": \"In the response to a <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverEndpoint.html\\\">CreateResolverEndpoint</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DeleteResolverEndpoint.html\\\">DeleteResolverEndpoint</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverEndpoint.html\\\">GetResolverEndpoint</a>, Updates the name, or ResolverEndpointType for an endpoint, or <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverEndpoint.html\\\">UpdateResolverEndpoint</a> request, a complex\
  \ type that contains settings for an existing inbound or outbound Resolver endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver endpoint.\"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that identifies the request that created the Resolver endpoint. The <code>CreatorRequestId</code> allows failed requests to be retried without the risk of running the operation twice.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN (Amazon Resource Name) for the Resolver endpoint.\"\n        }\n      ]\n    },\n \
  \   \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name that you assigned to the Resolver endpoint when you submitted a <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverEndpoint.html\\\">CreateResolverEndpoint</a> request.\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"The ID of one or more security groups that control access to this VPC. The security group must include one or more inbound rules (for inbound endpoints) or outbound rules (for outbound endpoints). Inbound and outbound rules must allow TCP and UDP access. For inbound access, open port 53. For outbound access, open the port that you're using for DNS queries on your network.\"\n        }\n      ]\n    },\n    \"Direction\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverEndpointDirection\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the Resolver endpoint allows inbound or outbound DNS queries:</p> <ul> <li> <p> <code>INBOUND</code>: allows DNS queries to your VPC from your network</p> </li> <li> <p> <code>OUTBOUND</code>: allows DNS queries from your VPC to your network</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"IpAddressCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressCount\"\n        },\n        {\n          \"description\": \"The number of IP addresses that the Resolver endpoint can use for DNS queries.\"\n        }\n      ]\n    },\n    \"HostVPCId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the VPC that you want to create the Resolver endpoint in.\"\n        }\n    \
  \  ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverEndpointStatus\"\n        },\n        {\n          \"description\": \"<p>A code that specifies the current status of the Resolver endpoint. Valid values include the following:</p> <ul> <li> <p> <code>CREATING</code>: Resolver is creating and configuring one or more Amazon VPC network interfaces for this endpoint.</p> </li> <li> <p> <code>OPERATIONAL</code>: The Amazon VPC network interfaces for this endpoint are correctly configured and able to pass inbound or outbound DNS queries between your network and Resolver.</p> </li> <li> <p> <code>UPDATING</code>: Resolver is associating or disassociating one or more network interfaces with this endpoint.</p> </li> <li> <p> <code>AUTO_RECOVERING</code>: Resolver is trying to recover one or more of the network interfaces that are associated with this endpoint. During the recovery process, the endpoint functions with limited capacity\
  \ because of the limit on the number of DNS queries per IP address (per network interface). For the current limit, see <a href=\\\"https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/DNSLimitations.html#limits-api-entities-resolver\\\">Limits on Route 53 Resolver</a>.</p> </li> <li> <p> <code>ACTION_NEEDED</code>: This endpoint is unhealthy, and Resolver can't automatically recover it. To resolve the problem, we recommend that you check each IP address that you associated with the endpoint. For each IP address that isn't available, add another IP address and then delete the IP address that isn't available. (An endpoint must always include at least two IP addresses.) A status of <code>ACTION_NEEDED</code> can have a variety of causes. Here are two common causes:</p> <ul> <li> <p>One or more of the network interfaces that are associated with the endpoint were deleted using Amazon VPC.</p> </li> <li> <p>The network interface couldn't be created for some reason that's outside the control\
  \ of Resolver.</p> </li> </ul> </li> <li> <p> <code>DELETING</code>: Resolver is deleting this endpoint and the associated network interfaces.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"A detailed description of the status of the Resolver endpoint.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the endpoint was created, in Unix time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    },\n    \"ModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the endpoint was last modified, in Unix\
  \ time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    },\n    \"ResolverEndpointType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverEndpointType\"\n        },\n        {\n          \"description\": \" The Resolver endpoint IP address type. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-endpoint-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: ResolverEndpoint
---
