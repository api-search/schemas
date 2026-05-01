---
description: PutComponentPolicyRequest schema from EC2 Image Builder
layout: schema
name: PutComponentPolicyRequest
properties_list:
- description: ''
  name: componentArn
  type: object
- description: ''
  name: policy
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-put-component-policy-request-schema.json
slug: ec2-image-builder-put-component-policy-request
source_filename: ec2-image-builder-put-component-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-put-component-policy-request-schema.json\",\n  \"title\": \"PutComponentPolicyRequest\",\n  \"description\": \"PutComponentPolicyRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the component that this policy should be applied to.\"\n        }\n      ]\n    },\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicyDocument\"\n        },\n        {\n          \"description\": \"The policy to apply.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"componentArn\",\n \
  \   \"policy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-put-component-policy-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: PutComponentPolicyRequest
---
