---
description: CreateServiceInput schema from Amazon Proton API
layout: schema
name: CreateServiceInput
properties_list:
- description: ''
  name: branchName
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: repositoryConnectionArn
  type: object
- description: ''
  name: repositoryId
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: templateMajorVersion
  type: object
- description: ''
  name: templateMinorVersion
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-service-input-schema.json
slug: amazon-proton-create-service-input
source_filename: amazon-proton-create-service-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-input-schema.json\",\n  \"title\": \"CreateServiceInput\",\n  \"description\": \"CreateServiceInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branchName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The name of the code repository branch that holds the code that's deployed in Proton. <i>Don't</i> include this parameter if your service template <i>doesn't</i> include a service pipeline.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the Proton service.\"\n        }\n  \
  \    ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The service name.\"\n        }\n      ]\n    },\n    \"repositoryConnectionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the repository connection. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/setting-up-for-service.html#setting-up-vcontrol\\\">Setting up an AWS CodeStar connection</a> in the <i>Proton User Guide</i>. <i>Don't</i> include this parameter if your service template <i>doesn't</i> include a service pipeline.\"\n        }\n      ]\n    },\n    \"repositoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryId\"\n        },\n        {\n          \"description\": \"The ID of the code repository.\
  \ <i>Don't</i> include this parameter if your service template <i>doesn't</i> include a service pipeline.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"A link to a spec file that provides inputs as defined in the service template bundle schema file. The spec file is in YAML format. <i>Don\\u2019t</i> include pipeline inputs in the spec if your service template <i>doesn\\u2019t</i> include a service pipeline. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-create-svc.html\\\">Create a service</a> in the <i>Proton User Guide</i>.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An optional list of metadata items that you can associate with the Proton service. A tag\
  \ is a key-value pair.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/resources.html\\\">Proton resources and tagging</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"templateMajorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The major version of the service template that was used to create the service.\"\n        }\n      ]\n    },\n    \"templateMinorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The minor version of the service template that was used to create the service.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name\
  \ of the service template that's used to create the service.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"spec\",\n    \"templateMajorVersion\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateServiceInput
---
