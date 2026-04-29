---
description: The proposed access control configuration for an IAM role. You can propose a configuration for a new IAM role or an existing IAM role that you own by specifying the trust policy. If the configuration is for a new IAM role, you must specify the trust policy. If the configuration is for an existing IAM role that you own and you do not propose the trust policy, the access preview uses the existing trust policy for the role. The proposed trust policy cannot be an empty string. For more information about role trust policy limits, see <a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_iam-quotas.html">IAM and STS quotas</a>.
layout: schema
name: IamRoleConfiguration
properties_list:
- description: ''
  name: trustPolicy
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-iam-role-configuration-schema.json
slug: iam-access-analyzer-iam-role-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-iam-role-configuration-schema.json\",\n  \"title\": \"IamRoleConfiguration\",\n  \"description\": \"The proposed access control configuration for an IAM role. You can propose a configuration for a new IAM role or an existing IAM role that you own by specifying the trust policy. If the configuration is for a new IAM role, you must specify the trust policy. If the configuration is for an existing IAM role that you own and you do not propose the trust policy, the access preview uses the existing trust policy for the role. The proposed trust policy cannot be an empty string. For more information about role trust policy limits, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_iam-quotas.html\\\">IAM and STS quotas</a>.\",\n  \"type\": \"object\",\n  \"\
  properties\": {\n    \"trustPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamTrustPolicy\"\n        },\n        {\n          \"description\": \"The proposed trust policy for the IAM role.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-iam-role-configuration-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: IamRoleConfiguration
---
