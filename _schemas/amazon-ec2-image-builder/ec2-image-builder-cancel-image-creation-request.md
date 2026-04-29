---
description: CancelImageCreationRequest schema from EC2 Image Builder
layout: schema
name: CancelImageCreationRequest
properties_list:
- description: ''
  name: imageBuildVersionArn
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-cancel-image-creation-request-schema.json
slug: ec2-image-builder-cancel-image-creation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-cancel-image-creation-request-schema.json\",\n  \"title\": \"CancelImageCreationRequest\",\n  \"description\": \"CancelImageCreationRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image that you want to cancel creation for.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier you provide to ensure idempotency of the request. For more information,\
  \ see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/Run_Instance_Idempotency.html\\\">Ensuring idempotency</a> in the <i>Amazon EC2 API Reference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"imageBuildVersionArn\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-cancel-image-creation-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CancelImageCreationRequest
---
