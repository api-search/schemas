---
description: ListImageScanFindingsResponse schema from EC2 Image Builder
layout: schema
name: ListImageScanFindingsResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: findings
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-image-scan-findings-response-schema.json
slug: ec2-image-builder-list-image-scan-findings-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-scan-findings-response-schema.json\",\n  \"title\": \"ListImageScanFindingsResponse\",\n  \"description\": \"ListImageScanFindingsResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"findings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageScanFindingsList\"\n        },\n        {\n          \"description\": \"The image scan findings for your account that meet your request filter criteria.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The next token used for paginated responses. When this field isn't empty, there are additional elements that the service has'ot included in this request. Use this token with the next request to retrieve additional objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-scan-findings-response-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListImageScanFindingsResponse
---
