---
description: UpdateResolverConfigRequest schema from openapi
layout: schema
name: UpdateResolverConfigRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: AutodefinedReverseFlag
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-resolver-config-request-schema.json
slug: amazon-route53-resolver-openapi-update-resolver-config-request
source_filename: amazon-route53-resolver-openapi-update-resolver-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-config-request-schema.json\",\n  \"title\": \"UpdateResolverConfigRequest\",\n  \"description\": \"UpdateResolverConfigRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"Resource ID of the Amazon VPC that you want to update the Resolver configuration for.\"\n        }\n      ]\n    },\n    \"AutodefinedReverseFlag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutodefinedReverseFlag\"\n        },\n        {\n          \"description\": \"<p>Indicates whether or not the Resolver will create autodefined rules for reverse DNS lookups.\
  \ This is enabled by default. Disabling this option will also affect EC2-Classic instances using ClassicLink. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/vpc-classiclink.html\\\">ClassicLink</a> in the <i>Amazon EC2 guide</i>.</p> <important> <p>We are retiring EC2-Classic on August 15, 2022. We recommend that you migrate from EC2-Classic to a VPC. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/vpc-migrate.html\\\">Migrate from EC2-Classic to a VPC</a> in the <i>Amazon EC2 guide</i> and the blog <a href=\\\"http://aws.amazon.com/blogs/aws/ec2-classic-is-retiring-heres-how-to-prepare/\\\">EC2-Classic Networking is Retiring \\u2013 Here\\u2019s How to Prepare</a>.</p> </important> <note> <p>It can take some time for the status change to be completed.</p> </note> <p/>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceId\",\n    \"AutodefinedReverseFlag\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-config-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: UpdateResolverConfigRequest
---
