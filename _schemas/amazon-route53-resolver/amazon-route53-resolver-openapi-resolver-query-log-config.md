---
description: In the response to a <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverQueryLogConfig.html">CreateResolverQueryLogConfig</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DeleteResolverQueryLogConfig.html">DeleteResolverQueryLogConfig</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverQueryLogConfig.html">GetResolverQueryLogConfig</a>, or <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_ListResolverQueryLogConfigs.html">ListResolverQueryLogConfigs</a> request, a complex type that contains settings for one query logging configuration.
layout: schema
name: ResolverQueryLogConfig
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ShareStatus
  type: object
- description: ''
  name: AssociationCount
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: DestinationArn
  type: object
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: CreationTime
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-resolver-query-log-config-schema.json
slug: amazon-route53-resolver-openapi-resolver-query-log-config
source_filename: amazon-route53-resolver-openapi-resolver-query-log-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-query-log-config-schema.json\",\n  \"title\": \"ResolverQueryLogConfig\",\n  \"description\": \"In the response to a <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverQueryLogConfig.html\\\">CreateResolverQueryLogConfig</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DeleteResolverQueryLogConfig.html\\\">DeleteResolverQueryLogConfig</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverQueryLogConfig.html\\\">GetResolverQueryLogConfig</a>, or <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_ListResolverQueryLogConfigs.html\\\">ListResolverQueryLogConfigs</a> request, a complex\
  \ type that contains settings for one query logging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID for the query logging configuration.\"\n        }\n      ]\n    },\n    \"OwnerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account that created the query logging configuration. \"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the specified query logging configuration. Valid values include the following:</p> <ul> <li> <p> <code>CREATING</code>: Resolver is creating the query logging configuration.</p>\
  \ </li> <li> <p> <code>CREATED</code>: The query logging configuration was successfully created. Resolver is logging queries that originate in the specified VPC.</p> </li> <li> <p> <code>DELETING</code>: Resolver is deleting this query logging configuration.</p> </li> <li> <p> <code>FAILED</code>: Resolver can't deliver logs to the location that is specified in the query logging configuration. Here are two common causes:</p> <ul> <li> <p>The specified destination (for example, an Amazon S3 bucket) was deleted.</p> </li> <li> <p>Permissions don't allow sending logs to the destination.</p> </li> </ul> </li> </ul>\"\n        }\n      ]\n    },\n    \"ShareStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareStatus\"\n        },\n        {\n          \"description\": \"An indication of whether the query logging configuration is shared with other Amazon Web Services accounts, or was shared with the current account by another Amazon Web Services account.\
  \ Sharing is configured through Resource Access Manager (RAM).\"\n        }\n      ]\n    },\n    \"AssociationCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The number of VPCs that are associated with the query logging configuration.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN for the query logging configuration.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigName\"\n        },\n        {\n          \"description\": \"The name of the query logging configuration. \"\n        }\n      ]\n    },\n    \"DestinationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationArn\"\n        },\n        {\n          \"description\"\
  : \"The ARN of the resource that you want Resolver to send query logs: an Amazon S3 bucket, a CloudWatch Logs log group, or a Kinesis Data Firehose delivery stream.\"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that identifies the request that created the query logging configuration. The <code>CreatorRequestId</code> allows failed requests to be retried without the risk of running the operation twice.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the query logging configuration was created, in Unix time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-query-log-config-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ResolverQueryLogConfig
---
