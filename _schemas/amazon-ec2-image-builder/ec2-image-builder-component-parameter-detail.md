---
description: Defines a parameter that is used to provide configuration details for the component.
layout: schema
name: ComponentParameterDetail
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: defaultValue
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-component-parameter-detail-schema.json
slug: ec2-image-builder-component-parameter-detail
source_filename: ec2-image-builder-component-parameter-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-parameter-detail-schema.json\",\n  \"title\": \"ComponentParameterDetail\",\n  \"description\": \"Defines a parameter that is used to provide configuration details for the component.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentParameterName\"\n        },\n        {\n          \"description\": \"The name of this input parameter.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentParameterType\"\n        },\n        {\n          \"description\": \"The type of input this parameter provides. The currently supported value is \\\"string\\\".\"\n        }\n      ]\n    },\n    \"defaultValue\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentParameterValueList\"\n        },\n        {\n          \"description\": \"The default value of this parameter if no input is provided.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentParameterDescription\"\n        },\n        {\n          \"description\": \"Describes this parameter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-parameter-detail-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ComponentParameterDetail
---
