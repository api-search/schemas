---
description: A proposed grant configuration for a KMS key. For more information, see <a href="https://docs.aws.amazon.com/kms/latest/APIReference/API_CreateGrant.html">CreateGrant</a>.
layout: schema
name: KmsGrantConfiguration
properties_list:
- description: ''
  name: operations
  type: object
- description: ''
  name: granteePrincipal
  type: object
- description: ''
  name: retiringPrincipal
  type: object
- description: ''
  name: constraints
  type: object
- description: ''
  name: issuingAccount
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-kms-grant-configuration-schema.json
slug: iam-access-analyzer-kms-grant-configuration
source_filename: iam-access-analyzer-kms-grant-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-kms-grant-configuration-schema.json\",\n  \"title\": \"KmsGrantConfiguration\",\n  \"description\": \"A proposed grant configuration for a KMS key. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/APIReference/API_CreateGrant.html\\\">CreateGrant</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsGrantOperationsList\"\n        },\n        {\n          \"description\": \"A list of operations that the grant permits.\"\n        }\n      ]\n    },\n    \"granteePrincipal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GranteePrincipal\"\n        },\n        {\n          \"description\": \"The principal that is given\
  \ permission to perform the operations that the grant permits.\"\n        }\n      ]\n    },\n    \"retiringPrincipal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetiringPrincipal\"\n        },\n        {\n          \"description\": \"The principal that is given permission to retire the grant by using <a href=\\\"https://docs.aws.amazon.com/kms/latest/APIReference/API_RetireGrant.html\\\">RetireGrant</a> operation.\"\n        }\n      ]\n    },\n    \"constraints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsGrantConstraints\"\n        },\n        {\n          \"description\": \"Use this structure to propose allowing <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#cryptographic-operations\\\">cryptographic operations</a> in the grant only when the operation request includes the specified <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\\\
  \">encryption context</a>.\"\n        }\n      ]\n    },\n    \"issuingAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IssuingAccount\"\n        },\n        {\n          \"description\": \" The Amazon Web Services account under which the grant was issued. The account is used to propose KMS grants issued by accounts other than the owner of the key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"operations\",\n    \"granteePrincipal\",\n    \"issuingAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-kms-grant-configuration-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: KmsGrantConfiguration
---
