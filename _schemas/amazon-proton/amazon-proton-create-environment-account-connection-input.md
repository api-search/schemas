---
description: CreateEnvironmentAccountConnectionInput schema from Amazon Proton API
layout: schema
name: CreateEnvironmentAccountConnectionInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: codebuildRoleArn
  type: object
- description: ''
  name: componentRoleArn
  type: object
- description: ''
  name: environmentName
  type: object
- description: ''
  name: managementAccountId
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-environment-account-connection-input-schema.json
slug: amazon-proton-create-environment-account-connection-input
source_filename: amazon-proton-create-environment-account-connection-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-environment-account-connection-input-schema.json\",\n  \"title\": \"CreateEnvironmentAccountConnectionInput\",\n  \"description\": \"CreateEnvironmentAccountConnectionInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"When included, if two identical requests are made with the same client token, Proton returns the environment account connection that the first request created.\"\n        }\n      ]\n    },\n    \"codebuildRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource\
  \ Name (ARN) of an IAM service role in the environment account. Proton uses this role to provision infrastructure resources using CodeBuild-based provisioning in the associated environment account.\"\n        }\n      ]\n    },\n    \"componentRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM service role that Proton uses when provisioning directly defined components in the associated environment account. It determines the scope of infrastructure that a component can provision in the account.</p> <p>You must specify <code>componentRoleArn</code> to allow directly defined components to be associated with any environments running in this account.</p> <p>For more information about components, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-components.html\\\">Proton components</a> in the <i>Proton User Guide</i>.</p>\"\n \
  \       }\n      ]\n    },\n    \"environmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the Proton environment that's created in the associated management account.\"\n        }\n      ]\n    },\n    \"managementAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccountId\"\n        },\n        {\n          \"description\": \"The ID of the management account that accepts or rejects the environment account connection. You create and manage the Proton environment in this account. If the management account accepts the environment account connection, Proton can use the associated IAM role to provision environment infrastructure resources in the associated environment account.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n       \
  \ {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM service role that's created in the environment account. Proton uses this role to provision infrastructure resources in the associated environment account.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An optional list of metadata items that you can associate with the Proton environment account connection. A tag is a key-value pair.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/resources.html\\\">Proton resources and tagging</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentName\",\n    \"managementAccountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-environment-account-connection-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateEnvironmentAccountConnectionInput
---
