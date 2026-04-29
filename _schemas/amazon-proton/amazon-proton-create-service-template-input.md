---
description: CreateServiceTemplateInput schema from Amazon Proton API
layout: schema
name: CreateServiceTemplateInput
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: encryptionKey
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: pipelineProvisioning
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-service-template-input-schema.json
slug: amazon-proton-create-service-template-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-template-input-schema.json\",\n  \"title\": \"CreateServiceTemplateInput\",\n  \"description\": \"CreateServiceTemplateInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the service template.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayName\"\n        },\n        {\n          \"description\": \"The name of the service template as displayed in the developer interface.\"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"A customer provided encryption key that's used to encrypt data.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service template.\"\n        }\n      ]\n    },\n    \"pipelineProvisioning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Provisioning\"\n        },\n        {\n          \"description\": \"By default, Proton provides a service pipeline for your service. When this parameter is included, it indicates that an Proton service pipeline <i>isn't</i> provided for your service. After it's included, it <i>can't</i> be changed. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-template-authoring.html#ag-template-bundles\\\">Template bundles</a> in the <i>Proton User Guide</i>.\"\
  \n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An optional list of metadata items that you can associate with the Proton service template. A tag is a key-value pair.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/resources.html\\\">Proton resources and tagging</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-template-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateServiceTemplateInput
---
