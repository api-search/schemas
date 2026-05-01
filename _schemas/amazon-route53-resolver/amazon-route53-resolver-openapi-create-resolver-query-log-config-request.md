---
description: CreateResolverQueryLogConfigRequest schema from openapi
layout: schema
name: CreateResolverQueryLogConfigRequest
properties_list:
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
  name: Tags
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-create-resolver-query-log-config-request-schema.json
slug: amazon-route53-resolver-openapi-create-resolver-query-log-config-request
source_filename: amazon-route53-resolver-openapi-create-resolver-query-log-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-resolver-query-log-config-request-schema.json\",\n  \"title\": \"CreateResolverQueryLogConfigRequest\",\n  \"description\": \"CreateResolverQueryLogConfigRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigName\"\n        },\n        {\n          \"description\": \"The name that you want to give the query logging configuration.\"\n        }\n      ]\n    },\n    \"DestinationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationArn\"\n        },\n        {\n          \"description\": \"<p>The ARN of the resource that you want Resolver to send query logs. You can send query logs to\
  \ an S3 bucket, a CloudWatch Logs log group, or a Kinesis Data Firehose delivery stream. Examples of valid values include the following:</p> <ul> <li> <p> <b>S3 bucket</b>: </p> <p> <code>arn:aws:s3:::examplebucket</code> </p> <p>You can optionally append a file prefix to the end of the ARN.</p> <p> <code>arn:aws:s3:::examplebucket/development/</code> </p> </li> <li> <p> <b>CloudWatch Logs log group</b>: </p> <p> <code>arn:aws:logs:us-west-1:123456789012:log-group:/mystack-testgroup-12ABC1AB12A1:*</code> </p> </li> <li> <p> <b>Kinesis Data Firehose delivery stream</b>:</p> <p> <code>arn:aws:kinesis:us-east-2:0123456789:stream/my_stream_name</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that identifies the request and that allows failed requests to be retried without the risk of running the\
  \ operation twice. <code>CreatorRequestId</code> can be any unique string, for example, a date/time stamp. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of the tag keys and values that you want to associate with the query logging configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"DestinationArn\",\n    \"CreatorRequestId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-resolver-query-log-config-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: CreateResolverQueryLogConfigRequest
---
