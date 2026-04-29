---
description: Origin schema
layout: schema
name: Origin
properties_list:
- description: A unique identifier for the origin.
  name: Id
  type: string
- description: The domain name for the origin (e.g., my-bucket.s3.amazonaws.com).
  name: DomainName
  type: string
- description: An optional path to append to the origin domain name.
  name: OriginPath
  type: string
- description: ''
  name: S3OriginConfig
  type: object
- description: ''
  name: CustomOriginConfig
  type: object
provider_name: Amazon CloudFront
provider_slug: amazon-cloudfront
schema_file: json-schema/cloudfront-origin-schema.json
slug: cloudfront-origin
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-origin-schema.json\",\n  \"title\": \"Origin\",\n  \"description\": \"Origin schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the origin.\"\n    },\n    \"DomainName\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name for the origin (e.g., my-bucket.s3.amazonaws.com).\"\n    },\n    \"OriginPath\": {\n      \"type\": \"string\",\n      \"description\": \"An optional path to append to the origin domain name.\"\n    },\n    \"S3OriginConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"OriginAccessIdentity\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"CustomOriginConfig\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"HTTPPort\": {\n          \"type\": \"integer\"\n        },\n        \"HTTPSPort\": {\n          \"type\": \"integer\"\n        },\n        \"OriginProtocolPolicy\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"http-only\",\n            \"match-viewer\",\n            \"https-only\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"Id\",\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-origin-schema.json
tags:
- AWS
- CloudFront
- CDN
- Content Delivery
- Edge
title: Origin
---
