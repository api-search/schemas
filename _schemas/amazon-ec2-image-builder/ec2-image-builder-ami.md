---
description: Details of an Amazon EC2 AMI.
layout: schema
name: Ami
properties_list:
- description: ''
  name: region
  type: object
- description: ''
  name: image
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: state
  type: object
- description: ''
  name: accountId
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-ami-schema.json
slug: ec2-image-builder-ami
source_filename: ec2-image-builder-ami-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ami-schema.json\",\n  \"title\": \"Ami\",\n  \"description\": \"Details of an Amazon EC2 AMI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region of the Amazon EC2 AMI.\"\n        }\n      ]\n    },\n    \"image\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The AMI ID of the Amazon EC2 AMI.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name\
  \ of the Amazon EC2 AMI.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the Amazon EC2 AMI. Minimum and maximum length are in characters.\"\n        }\n      ]\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/ImageState\"\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The account ID of the owner of the AMI.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ami-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: Ami
---
