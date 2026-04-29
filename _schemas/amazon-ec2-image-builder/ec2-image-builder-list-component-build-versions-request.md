---
description: ListComponentBuildVersionsRequest schema from EC2 Image Builder
layout: schema
name: ListComponentBuildVersionsRequest
properties_list:
- description: ''
  name: componentVersionArn
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-component-build-versions-request-schema.json
slug: ec2-image-builder-list-component-build-versions-request
source_filename: ec2-image-builder-list-component-build-versions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-component-build-versions-request-schema.json\",\n  \"title\": \"ListComponentBuildVersionsRequest\",\n  \"description\": \"ListComponentBuildVersionsRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionArn\"\n        },\n        {\n          \"description\": \"The component version Amazon Resource Name (ARN) whose versions you want to list.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RestrictedInteger\"\n        },\n        {\n          \"description\": \"The maximum items to return in a request.\"\n        }\n      ]\n    },\n    \"\
  nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A token to specify where to start paginating. This is the NextToken from a previously truncated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"componentVersionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-component-build-versions-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListComponentBuildVersionsRequest
---
