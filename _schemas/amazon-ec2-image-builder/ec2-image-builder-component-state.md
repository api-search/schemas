---
description: A group of fields that describe the current status of components that are no longer active.
layout: schema
name: ComponentState
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: reason
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-component-state-schema.json
slug: ec2-image-builder-component-state
source_filename: ec2-image-builder-component-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-state-schema.json\",\n  \"title\": \"ComponentState\",\n  \"description\": \"A group of fields that describe the current status of components that are no longer active.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentStatus\"\n        },\n        {\n          \"description\": \"The current state of the component.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Describes how or why the component changed state.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-state-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ComponentState
---
