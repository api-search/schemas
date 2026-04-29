---
description: A complex type that contains optional Amazon Web Services Key Management Service (KMS) encryption settings for your Network Firewall resources. Your data is encrypted by default with an Amazon Web Services owned key that Amazon Web Services owns and manages for you. You can use either the Amazon Web Services owned key, or provide your own customer managed key. To learn more about KMS encryption of your Network Firewall resources, see <a href="https://docs.aws.amazon.com/kms/latest/developerguide/kms-encryption-at-rest.html">Encryption at rest with Amazon Web Services Key Managment Service</a> in the <i>Network Firewall Developer Guide</i>.
layout: schema
name: EncryptionConfiguration
properties_list:
- description: ''
  name: KeyId
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-encryption-configuration-schema.json
slug: openapi-encryption-configuration
source_filename: openapi-encryption-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-encryption-configuration-schema.json\",\n  \"title\": \"EncryptionConfiguration\",\n  \"description\": \"A complex type that contains optional Amazon Web Services Key Management Service (KMS) encryption settings for your Network Firewall resources. Your data is encrypted by default with an Amazon Web Services owned key that Amazon Web Services owns and manages for you. You can use either the Amazon Web Services owned key, or provide your own customer managed key. To learn more about KMS encryption of your Network Firewall resources, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/kms-encryption-at-rest.html\\\">Encryption at rest with Amazon Web Services Key Managment Service</a> in the <i>Network Firewall Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\"\
  : {\n    \"KeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services Key Management Service (KMS) customer managed key. You can use any of the key identifiers that KMS supports, unless you're using a key that's managed by another account. If you're using a key managed by another account, then specify the key ARN. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id\\\">Key ID</a> in the <i>Amazon Web Services KMS Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionType\"\n        },\n        {\n          \"description\": \"The type of Amazon Web Services KMS key to use for encryption of your Network Firewall resources.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-encryption-configuration-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: EncryptionConfiguration
---
