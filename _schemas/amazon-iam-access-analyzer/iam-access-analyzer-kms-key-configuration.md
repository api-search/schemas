---
description: <p>Proposed access control configuration for a KMS key. You can propose a configuration for a new KMS key or an existing KMS key that you own by specifying the key policy and KMS grant configuration. If the configuration is for an existing key and you do not specify the key policy, the access preview uses the existing policy for the key. If the access preview is for a new resource and you do not specify the key policy, then the access preview uses the default key policy. The proposed key policy cannot be an empty string. For more information, see <a href="https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html#key-policy-default">Default key policy</a>. For more information about key policy limits, see <a href="https://docs.aws.amazon.com/kms/latest/developerguide/resource-limits.html">Resource quotas</a>.</p> <p/>
layout: schema
name: KmsKeyConfiguration
properties_list:
- description: ''
  name: keyPolicies
  type: object
- description: ''
  name: grants
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-kms-key-configuration-schema.json
slug: iam-access-analyzer-kms-key-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-kms-key-configuration-schema.json\",\n  \"title\": \"KmsKeyConfiguration\",\n  \"description\": \"<p>Proposed access control configuration for a KMS key. You can propose a configuration for a new KMS key or an existing KMS key that you own by specifying the key policy and KMS grant configuration. If the configuration is for an existing key and you do not specify the key policy, the access preview uses the existing policy for the key. If the access preview is for a new resource and you do not specify the key policy, then the access preview uses the default key policy. The proposed key policy cannot be an empty string. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html#key-policy-default\\\">Default key policy</a>.\
  \ For more information about key policy limits, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/resource-limits.html\\\">Resource quotas</a>.</p> <p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyPoliciesMap\"\n        },\n        {\n          \"description\": \"Resource policy configuration for the KMS key. The only valid value for the name of the key policy is <code>default</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html#key-policy-default\\\">Default key policy</a>.\"\n        }\n      ]\n    },\n    \"grants\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsGrantConfigurationsList\"\n        },\n        {\n          \"description\": \"A list of proposed grant configurations for the KMS key. If the proposed grant configuration is for an existing key, the\
  \ access preview uses the proposed list of grant configurations in place of the existing grants. Otherwise, the access preview uses the existing grants for the key.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-kms-key-configuration-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: KmsKeyConfiguration
---
