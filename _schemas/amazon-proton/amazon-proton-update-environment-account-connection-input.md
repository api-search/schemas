---
description: UpdateEnvironmentAccountConnectionInput schema from Amazon Proton API
layout: schema
name: UpdateEnvironmentAccountConnectionInput
properties_list:
- description: ''
  name: codebuildRoleArn
  type: object
- description: ''
  name: componentRoleArn
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: roleArn
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-environment-account-connection-input-schema.json
slug: amazon-proton-update-environment-account-connection-input
source_filename: amazon-proton-update-environment-account-connection-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-environment-account-connection-input-schema.json\",\n  \"title\": \"UpdateEnvironmentAccountConnectionInput\",\n  \"description\": \"UpdateEnvironmentAccountConnectionInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codebuildRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an IAM service role in the environment account. Proton uses this role to provision infrastructure resources using CodeBuild-based provisioning in the associated environment account.\"\n        }\n      ]\n    },\n    \"componentRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n \
  \       {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM service role that Proton uses when provisioning directly defined components in the associated environment account. It determines the scope of infrastructure that a component can provision in the account.</p> <p>The environment account connection must have a <code>componentRoleArn</code> to allow directly defined components to be associated with any environments running in the account.</p> <p>For more information about components, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-components.html\\\">Proton components</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionId\"\n        },\n        {\n          \"description\": \"The ID of the environment account connection to update.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM service role that's associated with the environment account connection to update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-environment-account-connection-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateEnvironmentAccountConnectionInput
---
