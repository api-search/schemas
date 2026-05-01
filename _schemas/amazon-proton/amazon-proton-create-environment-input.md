---
description: CreateEnvironmentInput schema from Amazon Proton API
layout: schema
name: CreateEnvironmentInput
properties_list:
- description: ''
  name: codebuildRoleArn
  type: object
- description: ''
  name: componentRoleArn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: environmentAccountConnectionId
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: protonServiceRoleArn
  type: object
- description: ''
  name: provisioningRepository
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
schema_file: json-schema/amazon-proton-create-environment-input-schema.json
slug: amazon-proton-create-environment-input
source_filename: amazon-proton-create-environment-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-environment-input-schema.json\",\n  \"title\": \"CreateEnvironmentInput\",\n  \"description\": \"CreateEnvironmentInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codebuildRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM service role that allows Proton to provision infrastructure using CodeBuild-based provisioning on your behalf.</p> <p>To use CodeBuild-based provisioning for the environment or for any service instance running in the environment, specify either the <code>environmentAccountConnectionId</code> or <code>codebuildRoleArn</code> parameter.</p>\"\n        }\n      ]\n    },\n    \"componentRoleArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM service role that Proton uses when provisioning directly defined components in this environment. It determines the scope of infrastructure that a component can provision.</p> <p>You must specify <code>componentRoleArn</code> to allow directly defined components to be associated with this environment.</p> <p>For more information about components, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-components.html\\\">Proton components</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the environment that's being created and deployed.\"\n        }\n      ]\n    },\n    \"environmentAccountConnectionId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionId\"\n        },\n        {\n          \"description\": \"<p>The ID of the environment account connection that you provide if you're provisioning your environment infrastructure resources to an environment account. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-env-account-connections.html\\\">Environment account connections</a> in the <i>Proton User guide</i>.</p> <p>To use Amazon Web Services-managed provisioning for the environment, specify either the <code>environmentAccountConnectionId</code> or <code>protonServiceRoleArn</code> parameter and omit the <code>provisioningRepository</code> parameter.</p>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment.\"\n        }\n\
  \      ]\n    },\n    \"protonServiceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the Proton service role that allows Proton to make calls to other services on your behalf.</p> <p>To use Amazon Web Services-managed provisioning for the environment, specify either the <code>environmentAccountConnectionId</code> or <code>protonServiceRoleArn</code> parameter and omit the <code>provisioningRepository</code> parameter.</p>\"\n        }\n      ]\n    },\n    \"provisioningRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryBranchInput\"\n        },\n        {\n          \"description\": \"<p>The linked repository that you use to host your rendered infrastructure templates for self-managed provisioning. A linked repository is a repository that has been registered with Proton. For more information, see <a>CreateRepository</a>.</p>\
  \ <p>To use self-managed provisioning for the environment, specify this parameter and omit the <code>environmentAccountConnectionId</code> and <code>protonServiceRoleArn</code> parameters.</p>\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"A YAML formatted string that provides inputs as defined in the environment template bundle schema file. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-environments.html\\\">Environments</a> in the <i>Proton User Guide</i>.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An optional list of metadata items that you can associate with the Proton environment. A tag is a key-value pair.</p> <p>For more information, see <a href=\\\"\
  https://docs.aws.amazon.com/proton/latest/userguide/resources.html\\\">Proton resources and tagging</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"templateMajorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The major version of the environment template.\"\n        }\n      ]\n    },\n    \"templateMinorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The minor version of the environment template.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment template. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-templates.html\\\
  \">Environment Templates</a> in the <i>Proton User Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"spec\",\n    \"templateMajorVersion\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-environment-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateEnvironmentInput
---
