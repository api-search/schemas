---
description: The environment template data.
layout: schema
name: EnvironmentTemplateSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: lastModifiedAt
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: provisioning
  type: object
- description: ''
  name: recommendedVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-environment-template-summary-schema.json
slug: amazon-proton-environment-template-summary
source_filename: amazon-proton-environment-template-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-template-summary-schema.json\",\n  \"title\": \"EnvironmentTemplateSummary\",\n  \"description\": \"The environment template data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentTemplateArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the environment template.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the environment template was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\
  \n        },\n        {\n          \"description\": \"A description of the environment template.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayName\"\n        },\n        {\n          \"description\": \"The name of the environment template as displayed in the developer interface.\"\n        }\n      ]\n    },\n    \"lastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the environment template was last modified.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment template.\"\n        }\n      ]\n    },\n    \"provisioning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Provisioning\"\n\
  \        },\n        {\n          \"description\": \"When included, indicates that the environment template is for customer provisioned and managed infrastructure.\"\n        }\n      ]\n    },\n    \"recommendedVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FullTemplateVersionNumber\"\n        },\n        {\n          \"description\": \"The recommended version of the environment template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"lastModifiedAt\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-template-summary-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: EnvironmentTemplateSummary
---
