---
description: GetImagePolicyResponse schema from EC2 Image Builder
layout: schema
name: GetImagePolicyResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: policy
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-get-image-policy-response-schema.json
slug: ec2-image-builder-get-image-policy-response
source_filename: ec2-image-builder-get-image-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-get-image-policy-response-schema.json\",\n  \"title\": \"GetImagePolicyResponse\",\n  \"description\": \"GetImagePolicyResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicyDocument\"\n        },\n        {\n          \"description\": \"The image policy object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-get-image-policy-response-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: GetImagePolicyResponse
---
