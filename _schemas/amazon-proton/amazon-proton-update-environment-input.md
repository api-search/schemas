---
description: UpdateEnvironmentInput schema from Amazon Proton API
layout: schema
name: UpdateEnvironmentInput
properties_list:
- description: ''
  name: codebuildRoleArn
  type: object
- description: ''
  name: componentRoleArn
  type: object
- description: ''
  name: deploymentType
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
  name: templateMajorVersion
  type: object
- description: ''
  name: templateMinorVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-environment-input-schema.json
slug: amazon-proton-update-environment-input
source_filename: amazon-proton-update-environment-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-environment-input-schema.json\",\n  \"title\": \"UpdateEnvironmentInput\",\n  \"description\": \"UpdateEnvironmentInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codebuildRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM service role that allows Proton to provision infrastructure using CodeBuild-based provisioning on your behalf.\"\n        }\n      ]\n    },\n    \"componentRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM service role that Proton uses when\
  \ provisioning directly defined components in this environment. It determines the scope of infrastructure that a component can provision.</p> <p>The environment must have a <code>componentRoleArn</code> to allow directly defined components to be associated with the environment.</p> <p>For more information about components, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-components.html\\\">Proton components</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"deploymentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentUpdateType\"\n        },\n        {\n          \"description\": \"<p>There are four modes for updating an environment. The <code>deploymentType</code> field defines the mode.</p> <dl> <dt/> <dd> <p> <code>NONE</code> </p> <p>In this mode, a deployment <i>doesn't</i> occur. Only the requested metadata parameters are updated.</p> </dd> <dt/> <dd> <p> <code>CURRENT_VERSION</code> </p>\
  \ <p>In this mode, the environment is deployed and updated with the new spec that you provide. Only requested parameters are updated. <i>Don\\u2019t</i> include major or minor version parameters when you use this <code>deployment-type</code>.</p> </dd> <dt/> <dd> <p> <code>MINOR_VERSION</code> </p> <p>In this mode, the environment is deployed and updated with the published, recommended (latest) minor version of the current major version in use, by default. You can also specify a different minor version of the current major version in use.</p> </dd> <dt/> <dd> <p> <code>MAJOR_VERSION</code> </p> <p>In this mode, the environment is deployed and updated with the published, recommended (latest) major and minor version of the current template, by default. You can also specify a different major version that is higher than the major version in use and a minor version (optional).</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the environment update.\"\n        }\n      ]\n    },\n    \"environmentAccountConnectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionId\"\n        },\n        {\n          \"description\": \"<p>The ID of the environment account connection.</p> <p>You can only update to a new environment account connection if it was created in the same environment account that the current environment account connection was created in and is associated with the current environment.</p>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment to update.\"\n        }\n      ]\n    },\n    \"protonServiceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Proton service role that allows Proton to make API calls to other services your behalf.\"\n        }\n      ]\n    },\n    \"provisioningRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryBranchInput\"\n        },\n        {\n          \"description\": \"The linked repository that you use to host your rendered infrastructure templates for self-managed provisioning. A linked repository is a repository that has been registered with Proton. For more information, see <a>CreateRepository</a>.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"The formatted specification that defines the update.\"\n        }\n      ]\n    },\n    \"templateMajorVersion\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The major version of the environment to update.\"\n        }\n      ]\n    },\n    \"templateMinorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The minor version of the environment to update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentType\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-environment-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateEnvironmentInput
---
