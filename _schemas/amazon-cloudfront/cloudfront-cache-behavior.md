---
description: CacheBehavior schema
layout: schema
name: CacheBehavior
properties_list:
- description: The pattern that specifies which requests to apply the behavior to. Not required for the default cache behavior.
  name: PathPattern
  type: string
- description: The ID of the origin that you want CloudFront to route requests to.
  name: TargetOriginId
  type: string
- description: The protocol that viewers can use to access the files in the origin.
  name: ViewerProtocolPolicy
  type: string
- description: ''
  name: AllowedMethods
  type: object
- description: The unique identifier of the cache policy.
  name: CachePolicyId
  type: string
- description: The unique identifier of the origin request policy.
  name: OriginRequestPolicyId
  type: string
- description: Whether you want CloudFront to automatically compress certain files for this cache behavior.
  name: Compress
  type: boolean
- description: ''
  name: FunctionAssociations
  type: object
- description: ''
  name: LambdaFunctionAssociations
  type: object
provider_name: Amazon CloudFront
provider_slug: amazon-cloudfront
schema_file: json-schema/cloudfront-cache-behavior-schema.json
slug: cloudfront-cache-behavior
source_filename: cloudfront-cache-behavior-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-cache-behavior-schema.json\",\n  \"title\": \"CacheBehavior\",\n  \"description\": \"CacheBehavior schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PathPattern\": {\n      \"type\": \"string\",\n      \"description\": \"The pattern that specifies which requests to apply the behavior to. Not required for the default cache behavior.\"\n    },\n    \"TargetOriginId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the origin that you want CloudFront to route requests to.\"\n    },\n    \"ViewerProtocolPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow-all\",\n        \"https-only\",\n        \"redirect-to-https\"\n      ],\n      \"description\": \"The protocol that viewers can use to access the files in the origin.\"\n    },\n    \"\
  AllowedMethods\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Quantity\": {\n          \"type\": \"integer\"\n        },\n        \"Items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"GET\",\n              \"HEAD\",\n              \"POST\",\n              \"PUT\",\n              \"PATCH\",\n              \"OPTIONS\",\n              \"DELETE\"\n            ]\n          }\n        }\n      }\n    },\n    \"CachePolicyId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cache policy.\"\n    },\n    \"OriginRequestPolicyId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the origin request policy.\"\n    },\n    \"Compress\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether you want CloudFront to automatically compress certain files for this cache behavior.\"\n    },\n    \"FunctionAssociations\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Quantity\": {\n          \"type\": \"integer\"\n        },\n        \"Items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"FunctionARN\": {\n                \"type\": \"string\"\n              },\n              \"EventType\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"viewer-request\",\n                  \"viewer-response\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    },\n    \"LambdaFunctionAssociations\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Quantity\": {\n          \"type\": \"integer\"\n        },\n        \"Items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"LambdaFunctionARN\": {\n                \"type\"\
  : \"string\"\n              },\n              \"EventType\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"viewer-request\",\n                  \"viewer-response\",\n                  \"origin-request\",\n                  \"origin-response\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"ViewerProtocolPolicy\",\n    \"TargetOriginId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-cache-behavior-schema.json
tags:
- CloudFront
- CDN
- Content Delivery
- Edge
title: CacheBehavior
---
