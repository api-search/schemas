---
description: ListImageScanFindingsRequest schema from EC2 Image Builder
layout: schema
name: ListImageScanFindingsRequest
properties_list:
- description: ''
  name: filters
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-image-scan-findings-request-schema.json
slug: ec2-image-builder-list-image-scan-findings-request
source_filename: ec2-image-builder-list-image-scan-findings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-scan-findings-request-schema.json\",\n  \"title\": \"ListImageScanFindingsRequest\",\n  \"description\": \"ListImageScanFindingsRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageScanFindingsFilterList\"\n        },\n        {\n          \"description\": \"<p>An array of name value pairs that you can use to filter your results. You can use the following filters to streamline results:</p> <ul> <li> <p> <code>imageBuildVersionArn</code> </p> </li> <li> <p> <code>imagePipelineArn</code> </p> </li> <li> <p> <code>vulnerabilityId</code> </p> </li> <li> <p> <code>severity</code> </p> </li> </ul> <p>If you don't request a filter, then all\
  \ findings in your account are listed.</p>\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RestrictedInteger\"\n        },\n        {\n          \"description\": \"The maximum items to return in a request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A token to specify where to start paginating. This is the NextToken from a previously truncated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-scan-findings-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListImageScanFindingsRequest
---
