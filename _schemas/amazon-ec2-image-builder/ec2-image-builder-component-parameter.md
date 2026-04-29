---
description: Contains a key/value pair that sets the named component parameter.
layout: schema
name: ComponentParameter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-component-parameter-schema.json
slug: ec2-image-builder-component-parameter
source_filename: ec2-image-builder-component-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-parameter-schema.json\",\n  \"title\": \"ComponentParameter\",\n  \"description\": \"Contains a key/value pair that sets the named component parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentParameterName\"\n        },\n        {\n          \"description\": \"The name of the component parameter to set.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentParameterValueList\"\n        },\n        {\n          \"description\": \"Sets the value for the named component parameter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-parameter-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ComponentParameter
---
