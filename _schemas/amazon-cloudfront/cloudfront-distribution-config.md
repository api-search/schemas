---
description: DistributionConfig schema
layout: schema
name: DistributionConfig
properties_list:
- description: A unique value that ensures the request can't be replayed.
  name: CallerReference
  type: string
- description: CNAMEs (alternate domain names) for the distribution.
  name: Aliases
  type: object
- description: The object that you want CloudFront to return when an end user requests the root URL.
  name: DefaultRootObject
  type: string
- description: ''
  name: Origins
  type: object
- description: ''
  name: DefaultCacheBehavior
  type: object
- description: ''
  name: CacheBehaviors
  type: object
- description: A comment to describe the distribution.
  name: Comment
  type: string
- description: Whether the distribution is enabled to accept user requests.
  name: Enabled
  type: boolean
- description: The price class for the distribution.
  name: PriceClass
  type: string
- description: ''
  name: ViewerCertificate
  type: object
- description: The AWS WAF web ACL to associate with this distribution.
  name: WebACLId
  type: string
- description: ''
  name: HttpVersion
  type: string
- description: ''
  name: IsIPV6Enabled
  type: boolean
provider_name: Amazon CloudFront
provider_slug: amazon-cloudfront
schema_file: json-schema/cloudfront-distribution-config-schema.json
slug: cloudfront-distribution-config
source_filename: cloudfront-distribution-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-distribution-config-schema.json\",\n  \"title\": \"DistributionConfig\",\n  \"description\": \"DistributionConfig schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CallerReference\": {\n      \"type\": \"string\",\n      \"description\": \"A unique value that ensures the request can't be replayed.\"\n    },\n    \"Aliases\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Quantity\": {\n          \"type\": \"integer\"\n        },\n        \"Items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"CNAMEs (alternate domain names) for the distribution.\"\n    },\n    \"DefaultRootObject\": {\n      \"type\": \"string\",\n      \"description\": \"The object that\
  \ you want CloudFront to return when an end user requests the root URL.\"\n    },\n    \"Origins\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Quantity\": {\n          \"type\": \"integer\"\n        },\n        \"Items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Origin\"\n          }\n        }\n      }\n    },\n    \"DefaultCacheBehavior\": {\n      \"$ref\": \"#/components/schemas/CacheBehavior\"\n    },\n    \"CacheBehaviors\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Quantity\": {\n          \"type\": \"integer\"\n        },\n        \"Items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/CacheBehavior\"\n          }\n        }\n      }\n    },\n    \"Comment\": {\n      \"type\": \"string\",\n      \"description\": \"A comment to describe the distribution.\"\n    },\n    \"Enabled\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether the distribution is enabled to accept user requests.\"\n    },\n    \"PriceClass\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PriceClass_100\",\n        \"PriceClass_200\",\n        \"PriceClass_All\"\n      ],\n      \"description\": \"The price class for the distribution.\"\n    },\n    \"ViewerCertificate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"CloudFrontDefaultCertificate\": {\n          \"type\": \"boolean\"\n        },\n        \"ACMCertificateArn\": {\n          \"type\": \"string\"\n        },\n        \"SSLSupportMethod\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"sni-only\",\n            \"vip\",\n            \"static-ip\"\n          ]\n        },\n        \"MinimumProtocolVersion\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"WebACLId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS WAF web ACL to associate with this\
  \ distribution.\"\n    },\n    \"HttpVersion\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"http1.1\",\n        \"http2\",\n        \"http3\",\n        \"http2and3\"\n      ]\n    },\n    \"IsIPV6Enabled\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"CallerReference\",\n    \"Origins\",\n    \"DefaultCacheBehavior\",\n    \"Comment\",\n    \"Enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-distribution-config-schema.json
tags:
- AWS
- CloudFront
- CDN
- Content Delivery
- Edge
title: DistributionConfig
---
