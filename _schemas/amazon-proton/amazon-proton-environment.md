---
description: Detailed data of an Proton environment resource. An Proton environment is a set of resources shared across Proton services.
layout: schema
name: Environment
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: codebuildRoleArn
  type: object
- description: ''
  name: componentRoleArn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: deploymentStatus
  type: object
- description: ''
  name: deploymentStatusMessage
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: environmentAccountConnectionId
  type: object
- description: ''
  name: environmentAccountId
  type: object
- description: ''
  name: lastDeploymentAttemptedAt
  type: object
- description: ''
  name: lastDeploymentSucceededAt
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: protonServiceRoleArn
  type: object
- description: ''
  name: provisioning
  type: object
- description: ''
  name: provisioningRepository
  type: object
- description: ''
  name: spec
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
schema_file: json-schema/amazon-proton-environment-schema.json
slug: amazon-proton-environment
source_filename: amazon-proton-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-schema.json\",\n  \"title\": \"Environment\",\n  \"description\": \"Detailed data of an Proton environment resource. An Proton environment is a set of resources shared across Proton services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the environment.\"\n        }\n      ]\n    },\n    \"codebuildRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM service role that allows Proton to provision infrastructure using CodeBuild-based provisioning on\
  \ your behalf.\"\n        }\n      ]\n    },\n    \"componentRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM service role that Proton uses when provisioning directly defined components in this environment. It determines the scope of infrastructure that a component can provision.</p> <p>The environment must have a <code>componentRoleArn</code> to allow directly defined components to be associated with the environment.</p> <p>For more information about components, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-components.html\\\">Proton components</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the environment was created.\"\
  \n        }\n      ]\n    },\n    \"deploymentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The environment deployment status.\"\n        }\n      ]\n    },\n    \"deploymentStatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"An environment deployment status message.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the environment.\"\n        }\n      ]\n    },\n    \"environmentAccountConnectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionId\"\n        },\n        {\n          \"description\": \"The ID of the environment account connection\
  \ that's used to provision infrastructure resources in an environment account.\"\n        }\n      ]\n    },\n    \"environmentAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccountId\"\n        },\n        {\n          \"description\": \"The ID of the environment account that the environment infrastructure resources are provisioned in.\"\n        }\n      ]\n    },\n    \"lastDeploymentAttemptedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when a deployment of the environment was last attempted.\"\n        }\n      ]\n    },\n    \"lastDeploymentSucceededAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the environment was last deployed successfully.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment.\"\n        }\n      ]\n    },\n    \"protonServiceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Proton service role that allows Proton to make calls to other services on your behalf.\"\n        }\n      ]\n    },\n    \"provisioning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Provisioning\"\n        },\n        {\n          \"description\": \"When included, indicates that the environment template is for customer provisioned and managed infrastructure.\"\n        }\n      ]\n    },\n    \"provisioningRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryBranch\"\n        },\n        {\n          \"description\": \"The linked\
  \ repository that you use to host your rendered infrastructure templates for self-managed provisioning. A linked repository is a repository that has been registered with Proton. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/APIReference/API_CreateRepository.html\\\">CreateRepository</a>.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"The environment spec.\"\n        }\n      ]\n    },\n    \"templateMajorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The major version of the environment template.\"\n        }\n      ]\n    },\n    \"templateMinorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\"\
  : \"The minor version of the environment template.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the environment template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"deploymentStatus\",\n    \"lastDeploymentAttemptedAt\",\n    \"lastDeploymentSucceededAt\",\n    \"name\",\n    \"templateMajorVersion\",\n    \"templateMinorVersion\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-environment-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: Environment
---
