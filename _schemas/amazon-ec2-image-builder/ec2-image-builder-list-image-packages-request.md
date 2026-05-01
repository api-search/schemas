---
description: ListImagePackagesRequest schema from EC2 Image Builder
layout: schema
name: ListImagePackagesRequest
properties_list:
- description: ''
  name: imageBuildVersionArn
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-image-packages-request-schema.json
slug: ec2-image-builder-list-image-packages-request
source_filename: ec2-image-builder-list-image-packages-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-packages-request-schema.json\",\n  \"title\": \"ListImagePackagesRequest\",\n  \"description\": \"ListImagePackagesRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"Filter results for the ListImagePackages request by the Image Build Version ARN\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RestrictedInteger\"\n        },\n        {\n          \"description\": \"The maximum items to return in a request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A token to specify where to start paginating. This is the NextToken from a previously truncated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"imageBuildVersionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-packages-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListImagePackagesRequest
---
