---
description: ListComponentBuildVersionsResponse schema from EC2 Image Builder
layout: schema
name: ListComponentBuildVersionsResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: componentSummaryList
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-component-build-versions-response-schema.json
slug: ec2-image-builder-list-component-build-versions-response
source_filename: ec2-image-builder-list-component-build-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-component-build-versions-response-schema.json\",\n  \"title\": \"ListComponentBuildVersionsResponse\",\n  \"description\": \"ListComponentBuildVersionsResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"componentSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentSummaryList\"\n        },\n        {\n          \"description\": \"The list of component summaries for the specified semantic version.\"\n        }\n      ]\n    },\n    \"nextToken\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The next token used for paginated responses. When this field isn't empty, there are additional elements that the service has'ot included in this request. Use this token with the next request to retrieve additional objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-component-build-versions-response-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListComponentBuildVersionsResponse
---
