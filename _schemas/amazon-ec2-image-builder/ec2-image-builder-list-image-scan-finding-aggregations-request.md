---
description: ListImageScanFindingAggregationsRequest schema from EC2 Image Builder
layout: schema
name: ListImageScanFindingAggregationsRequest
properties_list:
- description: ''
  name: filter
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-image-scan-finding-aggregations-request-schema.json
slug: ec2-image-builder-list-image-scan-finding-aggregations-request
source_filename: ec2-image-builder-list-image-scan-finding-aggregations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-scan-finding-aggregations-request-schema.json\",\n  \"title\": \"ListImageScanFindingAggregationsRequest\",\n  \"description\": \"ListImageScanFindingAggregationsRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"$ref\": \"#/components/schemas/Filter\"\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A token to specify where to start paginating. This is the NextToken from a previously truncated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-scan-finding-aggregations-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListImageScanFindingAggregationsRequest
---
