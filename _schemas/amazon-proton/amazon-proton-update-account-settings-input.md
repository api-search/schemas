---
description: UpdateAccountSettingsInput schema from Amazon Proton API
layout: schema
name: UpdateAccountSettingsInput
properties_list:
- description: ''
  name: deletePipelineProvisioningRepository
  type: object
- description: ''
  name: pipelineCodebuildRoleArn
  type: object
- description: ''
  name: pipelineProvisioningRepository
  type: object
- description: ''
  name: pipelineServiceRoleArn
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-account-settings-input-schema.json
slug: amazon-proton-update-account-settings-input
source_filename: amazon-proton-update-account-settings-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-account-settings-input-schema.json\",\n  \"title\": \"UpdateAccountSettingsInput\",\n  \"description\": \"UpdateAccountSettingsInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deletePipelineProvisioningRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Set to <code>true</code> to remove a configured pipeline repository from the account settings. Don't set this field if you are updating the configured pipeline repository.\"\n        }\n      ]\n    },\n    \"pipelineCodebuildRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArnOrEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon\
  \ Resource Name (ARN) of the service role you want to use for provisioning pipelines. Proton assumes this role for CodeBuild-based provisioning.\"\n        }\n      ]\n    },\n    \"pipelineProvisioningRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryBranchInput\"\n        },\n        {\n          \"description\": \"<p>A linked repository for pipeline provisioning. Specify it if you have environments configured for self-managed provisioning with services that include pipelines. A linked repository is a repository that has been registered with Proton. For more information, see <a>CreateRepository</a>.</p> <p>To remove a previously configured repository, set <code>deletePipelineProvisioningRepository</code> to <code>true</code>, and don't set <code>pipelineProvisioningRepository</code>.</p>\"\n        }\n      ]\n    },\n    \"pipelineServiceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArnOrEmptyString\"\
  \n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the service role you want to use for provisioning pipelines. Assumed by Proton for Amazon Web Services-managed provisioning, and by customer-owned automation for self-managed provisioning.</p> <p>To remove a previously configured ARN, specify an empty string.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-account-settings-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateAccountSettingsInput
---
