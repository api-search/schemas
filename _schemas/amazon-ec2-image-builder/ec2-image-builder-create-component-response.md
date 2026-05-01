---
description: CreateComponentResponse schema from EC2 Image Builder
layout: schema
name: CreateComponentResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: componentBuildVersionArn
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-create-component-response-schema.json
slug: ec2-image-builder-create-component-response
source_filename: ec2-image-builder-create-component-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-component-response-schema.json\",\n  \"title\": \"CreateComponentResponse\",\n  \"description\": \"CreateComponentResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token used to make this request idempotent.\"\n        }\n      ]\n    },\n    \"componentBuildVersionArn\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/ComponentBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the component that this request created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-component-response-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CreateComponentResponse
---
