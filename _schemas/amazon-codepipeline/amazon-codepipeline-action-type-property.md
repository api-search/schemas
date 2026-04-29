---
description: Represents information about each property specified in the action configuration, such as the description and key name that display for the customer using the action type.
layout: schema
name: ActionTypeProperty
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: optional
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: noEcho
  type: object
- description: ''
  name: queryable
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-property-schema.json
slug: amazon-codepipeline-action-type-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-property-schema.json\",\n  \"title\": \"ActionTypeProperty\",\n  \"description\": \"Represents information about each property specified in the action configuration, such as the description and key name that display for the customer using the action type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionConfigurationKey\"\n        },\n        {\n          \"description\": \"The property name that is displayed to users.\"\n        }\n      ]\n    },\n    \"optional\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the configuration property is an optional value.\"\n      \
  \  }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the configuration property is a key.\"\n        }\n      ]\n    },\n    \"noEcho\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether to omit the field value entered by the customer in the log. If <code>true</code>, the value is not saved in CloudTrail logs for the action execution.\"\n        }\n      ]\n    },\n    \"queryable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates that the property is used with polling. An action type can have up to one queryable property. If it has one, that property must be both required and not secret.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/PropertyDescription\"\n        },\n        {\n          \"description\": \"The description of the property that is displayed to users.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"optional\",\n    \"key\",\n    \"noEcho\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-property-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypeProperty
---
