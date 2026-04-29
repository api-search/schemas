---
description: Proton settings that are used for multiple services in the Amazon Web Services account.
layout: schema
name: AccountSettings
properties_list:
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
schema_file: json-schema/amazon-proton-account-settings-schema.json
slug: amazon-proton-account-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-account-settings-schema.json\",\n  \"title\": \"AccountSettings\",\n  \"description\": \"Proton settings that are used for multiple services in the Amazon Web Services account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineCodebuildRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArnOrEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the service role that Proton uses for provisioning pipelines. Proton assumes this role for CodeBuild-based provisioning.\"\n        }\n      ]\n    },\n    \"pipelineProvisioningRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryBranch\"\n        },\n        {\n          \"description\": \"The linked repository\
  \ for pipeline provisioning. Required if you have environments configured for self-managed provisioning with services that include pipelines. A linked repository is a repository that has been registered with Proton. For more information, see <a>CreateRepository</a>.\"\n        }\n      ]\n    },\n    \"pipelineServiceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArnOrEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the service role you want to use for provisioning pipelines. Assumed by Proton for Amazon Web Services-managed provisioning, and by customer-owned automation for self-managed provisioning.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-account-settings-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: AccountSettings
---
