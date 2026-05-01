---
description: DistributionList schema
layout: schema
name: DistributionList
properties_list:
- description: ''
  name: Marker
  type: string
- description: ''
  name: NextMarker
  type: string
- description: ''
  name: MaxItems
  type: integer
- description: ''
  name: IsTruncated
  type: boolean
- description: ''
  name: Quantity
  type: integer
- description: ''
  name: Items
  type: array
provider_name: Amazon CloudFront
provider_slug: amazon-cloudfront
schema_file: json-schema/cloudfront-distribution-list-schema.json
slug: cloudfront-distribution-list
source_filename: cloudfront-distribution-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-distribution-list-schema.json\",\n  \"title\": \"DistributionList\",\n  \"description\": \"DistributionList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Marker\": {\n      \"type\": \"string\"\n    },\n    \"NextMarker\": {\n      \"type\": \"string\"\n    },\n    \"MaxItems\": {\n      \"type\": \"integer\"\n    },\n    \"IsTruncated\": {\n      \"type\": \"boolean\"\n    },\n    \"Quantity\": {\n      \"type\": \"integer\"\n    },\n    \"Items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Distribution\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-distribution-list-schema.json
tags:
- CloudFront
- CDN
- Content Delivery
- Edge
title: DistributionList
---
