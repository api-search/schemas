---
description: Distribution schema
layout: schema
name: Distribution
properties_list:
- description: The distribution's unique identifier.
  name: Id
  type: string
- description: The ARN of the distribution.
  name: ARN
  type: string
- description: The current status of the distribution (e.g., Deployed, InProgress).
  name: Status
  type: string
- description: The date and time the distribution was last modified.
  name: LastModifiedTime
  type: string
- description: The domain name corresponding to the distribution (e.g., d111111abcdef8.cloudfront.net).
  name: DomainName
  type: string
- description: ''
  name: DistributionConfig
  type: object
provider_name: Amazon CloudFront
provider_slug: amazon-cloudfront
schema_file: json-schema/cloudfront-distribution-schema.json
slug: cloudfront-distribution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-distribution-schema.json\",\n  \"title\": \"Distribution\",\n  \"description\": \"Distribution schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The distribution's unique identifier.\"\n    },\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the distribution.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the distribution (e.g., Deployed, InProgress).\"\n    },\n    \"LastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the distribution was last modified.\"\n    },\n    \"DomainName\": {\n      \"type\": \"string\",\n      \"description\": \"The domain\
  \ name corresponding to the distribution (e.g., d111111abcdef8.cloudfront.net).\"\n    },\n    \"DistributionConfig\": {\n      \"$ref\": \"#/components/schemas/DistributionConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-distribution-schema.json
tags:
- AWS
- CloudFront
- CDN
- Content Delivery
- Edge
title: Distribution
---
