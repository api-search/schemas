---
description: The environment template version data.
layout: schema
name: EnvironmentTemplateVersion
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
  name: lastModifiedAt
  type: object
- description: ''
  name: majorVersion
  type: object
- description: ''
  name: minorVersion
  type: object
- description: ''
  name: recommendedMinorVersion
  type: object
- description: ''
  name: schema
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-environment-template-version-schema.json
slug: amazon-proton-environment-template-version
source_filename: amazon-proton-environment-template-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-template-version-schema.json\",\n  \"title\": \"EnvironmentTemplateVersion\",\n  \"description\": \"The environment template version data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentTemplateVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the version of an environment template.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the version of an environment template was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the minor version of an environment template.\"\n        }\n      ]\n    },\n    \"lastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the version of an environment template was last modified.\"\n        }\n      ]\n    },\n    \"majorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The latest major version that's associated with the version of an environment template.\"\n        }\n      ]\n    },\n    \"minorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The minor version of an environment template.\"\n        }\n    \
  \  ]\n    },\n    \"recommendedMinorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The recommended minor version of the environment template.\"\n        }\n      ]\n    },\n    \"schema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateSchema\"\n        },\n        {\n          \"description\": \"The schema of the version of an environment template.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionStatus\"\n        },\n        {\n          \"description\": \"The status of the version of an environment template.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"The status message of the version of an\
  \ environment template.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the version of an environment template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"lastModifiedAt\",\n    \"majorVersion\",\n    \"minorVersion\",\n    \"status\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-template-version-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: EnvironmentTemplateVersion
---
