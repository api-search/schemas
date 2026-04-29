---
description: Summary data of an Proton environment account connection resource.
layout: schema
name: EnvironmentAccountConnectionSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: componentRoleArn
  type: object
- description: ''
  name: environmentAccountId
  type: object
- description: ''
  name: environmentName
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: lastModifiedAt
  type: object
- description: ''
  name: managementAccountId
  type: object
- description: ''
  name: requestedAt
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-environment-account-connection-summary-schema.json
slug: amazon-proton-environment-account-connection-summary
source_filename: amazon-proton-environment-account-connection-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-account-connection-summary-schema.json\",\n  \"title\": \"EnvironmentAccountConnectionSummary\",\n  \"description\": \"Summary data of an Proton environment account connection resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the environment account connection.\"\n        }\n      ]\n    },\n    \"componentRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM service role that Proton uses when provisioning directly defined components\
  \ in the associated environment account. It determines the scope of infrastructure that a component can provision in the account.</p> <p>The environment account connection must have a <code>componentRoleArn</code> to allow directly defined components to be associated with any environments running in the account.</p> <p>For more information about components, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-components.html\\\">Proton components</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"environmentAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccountId\"\n        },\n        {\n          \"description\": \"The ID of the environment account that's connected to the environment account connection.\"\n        }\n      ]\n    },\n    \"environmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\"\
  : \"The name of the environment that's associated with the environment account connection.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionId\"\n        },\n        {\n          \"description\": \"The ID of the environment account connection.\"\n        }\n      ]\n    },\n    \"lastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the environment account connection was last modified.\"\n        }\n      ]\n    },\n    \"managementAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccountId\"\n        },\n        {\n          \"description\": \"The ID of the management account that's connected to the environment account connection.\"\n        }\n      ]\n    },\n    \"requestedAt\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the environment account connection request was made.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The IAM service role that's associated with the environment account connection.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionStatus\"\n        },\n        {\n          \"description\": \"The status of the environment account connection.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"environmentAccountId\",\n    \"environmentName\",\n    \"id\",\n    \"lastModifiedAt\",\n    \"managementAccountId\",\n    \"requestedAt\",\n    \"roleArn\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-account-connection-summary-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: EnvironmentAccountConnectionSummary
---
